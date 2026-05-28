# **Copying Sensitive Data to Clipboard**  

ID: IT1054  

Tactic: Collection  

Platform: Linux / Mac / Mobile / Windows  

Permissions Required: Standard  

Data Sources: Application Logs / Clipboard Monitoring / DLP Events / Endpoint Logs / File Monitoring / Process Monitoring  

Version: 1.0  

Created: 05/28/2026  

Last Modified: 05/28/2026  

---

## **Overview:**  

Employees may collect sensitive company information by **copying data to the clipboard** from business applications, source code repositories, customer systems, financial platforms, internal documents, or privileged consoles. Clipboard activity can be a precursor to exfiltration through chat, email, browser uploads, personal notes, AI tools, or unmanaged cloud services.  

This behavior may be legitimate during normal work, but it becomes higher risk when users copy large amounts of data, copy from sensitive systems outside their usual role, or copy content shortly before resignation, termination, or access changes.  

Organizations should monitor clipboard activity in context with source application, data classification, user role, destination application, and other behaviors such as screenshots, file downloads, archive creation, or uploads to external services.  

---

## **Example Scenario:**  

| **Name** | **Description** |
|---------|---------------|
| **Customer Record Copying** | A user copies rows of customer information from a CRM system before pasting the data into a personal spreadsheet. |
| **Source Code Snippet Collection** | A developer copies proprietary code from an internal repository into an unmanaged editor or personal notes application. |
| **Credential Copying** | An administrator copies secrets, API keys, or connection strings from a vault or configuration portal outside normal maintenance activity. |
| **Prompt Preparation** | An employee copies confidential content from internal documents before submitting it to an external AI or summarization tool. |

---

## **Mitigations:**  

1. **Apply DLP controls** to clipboard events involving sensitive labels, regulated data, source code, or credentials.  
2. **Restrict copy and paste** from high-risk applications where business workflows allow stronger controls.  
3. **Monitor clipboard activity** by source application, user role, sensitivity label, volume, and destination application.  
4. **Alert on clipboard activity** that occurs alongside bulk downloads, screenshots, archive creation, or external uploads.  
5. **Increase monitoring for elevated-risk users** during offboarding, investigation, or access review periods.  
6. **Educate employees** on approved handling of sensitive data and the risks of pasting corporate data into unmanaged tools.  

---

## **Groups Applied To:**  

| **Group Name**                | **Monitoring (Yes/No)** |
|--------------------------------|:----------------------:|
| R&D                            | Yes/No               |
| Sales                          | Yes/No               |
| Executives and Executive Assistants | Yes/No         |
| IT Operations/InfoSec          | Yes/No               |
| Support Staff/Everyone Else    | Yes/No               |

---

## **Detection:**  

| **Name** | **Description** | **Link** | **Risk Score** |
|---------|---------------|--------|--------------|
| **Sensitive Clipboard Copy Alert** | Detects sensitive or regulated data copied from monitored applications. | [Example Link](#) | Medium |
| **Credential Clipboard Alert** | Flags copying of secrets, API keys, access tokens, or connection strings. | [Example Link](#) | High |
| **Clipboard to Unmanaged App Alert** | Identifies sensitive data copied from a corporate source and pasted into an unmanaged application or browser destination. | [Example Link](#) | High |
| **Departing User Clipboard Spike** | Correlates increased clipboard activity with resignation, termination, or other elevated-risk HR indicators. | [Example Link](#) | Medium |

---

### **Additional Considerations**  

1. **Why It’s Critical:**  
   - Clipboard activity can be an early collection signal before data is moved through email, cloud storage, AI tools, chat, or screenshots.  
   - Copy and paste behavior may bypass controls that only focus on file downloads or direct uploads.  

2. **Broader Monitoring:**  
   - Correlate clipboard telemetry with **DLP, endpoint, browser, application, and identity events.**  
   - Tune alerts carefully to reduce noise from normal work while still surfacing unusual copying from sensitive systems.  

---

