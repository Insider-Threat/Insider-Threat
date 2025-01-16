# **Downloads from Intranet**

ID: IT1022

Tactic: Collection

Platform: Linux / Mac / Mobile / Windows

Permissions Required: Admin

Data Sources: Application / Authentication / Endpoint / Network / Tools / Email

Version: 1.1

Created: 04/28/2020

Last Modified: 01/16/2025

---

## **Overview:**

Bulk or unusual downloads from intranet systems may indicate that a user is staging data for unauthorized use or exfiltration. The intranet often contains sensitive information such as internal policies, procedures, project data, or intellectual property. Monitoring and controlling intranet downloads are essential to prevent data misuse and insider threats.

---

## **Example Scenario:**

| **Name**                     | **Description**                                                                                      |
|------------------------------|------------------------------------------------------------------------------------------------------|
| Bulk Downloads               | An employee planning to resign accesses intranet repositories, downloads a large volume of files, and stores them locally before transferring them to an external hard drive. |
| Unauthorized Repository Access | A user accesses and downloads files from intranet sections or directories unrelated to their role, indicating potential data staging. |

---

## **Mitigations**

1. Enforce role-based access controls (RBAC) on intranet sections, restricting access to authorized users.  
2. Monitor intranet download activity, flagging anomalies such as high-volume downloads or access to sensitive areas.  
3. Use Data Loss Prevention (DLP) tools to prevent unauthorized downloads and transfers from intranet systems.  
4. Regularly audit access permissions for intranet repositories to ensure compliance with least-privilege principles.  
5. Educate employees on acceptable use policies and the consequences of unauthorized intranet data handling.  

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
| Bulk Intranet Download Alert   | Flags users downloading an unusually large volume of data from intranet repositories.            | [Example Link](#) | High           |
| Repository Access Anomaly Alert | Detects access to intranet sections or files outside a user’s normal scope.                     | [Example Link](#) | Medium         |
| Data Transfer Alert            | Monitors for data downloaded from the intranet being transferred to unapproved locations or devices. | [Example Link](#) | High           |
| Behavioral Anomaly Alert       | Identifies deviations in user behavior, such as accessing sensitive intranet directories during unusual hours. | [Example Link](#) | Medium         |

