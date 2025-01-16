# **Suspicious Intranet Activity**

ID: IT1011

Tactic: Initial Discovery

Platform: Linux / Mac / Mobile / Windows

Permissions Required: Standard

Data Sources: Application / Endpoint / Network Logs

Version: 1.1

Created: 04/28/2020

Last Modified: 01/16/2025

---

## **Overview:**

Suspicious intranet activity involves behaviors like browsing an unusually high number of internal pages, receiving numerous access-denied responses, or searching for sensitive information such as credentials, SSH keys, passwords, or tokens. These activities may indicate that a user is attempting to locate data beyond their job scope. Identifying and investigating such behaviors is essential to prevent unauthorized data access or exfiltration.

---

## **Example Scenario:**

| **Name**                   | **Description**                                                                                      |
|----------------------------|------------------------------------------------------------------------------------------------------|
| Employee Collecting Data   | A user is observed browsing a large number of internal pages and repeatedly encountering access-denied responses. Their activity pattern is abnormal compared to their historical usage. |
| Credential Hunting         | A user searches intranet pages for sensitive information like passwords, tokens, or configuration files, potentially indicating an attempt to escalate privileges. |

---

## **Mitigations**

1. Restrict access to sensitive information by implementing role-based access controls (RBAC).  
2. Enable logging and monitoring of intranet activity, focusing on access to sensitive areas or data.  
3. Deploy behavioral analytics tools to flag anomalous browsing patterns.  
4. Conduct regular audits of permissions to ensure employees only have access to resources necessary for their job roles.  
5. Educate employees on acceptable use policies and the importance of reporting suspicious activity.  

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
| High Page View Alert     | Flags users accessing an unusually high number of intranet pages in a short time frame.         | [Example Link](#) | Medium         |
| Access Denied Alert      | Monitors for repeated access-denied responses, indicating potential unauthorized browsing.       | [Example Link](#) | High           |
| Sensitive Data Search Alert | Detects searches for credentials, passwords, tokens, or other sensitive information on intranet pages. | [Example Link](#) | High           |
| Traffic Pattern Anomaly Alert | Identifies abnormal intranet activity compared to the user’s historical behavior.                 | [Example Link](#) | Medium         |
