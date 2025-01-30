# **Use of File Share Site with External User**  

ID: IT1040  

Tactic: Exfiltration  

Platform: Linux / Mac / Mobile / Windows  

Permissions Required: Admin  

Data Sources: Application / Authentication / Endpoint / Network / Tools / Email  

Version: 1.1 

Created: 04/28/2020  

Last Modified: 01/30/2025  

---

## **Overview:**  

Many companies use **cloud-based file-sharing services** like **Microsoft SharePoint, Google Drive, Dropbox, or Box** to collaborate on documents and store data. While these platforms enhance productivity, they can also be exploited by insiders attempting to **exfiltrate sensitive data**. A **malicious insider** might add an **external email account** or create **public file-sharing links** to access and transfer company data undetected.  

Even unintentional **misconfigurations**—such as accidentally allowing external access to sensitive files—can result in **data leaks** and compliance violations.  

---

## **Example Scenario:**  

| **Name**                          | **Description**                                                                                      |
|-----------------------------------|------------------------------------------------------------------------------------------------------|
| **Data Sharing Before Resignation** | An employee planning to leave the company **adds their personal email account** to the company's file-sharing platform, allowing them to download confidential data as an external user without triggering internal alerts. |
| **Unauthorized Third-Party Access** | An employee shares a **file containing trade secrets** with a former colleague at a competitor by creating a **public link** on the company’s cloud storage system. |
| **Accidental External Sharing**    | A user **mistakenly configures** a sensitive folder on **Google Drive** to be **accessible to anyone with the link**, exposing internal data to the public. |
| **Collusion with External Actors** | An insider **adds an external email account belonging to a threat actor** to a restricted folder, enabling external data exfiltration without detection. |

---

## **Mitigations**  

1. **Monitor file-sharing activity**, especially the addition of external users to company file repositories.  
2. **Enforce role-based access controls (RBAC)** to restrict sharing of confidential/sensitive data.  
3. **Prevent public link creation** for internal-only repositories, ensuring only authorized personnel can share files externally.  
4. **Implement Data Loss Prevention (DLP)** solutions to detect and block unauthorized file-sharing attempts.  
5. **Enable logging and alerts** for external file-sharing activities, flagging large data transfers or access by non-corporate email domains.  
6. **Require security awareness training** for employees on the risks of misconfigured file-sharing settings.  

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
| **External File Sharing Alert**        | Detects when a user shares a file or folder with an **external email address**. | [Example Link](#) | High           |
| **Public Link Creation Alert**         | Flags the creation of **publicly accessible** file-sharing links on corporate storage platforms. | [Example Link](#) | High           |
| **Bulk File Download Alert**           | Monitors for **large data transfers** before an employee resignation.          | [Example Link](#) | High           |
| **Unusual Sharing Pattern Alert**      | Identifies **sudden spikes** in external sharing activity from a specific user. | [Example Link](#) | Medium         |

---

### **Additional Considerations**  

1. **Why It’s Critical:**  
   - **Unauthorized file sharing** can lead to **data breaches, regulatory violations (GDPR, CCPA, PCI-DSS), and competitive disadvantages** if intellectual property is leaked.  
   - Many **insider threats use external file-sharing as an exfiltration method** because it’s easy to evade detection if not properly monitored.  

2. **Broader Monitoring:**  
   - **Integrate file-sharing logs with SIEM tools** to correlate sharing events with other suspicious activities (e.g., increased access to sensitive documents).  
   - **Use behavioral analytics** to detect **anomalous sharing activity**, such as an employee suddenly sharing large amounts of data externally before resignation.  

---
