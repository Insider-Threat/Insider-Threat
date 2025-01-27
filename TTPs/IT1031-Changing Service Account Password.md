# **Changing Service Account Password**

ID: IT1031

Tactic: Business Impact

Platform: Linux / Mac / Mobile / Windows

Permissions Required: Admin

Data Sources: Application / Authentication / Endpoint / Network / Tools / Email

Version: 1.1

Created: 04/28/2020

Last Modified: 01/27/2025

---

## **Overview:**

Service accounts are critical for ensuring the proper operation of applications and services. These accounts are often used to execute essential commands or functions automatically. Unauthorized or uncoordinated password changes to service accounts can cause service outages, disrupt business operations, and create security risks. Proper monitoring and role-based access controls are essential to mitigate these risks.

---

## **Example Scenario:**

| **Name**                              | **Description**                                                                                      |
|---------------------------------------|------------------------------------------------------------------------------------------------------|
| **Malicious Changing of Password**    | A disgruntled employee with admin privileges changes the password of a critical service account without notifying the team or updating the applications that use the account, causing an outage and disrupting business operations. |
| **Accidental Password Change**        | An IT administrator mistakenly changes the password of a service account and forgets to update the dependent services, leading to widespread service failures. |
| **Unauthorized Access to Service Accounts** | An insider intentionally modifies the credentials of a service account to create downtime or hinder investigations into malicious activity. |

---

## **Mitigations**

1. Restrict access to service account management to a limited group of authorized administrators.  
2. Use account/password management tools that enforce role-based access controls (RBAC) and maintain audit logs.  
3. Implement a password rotation policy for service accounts, ensuring that changes are planned, documented, and synchronized across all dependent applications.  
4. Require multi-factor authentication (MFA) for all administrative actions, including service account password changes.  
5. Ensure more than one person has admin-level access to critical applications and services to prevent single points of failure.  
6. Automate service account password updates using tools that synchronize changes across all dependent systems.  

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
| Unauthorized Password Change Alert | Flags password changes made to critical service accounts without proper authorization or approvals. | [Example Link](#) | High           |
| Service Account Failure Alert  | Detects repeated authentication failures for a service account, potentially indicating an uncoordinated password change. | [Example Link](#) | High           |
| Behavioral Anomaly Alert       | Identifies unusual admin activity, such as unexpected modifications to service accounts outside of normal maintenance windows. | [Example Link](#) | Medium         |
| Outage Trigger Alert           | Monitors applications for unexpected downtime linked to service account authentication issues.   | [Example Link](#) | High           |


