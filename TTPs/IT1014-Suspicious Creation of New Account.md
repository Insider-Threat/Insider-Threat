# **Suspicious Creation of New Account**

ID: IT1014

Tactic: Initial Discovery

Platform: Linux / Mac / Mobile / Windows

Permissions Required: Standard

Data Sources: Application / Authentication / Endpoint / Network / Tools

Version: 1.1

Created: 04/28/2020

Last Modified: 01/16/2025

---

## **Overview:**

Employees with privileged access or the ability to create new accounts pose a unique risk. They may create unauthorized accounts to gain access to sensitive systems or data, either before their departure or as a method to establish persistence for post-departure access. Monitoring for suspicious account creation activity is critical to prevent unauthorized access and mitigate insider threats.

---

## **Example Scenario:**

| **Name**                      | **Description**                                                                                      |
|-------------------------------|------------------------------------------------------------------------------------------------------|
| Employee Creating Persistence | An employee creates a new account with elevated privileges to access the company’s environment after their main user account is deactivated. |
| Unauthorized Account Creation  | A privileged user creates an account without a valid business justification, flagging potential misuse of their elevated access. |

---

## **Mitigations**

1. Regularly review and audit account creation or modification activity by users with elevated privileges.  
2. Revoke all elevated privileges immediately when an employee resigns or is terminated.  
3. Implement alerts for account creation activity, particularly accounts with elevated privileges or access to sensitive systems.  
4. Enforce the principle of least privilege (POLP) by ensuring users have only the access necessary for their roles.  
5. Require dual approval for creating accounts with elevated permissions or access to sensitive data.  

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
| Unauthorized Account Creation Alert | Flags new account creation activity without a valid business justification or approval.          | [Example Link](#) | High           |
| Elevated Privilege Account Creation Alert | Monitors for accounts created with administrative or elevated privileges.                     | [Example Link](#) | High           |
| Account Creation Post-Resignation Alert | Tracks account creation activity for users who have submitted a resignation notice.            | [Example Link](#) | Medium         |
| Anomalous Account Activity Alert  | Detects account creation outside standard working hours or from unusual locations.               | [Example Link](#) | Medium         |
