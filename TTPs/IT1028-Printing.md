# **Printing**

ID: IT1028

Tactic: Exfiltration

Platform: Linux / Mac / Mobile / Windows

Permissions Required: Admin

Data Sources: Application / Authentication / Endpoint / Network / Tools / Email

Version: 1.1

Created: 04/28/2020

Last Modified: 01/27/2025

---

## **Overview:**

Printers and copiers are commonly used in organizations but are often overlooked in security monitoring. These devices can provide opportunities for data exfiltration, either by printing sensitive documents directly or exploiting stored print jobs on shared devices. Users may bypass traditional Data Loss Prevention (DLP) tools and other controls by transferring sensitive information to paper, creating a security blind spot that requires careful monitoring and mitigation.

---

## **Example Scenario:**

| **Name**                               | **Description**                                                                                      |
|----------------------------------------|------------------------------------------------------------------------------------------------------|
| **Data Exfiltration via Printer**      | A user planning to leave the company prints out sensitive project details, such as proprietary designs or technical specifications, before their final day. |
| **Sensitive Document Discovery**       | A user accesses a shared copier/printer and discovers stored print jobs, including a Vice President’s document containing confidential customer and pricing information. They reprint the file for themselves without authorization. |
| **Mass Document Printing**             | An insider planning to exfiltrate large volumes of data prints hundreds of pages of sensitive information over the course of a few days to avoid detection. |

---

## **Mitigations**

1. Configure printers and copiers to require authentication for access, preventing unauthorized viewing or printing of stored jobs.  
2. Use secure print release functionality, where users must authenticate at the device to retrieve their printed jobs.  
3. Monitor printing activity for unusual volumes or access to sensitive files, integrating logs with SIEM tools.  
4. Disable the storage of print jobs on shared devices, or limit the retention period for stored print jobs.  
5. Educate employees on proper use of shared devices and the consequences of printing sensitive information without authorization.  

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
| Large Volume Printing Alert    | Detects excessive or unusual printing activity, such as a single user printing hundreds of pages in a short time. | [Example Link](#) | High           |
| Sensitive Document Printing Alert | Monitors for printing activity involving sensitive or confidential files, such as customer lists or financial data. | [Example Link](#) | High           |
| Shared Printer Job Access Alert | Flags unauthorized access to stored print jobs on shared printers or copiers.                  | [Example Link](#) | Medium         |
| Anomalous Printing Time Alert  | Identifies printing activity outside of normal business hours, such as late at night or on weekends. | [Example Link](#) | Medium         |


