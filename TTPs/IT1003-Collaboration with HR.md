# **Collaboration with HR**

ID: IT1003

Tactic: Proactive Measures

Platform: Linux / Mac / Mobile / Windows

Permissions Required: Standard

Data Sources: Tools

Version: 1.0

Created: 04/28/2020

Last Modified: 01/13/2025

---

## **Overview:**

Building a strong partnership with the Human Resources (HR) department is essential for an effective Insider Threat program. HR collaboration provides valuable insights into key policies, stakeholders, and employee status, including Performance Improvement Plans (PIP), disciplinary actions, and layoffs. This information helps security teams proactively address potential insider threats and improve investigative capabilities.

---
https://github.com/Insider-Threat/Insider-Threat/blob/master/TTPs/IT1003-Collaboration%20with%20HR.md
## **Example Scenario:**

| **Name**              | **Description**                                                                                      |
|------------------------|------------------------------------------------------------------------------------------------------|
| Disciplinary Action Alert | HR informs the Insider Threat team about an employee facing termination due to repeated policy violations. This prompts closer monitoring of the individual’s activities. |
| Layoff Risk Monitoring  | HR notifies the Insider Threat team about a department-wide layoff. Security increases monitoring of impacted employees for data exfiltration attempts. |

---

## **Mitigations**

1. Establish regular communication channels between HR and the Insider Threat team to share relevant updates.  
2. Develop workflows to ensure timely notification of employees under disciplinary actions or PIPs.  
3. Implement access restrictions for employees flagged by HR to minimize risk.  
4. Conduct cross-functional training with HR to align on insider threat prevention strategies.  

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
| HR Flagged Employee Alert | Detects flagged employees based on updates from HR (e.g., PIPs or disciplinary actions).       | [Example Link](#) | High           |
| Layoff Watchlist Alert   | Monitors activity for employees identified as part of a layoff or workforce reduction.          | [Example Link](#) | Medium         |
| Termination Monitoring   | Tracks account activity for employees terminated but still having access to company resources.  | [Example Link](#) | High           |
