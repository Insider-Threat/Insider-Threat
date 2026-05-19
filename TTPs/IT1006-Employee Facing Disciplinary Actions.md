# **Employee Facing Disciplinary Actions**

ID: IT1006

Tactic: Initial Discovery

Platform: Linux / Mac / Mobile / Windows

Permissions Required: Standard

Data Sources: HR Data

Version: 1.1

Created: 04/28/2020

Last Modified: 01/15/2025

---

## **Overview:**

When an employee is facing disciplinary action, such as being placed on a performance improvement plan (PIP), reported for misconduct, or involved in a harassment complaint, the risk of insider threats may increase. Employees in these situations might feel resentment or fear termination, potentially leading to harmful actions like data exfiltration, sabotage, or retaliation.  

Proactive monitoring during these periods helps prevent malicious activity, safeguard sensitive information, and ensure that investigations are conducted with integrity. Additionally, close collaboration with HR ensures timely identification of high-risk situations and appropriate mitigations.

---

## **Example Scenario:**

| **Name**                          | **Description**                                                                                      |
|-----------------------------------|------------------------------------------------------------------------------------------------------|
| Employee Reported for Ethics Violation | An employee is accused of falsifying reports. Upon learning of the investigation, they delete evidence and email sensitive files to their personal account in anticipation of termination. |
| Employee on Performance Review    | An employee under a formal performance improvement plan begins downloading large amounts of sensitive data unrelated to their role. |
| Harassment Complaint              | An employee accused of harassment attempts to access private HR files to discover who reported them and retaliate. |
| Misuse of Access                  | An employee facing termination escalates their privileges or accesses sensitive files in an attempt to harm the company. |

---

## **Mitigations**

1. Proactively monitor employees accused of policy violations, harassment, or poor performance, focusing on anomalous activity such as data downloads or unauthorized access.  
2. Temporarily restrict access to sensitive systems or data until the investigation concludes.  
3. Educate employees on corporate policies and consequences of malicious actions during investigations.  
4. Collaborate with HR to implement clear escalation processes for employees facing disciplinary actions.  
5. Review logs of data access and monitor for potential misuse before disciplinary actions are communicated.  

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
| Data Deletion Alert      | Flags mass deletions or suspicious file removals by the employee under investigation.           | [Example Link](#) | High           |
| Unauthorized Email Activity Alert | Monitors for emails containing sensitive files sent to personal or external accounts.            | [Example Link](#) | High           |
| Privileged Access Alert  | Detects attempts to access systems or data outside the employee’s normal role during the investigation. | [Example Link](#) | Medium         |
| Unauthorized HR Data Access | Flags attempts to access sensitive HR data, such as complaint records or employee reviews.             | [Example Link](#) | High           |
| Anomalous Download Alert | Tracks large-scale downloads of sensitive files unrelated to the employee’s regular responsibilities.    | [Example Link](#) | High           |
