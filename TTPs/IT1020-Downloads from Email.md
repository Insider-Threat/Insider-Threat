# **Downloads from Email**

ID: IT1020

Tactic: Collection

Platform: Linux / Mac / Mobile / Windows

Permissions Required: Admin

Data Sources: Application / Authentication / Endpoint / Network / Tools / Email

Version: 1.1

Created: 04/28/2020

Last Modified: 01/16/2025

---

## **Overview:**

Emails often contain sensitive information, including financial records, project details, and client communications. Abnormal email download activity, such as large volumes of data downloads or accessing older messages, may indicate staging or unauthorized transfer of sensitive information. Monitoring such activities is crucial to prevent data exfiltration and safeguard sensitive content.

---

## **Example Scenario:**

| **Name**                     | **Description**                                                                                      |
|------------------------------|------------------------------------------------------------------------------------------------------|
| Bulk Downloads               | An employee planning to resign accesses and downloads a large number of email attachments containing sensitive project data. They save the files locally and transfer them to an external drive. |
| Access to Archived Emails    | A user retrieves and downloads archived emails containing sensitive information, such as customer contracts or proprietary strategies, which are unrelated to their current role. |

---

## **Mitigations**

1. Implement Data Loss Prevention (DLP) tools to monitor and restrict email attachment downloads and transfers to unauthorized locations.  
2. Use role-based access controls (RBAC) to limit access to sensitive email archives and attachments.  
3. Enable alerting for abnormal email activity, such as downloading multiple attachments or accessing older email archives.  
4. Educate employees about acceptable use policies and the consequences of unauthorized email downloads or data transfers.  
5. Conduct regular audits of email access permissions, ensuring only authorized users have access to sensitive information.  

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

## **Detection**

| **Name**                       | **Description**                                                                                 | **Link**          | **Risk Score** |
|--------------------------------|-------------------------------------------------------------------------------------------------|-------------------|:--------------:|
| Bulk Email Download Alert      | Flags instances of users downloading an unusually large number of email attachments.            | [Example Link](#) | High           |
| Archive Access Alert           | Detects access to older or archived emails containing sensitive information.                    | [Example Link](#) | Medium         |
| Anomalous Email Activity Alert | Monitors deviations in email access and download behavior compared to historical patterns.       | [Example Link](#) | High           |
| External Transfer Alert        | Tracks email attachments transferred to unapproved external devices or cloud services.          | [Example Link](#) | High           |

