# **Modify/Delete Logs**

ID: IT1016

Tactic: Initial Discovery

Platform: Linux / Mac / Mobile / Windows

Permissions Required: Standard

Data Sources: Application / Authentication / Endpoint / Network / Tools / Email

Version: 1.1

Created: 04/28/2020

Last Modified: 01/16/2025

---

## **Overview:**

Logs are critical for tracking user activity, system operations, and incident investigations. Attempting to modify or delete logs is highly irregular and often indicates an effort to conceal unauthorized actions. By altering log files, a user can potentially erase evidence of malicious activity, making detection and mitigation essential for preserving the integrity of forensic data.

---

## **Example Scenario:**

| **Name**                 | **Description**                                                                                      |
|--------------------------|------------------------------------------------------------------------------------------------------|
| Concealing Activity      | A user deletes log entries that show they performed an unauthorized change to a critical system to conceal their involvement in a business outage. |
| Disabling Logging         | A user modifies system settings to reduce or stop logging entirely, preventing future activity from being recorded. |

---

## **Mitigations**

1. Enforce access controls to prevent unauthorized users from modifying or deleting logs.  
2. Implement immutable logging solutions that prevent alteration or deletion of log files.  
3. Configure alerting for any changes to log configurations or unexpected gaps in logging activity.  
4. Regularly audit logging systems to ensure logging integrity and proper configuration.  
5. Use centralized logging systems that store logs in secure, tamper-proof locations separate from the originating systems.  

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

| **Name**                        | **Description**                                                                                 | **Link**          | **Risk Score** |
|---------------------------------|-------------------------------------------------------------------------------------------------|-------------------|:--------------:|
| Log Deletion Alert              | Flags attempts to delete log files or entries from critical systems.                           | [Example Link](#) | High           |
| Logging Disabled Alert          | Monitors for attempts to disable or reduce logging levels on systems or applications.          | [Example Link](#) | High           |
| Log Tampering Alert             | Detects changes to log files that are inconsistent with normal system processes.               | [Example Link](#) | Medium         |
| Gaps in Logging Activity Alert  | Identifies unexpected interruptions or gaps in expected log entries.                          | [Example Link](#) | Medium         |


