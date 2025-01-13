# **DLP Enforcement**

ID: IT1000

Tactic: Proactive Measures

Platform: Linux / Mac / Mobile / Windows

Permissions Required: Standard

Data Sources: Tools

Version: 1.0

Created: 04/28/2020

Last Modified: 01/13/2025

---

## **Overview:**

Data Loss Prevention (DLP) tools assist in detecting when sensitive information, such as Intellectual Property (e.g., source code) or Personally Identifiable Information (PII) (e.g., name, date of birth, driver's license number), is being transferred.  
DLP systems use predefined rules, keywords, or machine learning to scan files, emails, and uploads for sensitive data patterns. By automating detection, they help prevent accidental and malicious data breaches.

---

## **Procedure Examples:**

DLP tools monitor for sensitive data transfers, including Intellectual Property or PII. These tools scan files based on specific criteria and alert the Security Operations Center (SOC) team when matches are detected. Upon receiving an alert, the SOC team investigates to validate the detection.

### **Example Scenarios:**

1. **Unauthorized File Transfer:**  
   An employee working on a project needs to send a file to a third party. The DLP tool scans the file and detects source code, generating an alert. The SOC team investigates and finds the transfer is unauthorized, preventing the potential breach.

2. **False Positive - Legitimate Use Case:**  
   An employee sends encrypted customer records to an approved vendor. The DLP tool flags the transmission due to encryption patterns. After investigation, the SOC team verifies the transfer is authorized and clears the alert.

---

## **Mitigations**

1. Block or prevent data transfers when the DLP tool detects sensitive information.  
2. Display a pop-up message to inform employees of sensitive data detection and allow them to stop the transfer.  
3. Provide periodic training to employees on recognizing and handling sensitive data.  
4. Conduct regular tests of DLP rules to ensure they are configured accurately and minimize false positives.  
5. Review and update DLP rules to align with evolving compliance standards and organizational policies.

---

## **Groups Applied To:**

| Group Name                        | Monitoring (Yes/No) |
|-----------------------------------|:-------------------:|
| R&D                               | Yes/No              |
| Sales                             | Yes/No              |
| Executives and Executive Assistants | Yes/No            |
| IT Operations/InfoSec             | Yes/No              |
| Support Staff/Everyone Else       | Yes/No              |

---

## **Detection**

| Name              | Description                                                      | Link             | Risk Score |
|-------------------|------------------------------------------------------------------|------------------|:----------:|
| File Transfer Alert | Detects file transfers containing Intellectual Property (e.g., source code). | [Example Link](#) | High       |
| PII Email Alert   | Detects PII (e.g., SSN, credit card numbers) sent via email to external domains. | [Example Link](#) | Medium     |
| USB Copy Alert    | Flags attempts to copy sensitive files onto unauthorized USB devices. | [Example Link](#) | High       |
