# **Correspondence with Competitors**

ID: IT1009

Tactic: Initial Discovery

Platform: Linux / Mac / Mobile / Windows

Permissions Required: Standard

Data Sources: HR Data / Application / Authentication / Endpoint / Network / Sensitive Information Storage Locations / Tools

Version: 1.0

Created: 04/28/2020

Last Modified: 01/15/2025

---

## **Overview:**

Correspondence with a competitor is atypical behavior that may signal potential insider threats. Such communication could indicate an employee is unhappy with their role, attempting to disclose sensitive information, or exploring opportunities with a competitor. These interactions can occur through email, online chat, forums, or even social media. Proactive monitoring and swift investigation of such behavior are essential to safeguard proprietary information.

---

## **Example Scenario:**

| **Name**                      | **Description**                                                                                      |
|-------------------------------|------------------------------------------------------------------------------------------------------|
| Sensitive Data Disclosure     | An unhappy employee emails a competitor, sharing sensitive project details in hopes of securing a job offer. |
| Unauthorized Collaboration     | An employee uses a professional networking platform (e.g., LinkedIn) to share confidential company strategies with a competitor. |
| Insider Recruitment Attempt   | An employee is contacted by a competitor and agrees to transfer proprietary data as part of a recruitment effort. |

---

## **Mitigations**

1. Monitor email and chat communications for known competitor domains or mentions of confidential projects.  
2. Implement Data Loss Prevention (DLP) tools to detect and block the sharing of sensitive files or information.  
3. Educate employees about the risks and consequences of sharing proprietary information, including legal and ethical ramifications.  
4. Restrict access to sensitive data for employees flagged for unusual communication behavior.  
5. Collaborate with HR to identify employees who may be at risk of engaging in such activity due to dissatisfaction or external pressures.  

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
| Competitor Email Alert   | Flags emails sent to competitor domains or containing mentions of confidential topics.          | [Example Link](#) | High           |
| Social Media Monitoring Alert | Detects mentions of sensitive company information on social platforms like LinkedIn or forums.       | [Example Link](#) | Medium         |
| Unauthorized File Sharing Alert | Tracks file uploads to unauthorized platforms or domains, including competitor systems.                | [Example Link](#) | High           |
| Network Communication Alert | Monitors unusual patterns of outbound communications to external IPs associated with competitors.       | [Example Link](#) | Medium         |
