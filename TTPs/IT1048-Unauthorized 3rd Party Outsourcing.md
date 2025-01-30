# **Unauthorized 3rd Party Outsourcing**  

ID: IT1048  

Tactic: Business Impact  

Platform: Linux / Mac / Mobile / Windows  

Permissions Required: Standard  

Data Sources: Badge Reader Logs / CCTV Logs / Endpoint Logs / Application Logs / Authentication Logs / Network Traffic Logs  

Version: 1.1

Created: 06/23/2022  

Last Modified: 01/30/2025  

---

## **Overview:**  

In **remote and hybrid work environments**, direct oversight of employee activities is limited. Some employees may **outsource their assigned work to unauthorized third parties** to reduce their workload, increase productivity deceptively, or even **engage in fraudulent activity.**  

This practice introduces **unvetted individuals** into the organization’s ecosystem, increasing the risk of:  
- **Data breaches** (sharing credentials with unauthorized users).  
- **Regulatory violations** (sensitive data accessed by unapproved personnel).  
- **Intellectual property theft** (outsiders gaining access to proprietary information).  

Monitoring for **suspicious remote access activity** and enforcing strong authentication measures can help detect and prevent unauthorized outsourcing.  

---

## **Example Scenario:**  

| **Name**                                  | **Description**                                                                                      |
|------------------------------------------|------------------------------------------------------------------------------------------------------|
| **Employee Personally Outsourcing Work** | A software engineer is assigned a high-priority project but **hires an unapproved freelancer** to complete the work. They **provide VPN credentials** so the freelancer can log in remotely. |
| **Unusual Work Patterns & Access Locations** | An employee’s work is **suddenly completed at unusual hours or from different locations**, indicating someone else is logging in under their credentials. |
| **Offshore Data Handling Risks** | An employee with access to **sensitive customer information** outsources tasks to a **foreign contractor**, violating **compliance regulations (e.g., GDPR, HIPAA, PCI-DSS).** |

---

## **Mitigations**  

1. **Monitor for anomalous authentication activity**, such as logins from **unusual locations or IP addresses**.  
2. **Use multi-factor authentication (MFA)** to prevent unauthorized access by third parties.  
3. **Track VPN usage logs** to detect if credentials are being used from **multiple locations in short timeframes**.  
4. **Restrict data access based on need-to-know principles**, ensuring that sensitive information is not easily transferable.  
5. **Educate employees on the security risks and policy violations** associated with unauthorized outsourcing.  
6. **Audit work outputs and behavioral patterns**, especially for remote employees with access to critical systems.  

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

| **Name**                               | **Description**                                                                 | **Link**          | **Risk Score** |
|----------------------------------------|-------------------------------------------------------------------------------|-------------------|:--------------:|
| **Unusual Login Locations Alert**      | Detects **logins from unexpected countries or locations** inconsistent with normal behavior. | [Example Link](#) | High           |
| **Multiple VPN Sessions Alert**        | Flags instances where an employee’s **VPN credentials are used from multiple locations simultaneously**. | [Example Link](#) | High           |
| **Unusual Work Hours Alert**           | Identifies employees whose **activity spikes at unusual hours**, suggesting unauthorized outsourcing. | [Example Link](#) | Medium         |
| **Sensitive Data Access from New IPs** | Detects attempts to **access confidential files from IP addresses never used by the employee before**. | [Example Link](#) | High           |

---

### **Additional Considerations**  

1. **Why It’s Critical:**  
   - Unauthorized outsourcing can **expose sensitive company data** to external parties, violating **data protection laws and security policies**.  
   - **Employees sharing credentials with third parties** can lead to **data breaches, compliance violations, and intellectual property theft.**  

2. **Broader Monitoring:**  
   - **Integrate authentication logs with behavior analytics** to detect sudden changes in **work habits, login patterns, and productivity anomalies.**  
   - **Use session monitoring and keystroke analytics** in critical environments to identify **possible unauthorized use of corporate credentials.**  

---

