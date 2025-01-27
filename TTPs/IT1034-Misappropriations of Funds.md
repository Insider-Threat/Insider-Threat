# **Misappropriations of Funds**

ID: IT1034

Tactic: Business Impact

Platform: Linux / Mac / Mobile / Windows

Permissions Required: Admin

Data Sources: Application / Authentication / Endpoint / Network / Tools / Email / Financial Systems

Version: 1.1

Created: 04/28/2020

Last Modified: 01/27/2025

---

## **Overview:**

Employees are often entrusted with access to company funds, credit cards, or procurement systems to make purchases or transactions on behalf of their employer. When an employee abuses this trust by misappropriating funds for personal gain, it can lead to financial losses and reputational harm. Common examples include falsifying expense reports, misusing corporate credit cards, or inflating invoices to embezzle money. Monitoring and enforcing strict financial policies is critical to detect and prevent these activities.

---

## **Example Scenario:**

| **Name**                           | **Description**                                                                                      |
|------------------------------------|------------------------------------------------------------------------------------------------------|
| **Misuse of Credit Card**          | An employee with a company credit card purchases a large number of gift cards and keeps them for personal use, falsely claiming they were distributed as employee rewards. |
| **Falsified Expense Reports**      | An insider submits expense reports with fabricated receipts or inflated amounts, pocketing the difference. |
| **Unauthorized Vendor Payments**   | A user creates a fake vendor and directs payments to their personal account, embezzling funds from the company. |
| **Abuse of Procurement System**    | An employee uses a procurement system to order high-value items (e.g., electronics) for personal use, claiming they are for a business need. |

---

## **Mitigations**

1. Implement automated expense tracking systems that flag unusual transactions, such as high-value purchases or gift card expenses.  
2. Require all expense reports to be reviewed and approved by a manager or supervisor, with clear audit trails.  
3. Establish and enforce clear policies outlining acceptable uses of company funds, with mandatory training for employees.  
4. Conduct regular audits of company credit card usage and vendor payments to identify discrepancies or patterns of misuse.  
5. Use financial monitoring tools to detect anomalies in transactions, such as duplicate payments or unauthorized purchases.  

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
| Expense Anomaly Alert          | Flags high-value or unusual transactions submitted through expense reports or credit card logs.  | [Example Link](#) | High           |
| Duplicate Payment Alert        | Detects duplicate or suspiciously similar payments made to vendors or employees.                | [Example Link](#) | Medium         |
| Vendor Creation Alert          | Monitors for the creation of new vendors with incomplete or suspicious details.                  | [Example Link](#) | High           |
| Procurement System Misuse Alert| Flags unusual orders, such as electronics or high-value items, not tied to a documented business need. | [Example Link](#) | High           |


