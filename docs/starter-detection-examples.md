# Starter Detection Examples

These examples are intentionally generic. Treat them as detection patterns to adapt to your SIEM, EDR, DLP, CASB, or SaaS audit platform.

## IT1024: Upload to 3rd Party File Share

**Intent:** Detect sensitive files uploaded to unmanaged storage providers.

```kql
CloudUploadEvents
| where DestinationService in ("Dropbox", "Box", "Google Drive", "OneDrive Personal", "Mega")
| where IsManagedDestination == false
| where SensitivityLabel in ("Confidential", "Restricted", "Secret")
| summarize FileCount=count(), Bytes=sum(BytesUploaded) by User, DestinationService, bin(TimeGenerated, 1h)
| where FileCount >= 5 or Bytes >= 50000000
```

## IT1025: External Email with Attachments

**Intent:** Detect unusual external attachment activity.

```kql
EmailEvents
| where RecipientDomain !in (CorporateDomains)
| where AttachmentCount > 0
| summarize Messages=count(), Attachments=sum(AttachmentCount), Bytes=sum(AttachmentBytes) by Sender, RecipientDomain, bin(TimeGenerated, 1d)
| where Messages >= 5 or Bytes >= 25000000
```

## IT1026: Upload to Removable Storage Device

**Intent:** Detect sensitive file copies to removable media.

```kql
DeviceFileEvents
| where ActionType in ("FileCopied", "FileCreated")
| where DestinationDeviceType == "RemovableMedia"
| where SensitivityLabel in ("Confidential", "Restricted", "Secret")
| summarize FileCount=count(), Bytes=sum(FileSize) by User, DeviceName, RemovableDeviceId, bin(TimeGenerated, 1h)
| where FileCount >= 3 or Bytes >= 25000000
```

## IT1039: Exposure of Sensitive/Confidential Information in Public Repositories

**Intent:** Detect public repository exposure of sensitive content or secrets.

```kql
CodeRepositoryEvents
| where RepositoryVisibility == "Public"
| where EventType in ("Push", "CreateRepository", "ChangeVisibility")
| where SecretDetected == true or SensitivityMatch == true
| project TimeGenerated, User, Repository, EventType, SecretType, FilePath
```

## IT1040: Use of File Share Site with External User

**Intent:** Detect external sharing of sensitive files.

```kql
SaaSFileEvents
| where EventType in ("FileShared", "LinkCreated", "ExternalUserAdded")
| where IsExternal == true
| where SensitivityLabel in ("Confidential", "Restricted", "Secret")
| summarize SharedItems=count(), ExternalTargets=make_set(ExternalDomain, 20) by User, SourceApp, bin(TimeGenerated, 1d)
| where SharedItems >= 3
```

## IT1042: Multiple Employees Leaving to Same Company

**Intent:** Correlate clustered departures with pre-departure data activity.

```kql
HREvents
| where EventType == "Resignation" and NewEmployer != ""
| summarize Departures=count(), Employees=make_set(User, 50) by NewEmployer, Department, bin(EventDate, 30d)
| where Departures >= 2
| join kind=leftouter (
    FileActivity
    | where ActivityDate between (ago(45d) .. now())
    | summarize Downloads=count(), Bytes=sum(BytesAccessed) by User
) on $left.Employees has $right.User
```

## IT1051: Unauthorized OAuth Application Consent

**Intent:** Detect risky third-party application consent.

```kql
OAuthConsentEvents
| where ConsentType in ("UserConsent", "AdminConsent")
| where AppVerified == false or RiskyScope == true
| where Scopes has_any ("Mail.Read", "Files.Read.All", "offline_access", "Sites.Read.All")
| project TimeGenerated, User, AppName, Publisher, Scopes, ConsentType, AppId
```

## IT1052: Sensitive Data in External AI Tools

**Intent:** Detect uploads or prompt submissions of sensitive data to unmanaged AI services.

```kql
WebOrDlpEvents
| where DestinationCategory == "Generative AI"
| where IsManagedService == false
| where EventType in ("FileUpload", "Post", "Paste")
| where SensitivityLabel in ("Confidential", "Restricted", "Secret") or SecretDetected == true
| project TimeGenerated, User, DestinationHost, EventType, SensitivityLabel, FileName, Bytes
```

## IT1053: Personal Cloud Sync Client

**Intent:** Detect unmanaged sync clients and sensitive file staging.

```kql
DeviceProcessEvents
| where ProcessName in ("dropbox.exe", "googledrivefs.exe", "onedrive.exe", "mega.exe")
| where AccountType == "Personal" or IsApprovedApplication == false
| join kind=leftouter (
    DeviceFileEvents
    | where FolderPath has_any ("Dropbox", "Google Drive", "OneDrive", "MEGA")
    | where SensitivityLabel in ("Confidential", "Restricted", "Secret")
) on DeviceId, User
| summarize Events=count(), Files=countif(isnotempty(FileName)) by User, DeviceName, ProcessName, bin(TimeGenerated, 1d)
```

## IT1054: Copying Sensitive Data to Clipboard

**Intent:** Detect sensitive clipboard activity from monitored applications.

```kql
EndpointDlpEvents
| where ActionType in ("ClipboardCopy", "ClipboardPaste")
| where SensitivityLabel in ("Confidential", "Restricted", "Secret") or SecretDetected == true
| summarize Events=count(), Sources=make_set(SourceApplication, 20), Destinations=make_set(DestinationApplication, 20) by User, bin(TimeGenerated, 1h)
| where Events >= 5
```

## Tuning Notes

- Replace placeholder table and field names with your platform schema.
- Add approved application and domain allowlists.
- Add peer-group baselines for high-volume roles.
- Combine with HR or employment context only under approved governance.
- Treat first alerts as leads for review, not automatic conclusions.

