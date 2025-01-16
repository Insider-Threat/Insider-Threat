# **Activity Outside of Normal Scope**

ID: IT1012

Tactic: Initial Discovery

Platform: Linux / Mac / Mobile / Windows

Permissions Required: Standard

Data Sources: Application / Authentication / Endpoint / Network / Tools

Version: 1.1

Created: 04/28/2020

Last Modified: 01/16/2025

---

## **Overview:**

An employee's job function typically defines their access needs and expected activities. When a user attempts to access data or systems outside their normal scope, it may indicate malicious intent, curiosity, or a potential insider threat. Such activities, especially when targeting sensitive information, should be flagged and investigated promptly to prevent unauthorized data access or theft.

---

## **Example Scenario:**

| **Name**                   | **Description**                                                                                      |
|----------------------------|------------------------------------------------------------------------------------------------------|
| Employee Collecting Data   | An IT Operations team member responsible for provisioning laptops begins searching for source code related to a new product under development. |
| Unauthorized System Access | A sales employee tries to access an internal database containing financial reports unrelated to their role. |

---

## **Mitigations**

1. Restrict access to sensitive data and systems using role-based access controls (RBAC).  
2. Monitor access patterns and flag attempts to retrieve data outside an employee’s role or department.  
3. Conduct regular audits of user permissions to ensure access aligns with job functions.  
4. Deploy user behavior analytics (UBA) tools to detect deviations from normal activity patterns.  
5. Provide employee training on acceptable use policies and the consequences of unauthorized access.  

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
| Role Access Violation Alert | Flags attempts to access resources or systems not aligned with the user’s role or job function. | [Example Link](#) | High           |
| Sensitive Data Access Alert | Monitors access to sensitive or restricted files by users outside the designated access group. | [Example Link](#) | High           |
| Behavioral Anomaly Alert  | Detects deviations in user behavior, such as accessing unusual systems or data.                 | [Example Link](#) | Medium         |
| Unauthorized Query Alert  | Tracks attempts to query or search internal databases for information unrelated to the user’s job. | [Example Link](#) | Medium         |
