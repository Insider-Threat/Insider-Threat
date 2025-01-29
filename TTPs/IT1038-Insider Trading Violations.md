# **Insider Trading Violations**  

ID: IT1038  

Tactic: Business Impact  

Platform: Linux / Mac / Mobile / Windows  

Permissions Required: Admin  

Data Sources: Application / Authentication / Endpoint / Network / Tools / Email / Financial Systems  

Version: 1.1 

Created: 04/28/2020  

Last Modified: 01/29/2025  

---

## **Overview:**  

Insider trading occurs when an employee with access to material, nonpublic information (MNPI) about a company trades its stock, stock options, or other securities based on that privileged knowledge. This is illegal in many jurisdictions and can result in severe legal and financial penalties for both the individual and the company.  

Employees with access to financial reports, mergers and acquisitions (M&A) plans, product launches, or regulatory filings may attempt to profit by buying or selling shares before the information is made public. Preventing unauthorized access to sensitive financial data and monitoring employee trading behaviors can help mitigate this risk.  

---

## **Example Scenario:**  

| **Name**                         | **Description**                                                                                      |
|----------------------------------|------------------------------------------------------------------------------------------------------|
| **Trading on Quarterly Earnings** | An employee with access to the company’s financial reports buys stock before earnings are publicly announced, expecting the stock price to rise. |
| **M&A Leak for Personal Gain**    | A corporate executive learns about a planned acquisition and purchases stock in the target company before the deal is publicly disclosed. |
| **Tipping Off a Third Party**     | An employee shares insider information with a friend or family member, who then trades on the stock to profit from nonpublic knowledge. |

---

## **Mitigations**  

1. Restrict access to material nonpublic information (MNPI) to only those employees with a legitimate business need.  
2. Implement data classification policies to mark financial and sensitive business data as **confidential** and enforce access controls.  
3. Require employees with access to sensitive financial data to acknowledge **insider trading policies** and periodically complete compliance training.  
4. Monitor for unauthorized access to financial reports, M&A documents, and regulatory filings.  
5. Establish **pre-clearance requirements** for employees in key roles to report planned stock trades for compliance review.  
6. Work with compliance and legal teams to implement monitoring of **unusual stock trades** by employees or close associates.  

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

| **Name**                           | **Description**                                                                 | **Link**          | **Risk Score** |
|------------------------------------|-------------------------------------------------------------------------------|-------------------|:--------------:|
| **Financial Data Access Alert**    | Flags unauthorized access to financial reports or M&A documents.               | [Example Link](#) | High           |
| **Unusual Trading Activity Alert** | Detects abnormal trading activity by employees with access to sensitive data.   | [Example Link](#) | High           |
| **MNPI File Transfer Alert**       | Monitors for large transfers of nonpublic financial information via email or storage devices. | [Example Link](#) | High           |
| **Tipping Off a Third Party Alert** | Correlates employee data access with stock trades by known associates.          | [Example Link](#) | Medium         |

---

### **Additional Considerations**  

1. **Why It’s Critical:**  
   - Insider trading can result in severe legal penalties, financial losses, and reputational damage for the company.  
   - Regulatory bodies, such as the **SEC (U.S.), FCA (UK), and ESMA (EU),** enforce strict rules against insider trading violations.  

2. **Broader Monitoring:**  
   - Combine financial data access monitoring with **behavior analytics** to detect employees engaging in **suspicious searches or file transfers.**  
   - Use **trade surveillance systems** to identify **suspicious stock trading patterns** by employees or their close contacts.  


