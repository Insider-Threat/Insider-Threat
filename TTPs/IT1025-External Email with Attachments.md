# **External Email with Attachments**

ID: IT1025

Tactic: Exfiltration

Platform: Linux / Mac / Mobile / Windows

Permissions Required: Admin

Data Sources: Application / Authentication / Endpoint / Network / Tools / Email

Version: 1.1

Created: 04/28/2020

Last Modified: 01/27/2025

---

## **Overview:**

Exporting sensitive data through external email accounts is a common exfiltration method used by both insiders and external attackers. The simplicity of attaching files to emails and sending them to personal or third-party accounts makes this method effective and difficult to detect without proper monitoring. This activity can lead to the theft of proprietary information, customer data, or other critical business assets.

---

## **Example Scenario:**

| **Name**                     | **Description**                                                                                      |
|------------------------------|------------------------------------------------------------------------------------------------------|
| Data Exfiltration via Email  | An employee planning to work for a competitor attaches a customer list to an email and sends it to their personal email account before their last day. |
| Unauthorized Project Data Transfer | A user emails proprietary project files, such as designs or financial models, to an unapproved recipient. |

---

## **Mitigations**

1. Monitor email activity for patterns of large data transfers, especially to personal or third-party email domains.  
2. Employ email-based Data Loss Prevention (DLP) tools to detect and block unauthorized attachments containing sensitive information.  
3. Implement encryption and secure email gateways to prevent unauthorized access to corporate email systems.  
4. Restrict external email access for high-risk users or during sensitive periods, such as resignation or termination.  
5. Provide training to employees on acceptable email usage and the consequences of sending sensitive data to unauthorized accounts.  

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
| Large Email Attachment Alert   | Flags emails with unusually large file attachments sent to external domains.                    | [Example Link](#) | High           |
| External Domain Email Alert    | Detects emails sent to personal or third-party email addresses, such as Gmail or Yahoo.         | [Example Link](#) | Medium         |
| Sensitive Data Attachment Alert | Monitors for emails containing sensitive files, such as customer lists, source code, or financial data. | [Example Link](#) | High           |
| Behavioral Anomaly Alert       | Identifies deviations in email activity, such as frequent or unusual file-sharing patterns.     | [Example Link](#) | Medium         |


