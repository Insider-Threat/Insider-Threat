# **Upload to Removable Storage Device**

ID: IT1026

Tactic: Exfiltration

Platform: Linux / Mac / Mobile / Windows

Permissions Required: Admin

Data Sources: Application / Authentication / Endpoint / Network / Tools / Email

Version: 1.1

Created: 04/28/2020

Last Modified: 01/27/2025

---

## **Overview:**

Removable storage devices, such as USB drives and external hard drives, provide an easy way for individuals to transfer large amounts of data quickly. Abnormal or unauthorized transfers to such devices, particularly when they deviate from a user’s normal activity, may indicate staging or data exfiltration. Additionally, creating backups of corporate systems or devices onto non-work-related drives introduces further risk, as sensitive information can be easily exported and misused.

---

## **Example Scenario:**

| **Name**                                | **Description**                                                                                      |
|-----------------------------------------|------------------------------------------------------------------------------------------------------|
| Data Exfiltration via External Hard Drive | An employee planning to resign gathers sensitive data from internal repositories, stores it locally, and transfers the files to an external hard drive for later use. |
| Computer Backup to Personal Drive        | A user creates a complete backup of their corporate laptop, including sensitive emails and proprietary files, and transfers it to a personal external hard drive. |

---

## **Mitigations**

1. Use endpoint protection tools to monitor and block unauthorized use of removable storage devices.  
2. Enforce policies to disable USB ports on corporate devices unless explicitly required for business purposes.  
3. Employ Data Loss Prevention (DLP) tools to prevent sensitive data transfers to external storage devices.  
4. Regularly audit USB and external storage usage logs for signs of unusual activity.  
5. Block or restrict backup tools from writing to unauthorized drives or personal external storage devices.  
6. Provide training to employees on data handling policies, including restrictions on removable storage devices and personal backups.  

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
| USB Activity Alert             | Flags the use of removable storage devices for data transfers, especially large file transfers. | [Example Link](#) | High           |
| Anomalous Data Transfer Alert  | Detects significant data transfers to removable storage devices that deviate from normal behavior. | [Example Link](#) | High           |
| Sensitive Data Transfer Alert  | Monitors transfers of sensitive files, such as customer lists or proprietary documents, to external drives. | [Example Link](#) | High           |
| Backup File Transfer Alert     | Tracks attempts to transfer complete system backups to non-work-related drives.                 | [Example Link](#) | High           |
| File Integrity Alert           | Tracks changes to local files before large transfers to removable storage devices.              | [Example Link](#) | Medium         |


