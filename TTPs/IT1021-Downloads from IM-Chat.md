# **Downloads from IM/Chat**

ID: IT1021

Tactic: Collection

Platform: Linux / Mac / Mobile / Windows

Permissions Required: Admin

Data Sources: Application / Authentication / Endpoint / Network / Tools / Email

Version: 1.1

Created: 04/28/2020

Last Modified: 01/16/2025

---

## **Overview:**

Instant messaging (IM) and chat platforms are often used for quick collaboration and may inadvertently store sensitive information, such as proprietary documents, financial data, or project plans. Abnormal download activity from IM/Chat platforms, particularly when inconsistent with a user’s normal behavior, could indicate an insider threat or unauthorized data staging. Monitoring these platforms is crucial to safeguard sensitive information.

---

## **Example Scenario:**

| **Name**                     | **Description**                                                                                      |
|------------------------------|------------------------------------------------------------------------------------------------------|
| Bulk Downloads               | An employee planning to resign downloads a large volume of files shared via IM/Chat, saves them locally, and later transfers the data to an external hard drive. |
| Unusual Attachment Access    | A user accesses chat attachments containing sensitive project details unrelated to their job responsibilities, raising suspicion of data collection. |

---

## **Mitigations**

1. Use Data Loss Prevention (DLP) tools to monitor and block unauthorized downloads of sensitive files shared in IM/Chat platforms.  
2. Enforce role-based access controls (RBAC) to limit access to IM/Chat channels containing sensitive information.  
3. Monitor and log file-sharing activity within IM/Chat platforms, integrating with SIEM systems to detect anomalies.  
4. Educate employees on acceptable use policies and the risks of sharing sensitive information over IM/Chat platforms.  
5. Regularly review and update permissions for IM/Chat channels to ensure compliance with data governance policies.  

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
| Bulk IM/Chat Download Alert    | Flags instances of users downloading an unusually large number of files or attachments from IM/Chat platforms. | [Example Link](#) | High           |
| Anomalous Access Alert         | Detects access to sensitive IM/Chat channels or attachments outside a user’s normal scope.      | [Example Link](#) | Medium         |
| Data Transfer Alert            | Monitors for data transferred from IM/Chat to external devices or unapproved cloud services.     | [Example Link](#) | High           |
| Behavioral Anomaly Alert       | Identifies deviations in user activity patterns, such as accessing or downloading files during unusual hours. | [Example Link](#) | Medium         |


