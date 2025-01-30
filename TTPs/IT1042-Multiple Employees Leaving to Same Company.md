# **Multiple Employees Leaving to Same Company**  

ID: IT1015  

Tactic: Initial Discovery  

Platform: Linux / Mac / Mobile / Windows  

Permissions Required: Standard  

Data Sources: Application / Authentication / Endpoint / Network / Tools / Email / HR Data  

Version: 1.1 

Created: 04/28/2020  

Last Modified: 01/30/2025  

---

## **Overview:**  

When multiple employees **resign and join the same company within a short timeframe**, it may indicate **coordinated employee movement**, potentially involving **intellectual property theft, trade secret exfiltration, or collusion.**  
These employees may attempt to **recruit others** with access to proprietary data or **leverage internal knowledge** to give their new employer a competitive advantage.  

Organizations must monitor for **anomalous data access, unusual downloads, and unauthorized external communications** from employees planning to leave. **Collaboration between HR and InfoSec** is critical in detecting and preventing corporate data theft in these scenarios.  

---

## **Example Scenario:**  

| **Name**                                      | **Description**                                                                                      |
|----------------------------------------------|------------------------------------------------------------------------------------------------------|
| **Coordinated Employee Departures**          | Over a short period, **several employees from the same team resign** and join a competitor. One of them starts reaching out to current employees to encourage them to bring sensitive data. |
| **Mass Resignation After Takeover Talks**    | A company begins acquisition discussions, and a group of employees **quits to form a competing startup**, potentially using insider knowledge to gain an unfair market advantage. |
| **Recruitment of Key Employees**             | A former employee actively **contacts their ex-colleagues**, encouraging them to share trade secrets or move to the competitor. |

---

## **Mitigations**  

1. **Monitor bulk employee resignations** for patterns indicating potential data exfiltration or coordinated movement.  
2. **Review access logs** of departing employees to identify any unusual file downloads, email forwarding, or external storage usage.  
3. **Disable access to sensitive systems** for employees immediately upon resignation notice, especially those in high-risk roles.  
4. **Enforce Non-Disclosure Agreements (NDAs)** and include clauses restricting solicitation of former colleagues.  
5. **Conduct exit interviews** to assess employee sentiment and look for signs of coordinated departures.  
6. **Educate employees on legal consequences** of intellectual property theft and misappropriation of corporate data.  

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
| **Mass Resignation Alert**          | Detects a sudden increase in employee resignations from the same department or team. | [Example Link](#) | Medium         |
| **Unusual Data Access Before Departure** | Flags employees downloading large volumes of sensitive files before resigning. | [Example Link](#) | High           |
| **External Communication with Competitor** | Monitors for email exchanges between employees and known competitor domains.  | [Example Link](#) | High           |
| **Recruitment Pattern Detection**   | Identifies former employees reaching out to current staff via company email or messaging platforms. | [Example Link](#) | Medium         |

---

### **Additional Considerations**  

1. **Why It’s Critical:**  
   - **Coordinated employee departures** can lead to **trade secret theft, customer loss, and competitive disadvantages.**  
   - **Intellectual property theft** can result in **legal battles, financial losses, and regulatory penalties.**  

2. **Broader Monitoring:**  
   - **Integrate HR and security systems** to detect **trends in resignations linked to specific competitors.**  
   - Use **SIEM and behavior analytics** to identify **anomalous activity from employees planning to leave.**  

---


