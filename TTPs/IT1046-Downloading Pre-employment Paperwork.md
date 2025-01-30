# **Downloading Pre-Employment Paperwork**  

ID: IT1046  

Tactic: Initial Discovery  

Platform: Linux / Mac / Mobile / Windows  

Permissions Required: Standard  

Data Sources: Endpoint Logs / DLP Events / Network Traffic / Email Attachments  

Version: 1.1  

Created: 06/23/2022  

Last Modified: 01/30/2025  

---

## **Overview:**  

Employees who **download, store, or access pre-employment paperwork** on company devices may be actively pursuing new job opportunities or planning to leave the company. This activity could indicate **potential attrition risks**, insider threats, or even **conflicts of interest** if an employee is attempting to work for multiple companies simultaneously.  

Pre-employment paperwork can include:  
- **Offer letters**  
- **Background screening forms**  
- **New hire welcome guides**  
- **Employment contracts**  

Monitoring for **sudden interest in job-related documents** alongside **other risk indicators (e.g., unusual file transfers, external job site visits, large data downloads)** can help identify potential security risks before they escalate.  

---

## **Example Scenario:**  

| **Name**                                  | **Description**                                                                                      |
|------------------------------------------|------------------------------------------------------------------------------------------------------|
| **Employee Preparing to Resign**         | An employee downloads their **offer letter and onboarding paperwork** onto their company laptop, signaling an upcoming resignation. |
| **Working Multiple Jobs Simultaneously** | A remote employee **downloads background check forms** for a second job while still working for their current employer. |
| **Job Application-Related Document Creation** | A user creates a **resume, cover letter, or employment history document** on their company device. |

---

## **Mitigations**  

1. **Monitor for downloads of known pre-employment file types** (e.g., PDFs, DOCX, or ZIP files with job-related keywords).  
2. **Use Data Loss Prevention (DLP) tools** to detect and block the transfer of **employment-related documents to personal devices or email accounts**.  
3. **Track document metadata and naming conventions** to identify files like *offer_letter.pdf* or *employment_contract.docx*.  
4. **Combine this detection with job site browsing alerts** to correlate potential attrition risks.  
5. **Conduct behavioral analysis** to determine if the employee is exhibiting other signs of potential data exfiltration.  

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
| **Pre-Employment Document Download Alert** | Detects the download or storage of **job-related documents** on a company device. | [Example Link](#) | Medium         |
| **Email Attachment with Job-Related Content** | Flags emails containing **offer letters, contracts, or background check documents**. | [Example Link](#) | Medium         |
| **Job Site Browsing & Document Download Correlation** | Identifies users who **frequently visit job boards and download employment-related files**. | [Example Link](#) | High           |

---

### **Additional Considerations**  

1. **Why It’s Critical:**  
   - Tracking **pre-employment paperwork downloads** helps identify employees at risk of leaving, which can correlate with **data exfiltration risks**.  
   - Some employees may be **moonlighting or working multiple jobs** against company policy, creating potential conflicts of interest.  

2. **Broader Monitoring:**  
   - **Combine endpoint monitoring with network traffic analysis** to detect file transfers to personal storage.  
   - **Use behavior analytics (UBA/UEBA) tools** to track anomalies in employee activity before resignation.  

---


