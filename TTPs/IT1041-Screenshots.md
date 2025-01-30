# **Screenshots**  

ID: IT1041  

Tactic: Collection  

Platform: Linux / Mac / Mobile / Windows  

Permissions Required: Admin  

Data Sources: Application / Authentication / Endpoint / Network / Tools / Email  

Version: 1.1  

Created: 04/28/2020  

Last Modified: 01/30/2025  

---

## **Overview:**  

Most devices have built-in screenshot capabilities, and many third-party applications provide similar functionality. **Malicious insiders** may exploit screenshots to **steal sensitive information** while avoiding security controls that monitor file downloads, printing, or copying to external devices.  
By capturing screenshots, users can **bypass Data Loss Prevention (DLP) policies, encryption protections, and logging mechanisms**, making it difficult to detect exfiltration attempts.  

Screenshots are often used to capture **financial data, trade secrets, customer records, or privileged communications** without triggering security alerts. **Monitoring for suspicious screenshot activity** and implementing security controls can help mitigate this risk.  

---

## **Example Scenario:**  

| **Name**                                  | **Description**                                                                                      |
|------------------------------------------|------------------------------------------------------------------------------------------------------|
| **Screenshots of Sensitive Data**         | An employee circumvents security controls by taking screenshots of confidential customer data instead of downloading the files. |
| **Capturing Privileged Communications**   | A user takes screenshots of **executive emails** discussing an upcoming merger and leaks them externally. |
| **Using OCR to Extract Text from Images** | A malicious insider screenshots **PII from an internal HR portal** and uses Optical Character Recognition (OCR) to extract the text. |
| **Screenshots of Financial Dashboards**   | A finance employee takes screenshots of a **pre-release earnings report** and shares it with an unauthorized party. |

---

## **Mitigations**  

1. **Implement endpoint monitoring** to detect and log screenshot activities from built-in or third-party tools.  
2. **Restrict screenshot capabilities** in virtual desktop environments (VDI), remote desktop sessions, and sensitive applications.  
3. **Watermark sensitive data** to trace leaks back to the source in case of unauthorized screenshots.  
4. **Use anti-screen capture technology** in critical applications to prevent screenshots from being taken.  
5. **Enforce role-based access controls (RBAC)** to limit who can view sensitive data, reducing the risk of unauthorized screenshots.  
6. **Educate employees** on security risks and enforce policies against unauthorized screenshot capture of confidential information.  

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
| **Screenshot Capture Alert**       | Detects the use of screenshot tools in restricted applications or environments. | [Example Link](#) | High           |
| **OCR-Based Data Leak Alert**      | Flags attempts to extract sensitive text from images captured via screenshots. | [Example Link](#) | High           |
| **Suspicious Screen Capture Process** | Identifies unusual or unauthorized screenshot applications running on endpoints. | [Example Link](#) | Medium         |

---

### **Additional Considerations**  

1. **Why It’s Critical:**  
   - Screenshot-based exfiltration can **bypass traditional security controls** and allow unauthorized users to capture confidential information.  
   - Sensitive **financial, HR, legal, and trade secret information** can be stolen and leaked without leaving a clear forensic trail.  

2. **Broader Monitoring:**  
   - **Integrate endpoint monitoring with SIEM tools** to detect correlations between **data access and screenshot activities.**  
   - Use **AI-powered DLP solutions** to detect sensitive data in screenshots and alert security teams to possible insider threats.  

---

