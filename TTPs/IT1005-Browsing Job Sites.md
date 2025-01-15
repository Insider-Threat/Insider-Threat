# **Browsing Job Sites**

ID: IT1005

Tactic: Initial Discovery

Platform: Linux / Mac / Mobile / Windows

Permissions Required: Standard

Data Sources: Network Traffic, Endpoint Data

Version: 1.1

Created: 04/28/2020

Last Modified: 01/15/2025

---

## **Overview:**

Employees seeking new opportunities may also pose a risk of data exfiltration before departing the company. Identifying and investigating anomalous activity, such as browsing job sites or accessing data outside their normal duties, is critical to preventing the loss of sensitive or valuable data. Behavioral deviations may signal malicious intent or preparatory actions.

---

## **Example Scenario:**

| **Name**                       | **Description**                                                                                      |
|--------------------------------|------------------------------------------------------------------------------------------------------|
| Browsing Competitor Careers Site | An employee looking to leave the company visits competitors' career pages for open positions.        |
| Frequent Job Board Access       | An employee repeatedly visits general job boards (e.g., LinkedIn Jobs, Indeed) during work hours.    |

---

## **Mitigations**

1. Remove all access to company systems and sensitive data immediately upon resignation or termination.  
2. Require employees to sign an acknowledgment before their last day, confirming they are not taking company data.  
3. Monitor for anomalous data access or downloads during the employee’s notice period.  
4. Establish policies and communication encouraging employees to raise career concerns before seeking external opportunities.  

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
| Job Site Browsing Alert  | Detects access to known job or competitor career sites from company systems.                   | [Example Link](#) | Medium         |
| Anomalous Behavior Alert | Identifies deviations from normal behavior, such as accessing data outside the employee’s role. | [Example Link](#) | High           |
| Data Download Alert      | Tracks unusual file downloads or transfers during the employee’s notice period.                | [Example Link](#) | High           |
