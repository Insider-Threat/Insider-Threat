# **Upload to 3rd Party File Share**

ID: IT1024

Tactic: Exfiltration

Platform: Linux / Mac / Mobile / Windows

Permissions Required: Admin

Data Sources: Application / Authentication / Endpoint / Network / Tools / Email

Version: 1.1

Created: 04/28/2020

Last Modified: 01/16/2025

---

## **Overview:**

Third-party or unapproved file-sharing platforms, such as Google Drive, Dropbox, GitHub, and Box, are often free and easy to use, making them an appealing option for individuals attempting to exfiltrate data. Unauthorized uploads to these platforms can bypass corporate security controls, enabling individuals to access sensitive data outside the corporate environment. Monitoring and restricting uploads to such platforms is critical to prevent data breaches.

---

## **Example Scenario:**

| **Name**                     | **Description**                                                                                      |
|------------------------------|------------------------------------------------------------------------------------------------------|
| Bulk Data Export             | An employee planning to resign gathers sensitive data from various repositories and transfers it to an external file-sharing platform, such as Google Drive or Dropbox, to access it after leaving the company. |
| Unauthorized Code Sharing     | A user uploads proprietary source code to a public repository on GitHub without approval, exposing sensitive intellectual property. |

---

## **Mitigations**

1. Monitor and restrict large data transfers to unapproved file-sharing platforms.  
2. Block access to unauthorized file-sharing sites through network security tools, such as firewalls or proxy servers.  
3. Use Data Loss Prevention (DLP) tools to detect and prevent unauthorized uploads of sensitive files.  
4. Educate employees on acceptable use policies and the risks associated with using third-party file-sharing platforms.  
5. Regularly audit logs of data transfers to external platforms and investigate any anomalies.  

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
| Large File Upload Alert        | Flags users uploading unusually large files or data volumes to third-party platforms.            | [Example Link](#) | High           |
| Unauthorized Platform Alert    | Detects attempts to access or transfer data to unapproved file-sharing services.                | [Example Link](#) | High           |
| Source Code Sharing Alert      | Monitors for uploads of proprietary source code to public repositories like GitHub.             | [Example Link](#) | High           |
| Anomalous Transfer Alert       | Identifies unusual patterns of data transfer activity to external platforms.                    | [Example Link](#) | Medium         |

