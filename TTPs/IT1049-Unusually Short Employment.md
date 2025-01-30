# **Unusually Short Employment**  

ID: IT1049  

Tactic: Initial Discovery  

Platform: Linux / Mac / Mobile / Windows  

Permissions Required: Standard  

Data Sources: HR Data / Endpoint Logs / Application Logs / Authentication Logs / Network Traffic  

Version: 1.1

Created: 07/07/2022  

Last Modified: 01/30/2025  

---

## **Overview:**  

Employees leaving an organization after a **short tenure** may not always be suspicious, but when paired with **unusual access patterns, data exfiltration, or unauthorized file downloads**, it may indicate **malicious intent.**  

This behavior could suggest:  
- **Corporate espionage** (an individual joins the company solely to gain access to sensitive data).  
- **Data theft for a competitor** (a new hire downloads confidential materials before resigning).  
- **Abuse of privileged access** (an employee exploits their position before quickly leaving).  

Organizations should monitor **new hires with early resignations**, especially if their **data access, file transfers, or external communications** are inconsistent with normal job responsibilities.  

---

## **Example Scenario:**  

| **Name**                         | **Description**                                                                                      |
|----------------------------------|------------------------------------------------------------------------------------------------------|
| **Employee "Grab and Run" Tactic** | A person **joins a company under false pretenses**, immediately accesses sensitive databases, downloads proprietary data, and resigns within weeks. |
| **Suspicious Early Resignation**  | A recently hired engineer **downloads internal design documents**, then unexpectedly resigns to join a competitor. |
| **Short-Term Contractor Data Theft** | A temporary contractor **copies source code** from the company repository before their contract ends. |

---

## **Mitigations**  

1. **Limit access for new hires** to critical systems and sensitive data until **trust and need-to-know permissions** are established.  
2. **Monitor for excessive data access and downloads** within the **first 90 days of employment**.  
3. **Conduct exit interviews** and **review access logs** for employees who resign unexpectedly.  
4. **Use behavior analytics (UBA/UEBA)** to identify **sudden spikes in data activity** by short-term employees.  
5. **Disable access immediately upon resignation notification** for roles with **high data sensitivity.**  

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

| **Name**                                   | **Description**                                                                 | **Link**          | **Risk Score** |
|-------------------------------------------|-------------------------------------------------------------------------------|-------------------|:--------------:|
| **Early Resignation Alert**               | Detects employees **resigning within a short timeframe (e.g., <90 days)**.     | [Example Link](#) | Medium         |
| **Unusual Data Access by New Hire**       | Flags **sudden spikes in file downloads, database queries, or sensitive document views**. | [Example Link](#) | High           |
| **Bulk File Transfer Before Resignation** | Identifies employees **moving large amounts of data to personal devices before leaving**. | [Example Link](#) | High           |
| **Job Role vs. Data Access Mismatch**     | Detects **new hires accessing data unrelated to their job function**.          | [Example Link](#) | Medium         |

---

### **Additional Considerations**  

1. **Why It’s Critical:**  
   - **Short-term employees accessing high-value information** may indicate **corporate espionage, insider threats, or IP theft**.  
   - Monitoring early departures can **help prevent data breaches and ensure better hiring risk assessment.**  

2. **Broader Monitoring:**  
   - **Integrate HR and IT logs** to **correlate new hire data access with employment duration trends**.  
   - **Use endpoint security tools** to detect **unusual file downloads, printing, or external transfers before resignation.**  

---

