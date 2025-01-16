# **Downloads from Application**

ID: IT1018

Tactic: Collection

Platform: Linux / Mac / Mobile / Windows

Permissions Required: Admin

Data Sources: Application / Authentication / Endpoint / Network / Tools / Email

Version: 1.0

Created: 04/28/2020

Last Modified: 01/14/2025

---

## **Overview:**

Unusual or large data downloads from applications can indicate a user is staging data for unauthorized use or exfiltration. Such behavior, especially when deviating from normal activity patterns, may suggest preparation for resignation, data theft, or malicious intent. Detecting and mitigating these activities is critical to safeguarding sensitive information.

---

## **Example Scenario:**

| **Name**                     | **Description**                                                                                      |
|------------------------------|------------------------------------------------------------------------------------------------------|
| Bulk Downloads               | An employee planning to resign starts downloading large volumes of data from repositories, saves it locally, and later transfers it to an external hard drive. |
| Targeted Data Collection     | A user downloads files specific to a high-profile project, such as client lists or proprietary code, which are outside their regular job responsibilities. |

---

## **Mitigations**

1. Enforce role-based access controls (RBAC) on data repositories to ensure users can only access information relevant to their roles.  
2. Monitor download activity and flag unusual data transfer patterns, such as high-volume downloads or access to sensitive repositories.  
3. Use Data Loss Prevention (DLP) tools to block unauthorized downloads of sensitive files.  
4. Configure application logging to capture download activity and integrate logs with a SIEM for anomaly detection.  
5. Provide training to employees about acceptable data handling practices and the consequences of unauthorized data collection.  

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
| Large File Download Alert      | Flags instances of users downloading an unusually large volume of data within a short timeframe. | [Example Link](#) | High           |
| Repository Access Alert        | Monitors access to repositories or databases containing sensitive information outside a user’s normal scope. | [Example Link](#) | Medium         |
| Anomalous Download Pattern Alert | Detects deviations in user download behavior compared to historical activity.                   | [Example Link](#) | High           |
| External Transfer Alert        | Tracks file transfers from local storage to external devices or unapproved cloud services.       | [Example Link](#) | High           |

