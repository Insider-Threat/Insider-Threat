# **Corporate Restructuring/Reduction in Workforce**

ID: IT1008

Tactic: Initial Discovery

Platform: Linux / Mac / Mobile / Windows

Permissions Required: Standard

Data Sources: HR Data / Application / Authentication / Endpoint / Network / Sensitive Information Storage Locations / Tools

Version: 1.1

Created: 04/28/2020

Last Modified: 01/15/2025

---

## **Overview:**

During corporate restructuring or workforce reduction events, both impacted and non-impacted employees may pose an insider threat risk. Impacted employees may attempt to exfiltrate intellectual property or sensitive data as they prepare to leave the company.  

Non-impacted employees, feeling stressed about their own job security or acting out of loyalty to coworkers who were let go, may also engage in harmful activities. This could include sabotage, unauthorized access, or data theft as a form of revenge. Proactive monitoring and clear communication during these events are essential to mitigate risks and protect company assets.

---

## **Example Scenario:**

| **Name**                      | **Description**                                                                                      |
|-------------------------------|------------------------------------------------------------------------------------------------------|
| Reduction in Force (RIF)      | An employee notified of a RIF downloads all Confluence pages and SharePoint files from their business unit to their laptop. They copy these files to a personal external hard drive, triggering an alert for the SOC team to investigate. |
| Restructuring Announcement    | After a restructuring announcement, an employee begins accessing sensitive files outside their usual scope, including proprietary project data. |
| Non-Impacted Employee Action  | A non-impacted employee, feeling stressed about potential job losses, attempts to download proprietary data or delete important files as an act of revenge for their terminated coworkers. |

---

## **Mitigations**

1. Collaborate closely with HR and Authentication teams to reduce access to sensitive data for impacted employees immediately after notification.  
2. Use DLP tools to block unauthorized transfers of intellectual property to external devices or cloud storage.  
3. Provide clear communication to all employees, including non-impacted staff, about acceptable data handling practices and enforce strict policies.  
4. Monitor for behavioral anomalies among non-impacted employees, including sudden changes in data access patterns.  
5. Implement enhanced monitoring for large-scale downloads, unauthorized access, and unusual activity during restructuring events.  
6. Conduct exit interviews to ensure all company assets, including data, are accounted for.

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
| Large-Scale Download Alert | Flags significant data downloads from impacted employees following notification of restructuring. | [Example Link](#) | High           |
| Unauthorized USB Alert    | Detects data transfers to unauthorized external devices.                                       | [Example Link](#) | Medium         |
| Access Anomaly Alert      | Tracks access to sensitive files outside the employee’s usual scope or role.                  | [Example Link](#) | High           |
| Cloud Upload Alert        | Monitors uploads to personal or unapproved cloud storage services.                            | [Example Link](#) | High           |
| Privileged Access Attempt Alert | Detects attempts to elevate privileges or access restricted systems post-restructuring announcement. | [Example Link](#) | Medium         |
| Behavioral Anomaly Alert  | Monitors for unusual behavior, such as sudden data access by non-impacted employees.           | [Example Link](#) | High           |
