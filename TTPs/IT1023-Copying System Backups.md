# **Copying System Backups**

ID: IT1023

Tactic: Collection

Platform: Linux / Mac / Mobile / Windows

Permissions Required: Admin

Data Sources: Application / Authentication / Endpoint / Network / Tools / Email

Version: 1.1

Created: 04/28/2020

Last Modified: 01/16/2025

---

## **Overview:**

System, application, and endpoint backups often contain sensitive data, including configuration files, customer data, and intellectual property. These backups are typically compressed, making them easy to exfiltrate without detection. Unauthorized copying of backups can lead to significant security breaches, making it critical to monitor and control access to these files.

---

## **Example Scenario:**

| **Name**                     | **Description**                                                                                      |
|------------------------------|------------------------------------------------------------------------------------------------------|
| Backup Data Collection       | An employee planning to resign copies system backups from file repositories to their laptop and then transfers the data to an external drive for later use. |
| Unauthorized Backup Access   | A user accesses backup files containing sensitive application data and transfers them to an unapproved cloud storage service. |

---

## **Mitigations**

1. Enforce role-based access controls (RBAC) to restrict access to system and application backups to authorized personnel only.  
2. Monitor file access and copying activity for backup repositories and flag unusual behavior.  
3. Use Data Loss Prevention (DLP) tools to prevent unauthorized copying of backup files to external drives or cloud storage.  
4. Configure backup systems to use encryption, ensuring that unauthorized access does not expose sensitive information.  
5. Regularly audit access permissions for backup repositories to ensure compliance with least-privilege principles.  

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
| Backup Access Alert            | Flags instances of users accessing backup files outside their regular job responsibilities.      | [Example Link](#) | High           |
| Bulk Backup Copy Alert         | Detects large-scale copying of backup files from repositories or storage systems.               | [Example Link](#) | High           |
| Unauthorized Device Transfer Alert | Monitors transfers of backups to unapproved external devices, such as USB drives.             | [Example Link](#) | Medium         |
| Cloud Storage Upload Alert     | Tracks attempts to upload backup files to unauthorized cloud storage services.                  | [Example Link](#) | High           |

