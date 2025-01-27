# **Bulk Delete Files**

ID: IT1029

Tactic: Business Impact

Platform: Linux / Mac / Mobile / Windows

Permissions Required: Admin

Data Sources: Application / Authentication / Endpoint / Network / Tools / Email

Version: 1.1

Created: 04/28/2020

Last Modified: 01/27/2025

---

## **Overview:**

The intentional deletion of critical files or the unauthorized wiping of devices can have severe consequences for business operations, causing financial loss, reputational damage, and operational delays. Insiders with knowledge of sensitive data locations or device management systems can exploit their access to maliciously delete files, wipe devices, or disrupt business continuity. Monitoring and mitigating these activities is essential to protect company assets.

---

## **Example Scenario:**

| **Name**                        | **Description**                                                                                      |
|----------------------------------|------------------------------------------------------------------------------------------------------|
| **Malicious Destruction of Data** | An employee planning to resign maliciously deletes all files from a company’s shared drive, disrupting business operations. |
| **Unauthorized Device Wipe**     | A disgruntled IT administrator uses device management tools to remotely wipe multiple employee laptops without authorization, causing significant data loss and operational disruption. |
| **Deletion of Customer Records** | An insider with access to the CRM system erases customer records in retaliation for being passed over for a promotion. |
| **Disruption of Backup Files**   | A user deletes or corrupts backup files to prevent recovery efforts, causing extended downtime and loss of critical data. |

---

## **Mitigations**

1. Implement regular, automated backups to ensure critical data and devices can be recovered quickly in case of deletion or wiping.  
2. Restrict delete permissions and device management tool access to authorized users only.  
3. Enable file versioning on file shares to allow for easy recovery of deleted or modified files.  
4. Configure device management tools to require multi-factor authentication (MFA) and managerial approval for critical actions such as device wiping.  
5. Use Data Loss Prevention (DLP) tools to monitor and alert on bulk file deletion activities.  
6. Audit user and administrator activity regularly to identify unusual behaviors, such as unauthorized file deletions or device wipes.  

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
| Bulk File Deletion Alert       | Detects large-scale file deletion events occurring within a short timeframe.                    | [Example Link](#) | High           |
| Unauthorized Device Wipe Alert | Flags unauthorized or unusual device wipe activities performed via device management tools.     | [Example Link](#) | High           |
| Backup File Modification Alert | Monitors for deletion or corruption of backup files to prevent recovery efforts.                | [Example Link](#) | Medium         |
| Unauthorized Delete Alert      | Flags deletion activities performed by users who do not typically have delete permissions or perform such tasks. | [Example Link](#) | High           |
| Behavioral Anomaly Alert       | Identifies unusual file deletion patterns, such as deleting entire directories or sensitive files. | [Example Link](#) | Medium         |

