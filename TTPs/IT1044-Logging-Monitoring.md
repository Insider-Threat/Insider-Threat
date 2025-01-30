# **Logging and Monitoring**  

ID: IT1044  

Tactic: Proactive Measures  

Platform: Linux / Mac / Mobile / Windows  

Permissions Required: Standard  

Data Sources: Application / Authentication / Endpoint / Network / Tools / Email / Cloud Logs / SIEM  

Version: 1.1  

Created: 04/28/2020  

Last Modified: 01/30/2025  

---

## **Overview:**  

Effective **logging and monitoring** are **critical components** of a strong security posture. Properly configured logs allow organizations to **detect suspicious activity, investigate security incidents, and proactively respond to threats.**  

By **collecting, analyzing, and correlating logs** across multiple systems—including **authentication events, file access, network activity, and privileged actions**—security teams can **quickly identify and mitigate potential insider threats.**  

Without comprehensive logging, organizations **lack visibility** into user actions, increasing the risk of **data breaches, privilege abuse, and system compromise.**  

---

## **Example Scenario:**  

| **Name**                           | **Description**                                                                                      |
|------------------------------------|------------------------------------------------------------------------------------------------------|
| **Unusual Login Activity**         | An employee logs in from an unfamiliar location outside normal working hours, suggesting compromised credentials or insider activity. |
| **Privilege Escalation Attempt**   | A standard user account attempts to elevate privileges or access admin-only areas without authorization. |
| **Mass File Deletion or Transfer** | A user unexpectedly deletes large amounts of data or moves sensitive files to an external location, triggering a data exfiltration alert. |
| **Disabled or Altered Logging**    | An administrator disables security logs on a server to cover up unauthorized changes. |

---

## **Mitigations**  

1. **Enable centralized logging** using a **Security Information and Event Management (SIEM) system** to collect logs from applications, endpoints, and network devices.  
2. **Monitor authentication and access logs** for anomalies, such as multiple failed login attempts or access to restricted files.  
3. **Implement real-time alerts** for **suspicious behavior**, such as mass data transfers, privilege escalation, or unusual login locations.  
4. **Regularly audit and review logs** to ensure completeness, accuracy, and proper retention policies.  
5. **Restrict log modification privileges** to prevent insiders from tampering with records.  
6. **Use behavior analytics (UBA/UEBA)** to detect deviations from normal user activity.  

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

| **Name**                              | **Description**                                                                | **Link**          | **Risk Score** |
|---------------------------------------|--------------------------------------------------------------------------------|-------------------|:--------------:|
| **Unusual Login Alert**               | Detects logins from unusual locations or at abnormal times.                     | [Example Link](#) | High           |
| **Privilege Escalation Attempt Alert** | Flags unauthorized attempts to elevate privileges.                              | [Example Link](#) | High           |
| **Mass File Deletion Alert**          | Identifies sudden, large-scale data deletion events.                            | [Example Link](#) | High           |
| **Disabled Logging Alert**            | Detects attempts to turn off logging or alter log retention settings.           | [Example Link](#) | Critical       |

---

### **Additional Considerations**  

1. **Why It’s Critical:**  
   - Without proper logging, organizations **lack the forensic data** necessary to investigate security incidents.  
   - Monitoring **real-time alerts** enables **faster incident response and threat mitigation**.  

2. **Broader Monitoring:**  
   - **Integrate SIEM tools with behavioral analytics** to detect anomalies in user behavior.  
   - Establish **log retention policies** that comply with **regulatory requirements (e.g., GDPR, HIPAA, PCI-DSS, SOX).**  

---
