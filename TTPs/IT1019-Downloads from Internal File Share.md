# **Downloads from Internal File Share**

ID: IT1019

Tactic: Collection

Platform: Linux / Mac / Mobile / Windows

Permissions Required: Admin

Data Sources: Application / Authentication / Endpoint / Network / Tools / Email

Version: 1.0

Created: 04/28/2020

Last Modified: 01/14/2025

---

## **Overview:**

Large or unusual data transfers from internal file shares may indicate that a user is staging data for unauthorized use or exfiltration. This behavior, particularly when inconsistent with a user’s normal activity patterns, could signal malicious intent, preparation for resignation, or insider threat activity. Monitoring such downloads is critical for protecting sensitive information and identifying potential risks.

---

## **Example Scenario:**

| **Name**                     | **Description**                                                                                      |
|------------------------------|------------------------------------------------------------------------------------------------------|
| Bulk Downloads               | An employee planning to resign downloads large volumes of files from internal file shares and stores them locally before transferring them to an external hard drive. |
| Unusual Repository Access    | A user accesses and downloads files from shared drives or repositories they don’t typically interact with, raising suspicion of unauthorized activity. |

---

## **Mitigations**

1. Enforce role-based access controls (RBAC) on internal file shares to restrict access to authorized users.  
2. Monitor file share activity for unusual download patterns, such as high-volume downloads or access to sensitive directories.  
3. Use Data Loss Prevention (DLP) tools to block unauthorized data transfers from file shares.  
4. Implement logging and anomaly detection systems to identify deviations from normal user activity.  
5. Provide employees with training on data protection policies and reinforce the consequences of unauthorized data handling.  

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
| Large File Share Download Alert | Flags instances of users downloading an unusually large volume of data from internal file shares. | [Example Link](#) | High           |
| Access Anomaly Alert           | Detects access to shared folders or files outside a user’s typical scope of activity.           | [Example Link](#) | Medium         |
| Data Transfer Alert            | Tracks transfers of files from file shares to external devices or unapproved cloud services.     | [Example Link](#) | High           |
| Behavioral Anomaly Alert       | Identifies deviations in user behavior, such as accessing or downloading files at unusual times. | [Example Link](#) | Medium         |


