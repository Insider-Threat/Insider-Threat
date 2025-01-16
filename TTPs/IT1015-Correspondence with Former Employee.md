# **Correspondence with Former Employee**

ID: IT1015

Tactic: Initial Discovery

Platform: Linux / Mac / Mobile / Windows

Permissions Required: Standard

Data Sources: Application / Authentication / Endpoint / Network / Tools / Email

Version: 1.1

Created: 04/28/2020

Last Modified: 01/16/2025

---

## **Overview:**

Former employees who have left the company, especially those now working for competitors, may contact current employees to solicit sensitive information, proprietary data, or encourage them to leave the company. These interactions can occur via email, messaging apps, or social media. Detecting and investigating such correspondence is critical to safeguarding sensitive data and mitigating insider threat risks.

---

## **Example Scenario:**

| **Name**                       | **Description**                                                                                      |
|--------------------------------|------------------------------------------------------------------------------------------------------|
| Former Employee Communications | An employee leaves to work for a competitor and then reaches out to former colleagues, asking them to share proprietary product designs. |
| Recruitment to Competitor      | A former employee contacts a current employee, encouraging them to leave the company and bring along client lists or sensitive project data. |
| Collaborative Breach           | A former employee collaborates with a current employee to access sensitive systems by sharing login credentials or exploiting existing access. |

---

## **Mitigations**

1. Implement email monitoring and alerting for communication with domains associated with competitors or known former employees.  
2. Provide training to employees about the risks of sharing company information with former employees and the legal implications of such actions.  
3. Use Data Loss Prevention (DLP) tools to block unauthorized sharing of sensitive files or data through email or messaging platforms.  
4. Monitor access to sensitive systems or data for anomalies when correspondence with known former employees is detected.  
5. Collaborate with HR to maintain an up-to-date list of former employees, including high-risk departures (e.g., those who joined competitors).  

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

| **Name**                       | **Description**                                                                                      | **Link**          | **Risk Score** |
|--------------------------------|------------------------------------------------------------------------------------------------------|-------------------|:--------------:|
| Email Correspondence Alert     | Flags emails exchanged between current employees and known former employees.                         | [Example Link](#) | Medium         |
| Competitor Domain Alert        | Monitors emails or messages sent to domains associated with competitors or former employees.         | [Example Link](#) | High           |
| File Sharing Activity Alert    | Tracks attempts to share sensitive data through email, cloud services, or messaging apps.            | [Example Link](#) | High           |
| Behavioral Anomaly Alert       | Detects unusual access patterns or activity on sensitive systems coinciding with detected correspondence. | [Example Link](#) | Medium         |


