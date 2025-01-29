# **Forwarding Internal Communications to 3rd Party**

ID: IT1037  

Tactic: Business Impact  

Platform: Linux / Mac / Mobile / Windows  

Permissions Required: Admin  

Data Sources: Application / Authentication / Endpoint / Network / Tools / Email  

Version: 1.1  

Created: 04/28/2020  

Last Modified: 01/29/2025  

---

## **Overview:**  

Internal communications often contain sensitive business information, such as financial plans, mergers and acquisitions, product roadmaps, or legal matters. Unauthorized forwarding or sharing of these communications with external parties can result in reputational damage, regulatory violations, insider trading risks, or competitive disadvantages. Employees may leak information maliciously for personal or financial gain, or carelessly without understanding the potential consequences.  

Organizations must monitor email activity and enforce policies to ensure confidential communications remain internal.  

---

## **Example Scenario:**  

| **Name**                                       | **Description**                                                                                     |
|----------------------------------------------|-------------------------------------------------------------------------------------------------|
| **Leak of Mergers & Acquisitions (M&A) Plans**  | The CEO emails employees about an upcoming company acquisition that has not been publicly disclosed. An employee forwards the email to a journalist, leading to premature news coverage that negatively impacts negotiations. |
| **Sharing Confidential Strategy Documents**   | A disgruntled employee forwards internal product development plans to a competitor to undermine the company. |
| **Forwarding Financial Results Prematurely**  | A finance employee forwards an internal report with quarterly earnings before the official public release, violating insider trading laws. |

---

## **Mitigations**  

1. Implement **email security controls** that prevent or restrict email forwarding for sensitive communications.  
2. Use **Data Loss Prevention (DLP) tools** to detect and block unauthorized forwarding of emails containing sensitive information.  
3. Apply **email encryption and classification policies** to control access to confidential emails.  
4. Provide **employee security awareness training** on handling sensitive communications and the risks of unauthorized sharing.  
5. Monitor email traffic for **suspicious forwarding behavior**, such as multiple forwards to external addresses within a short time.  
6. Enforce **legal agreements (NDAs and confidentiality clauses)** to establish clear consequences for unauthorized disclosures.  

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

| **Name**                            | **Description**                                                                 | **Link**          | **Risk Score** |
|-------------------------------------|-------------------------------------------------------------------------------|-------------------|:--------------:|
| **Unauthorized Email Forwarding Alert** | Detects forwarding of internal communications to external email addresses.      | [Example Link](#) | High           |
| **Multiple External Forwarding Alert** | Flags excessive forwarding activity within a short timeframe.                     | [Example Link](#) | High           |
| **Keyword-Based Email Leak Alert**   | Triggers alerts when sensitive keywords (e.g., “Confidential,” “M&A,” “Earnings”) appear in forwarded emails. | [Example Link](#) | Medium         |
