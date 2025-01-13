# **Prevent Backups to Unapproved Storage Locations**

ID: IT1001

Tactic: Proactive Measures

Platform: Linux / Mac / Mobile / Windows

Permissions Required: Standard

Data Sources: Tools

Version: 1.0

Created: 04/28/2020

Last Modified: 01/13/2025

---

## **Overview:**

Companies should enforce policies to designate approved locations for backups, ensuring data is securely managed and recoverable in compliance with organizational standards. Backups to unapproved devices, such as an employee's personal external drive, pose a risk of data leakage and must be restricted.

---

## **Example Scenario:**

| **Name**               | **Description**                                                                                      |
|-------------------------|------------------------------------------------------------------------------------------------------|
| Backup to External Drive | An employee, planning to leave the company, backs up their work laptop to a personal external drive to retain company data. |

---

## **Mitigations**

1. Use Group Policies to disable or restrict backup functionality to unapproved storage devices.  
2. Deploy DLP tools to monitor and block unauthorized data transfers to external drives.  
3. Configure Anti-Virus or Endpoint Detection tools to detect and alert on unauthorized backup attempts.  
4. Educate employees on the risks and consequences of improper data backups.  

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

| **Name**                | **Description**                                                                                 | **Link**          | **Risk Score** |
|-------------------------|-------------------------------------------------------------------------------------------------|-------------------|:--------------:|
| External Backup Alert    | Detects backup attempts to unauthorized external storage devices.                              | [Example Link](#) | High           |
| Unauthorized File Copy Alert | Flags large-scale file transfers to unapproved storage locations.                            | [Example Link](#) | Medium         |
| Backup Tool Activity Alert | Monitors activity from backup tools (e.g., external hard drive connection logs).              | [Example Link](#) | High           |
