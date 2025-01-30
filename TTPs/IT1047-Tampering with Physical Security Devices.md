# **Tampering with Physical Security Devices**  

ID: IT1047  

Tactic: Business Impact  

Platform: Linux / Mac / Mobile / Windows  

Permissions Required: Standard  

Data Sources: Badge Reader Logs / CCTV Logs / Security Alarm Logs / IoT Device Logs  

Version: 1.1

Created: 06/23/2022  

Last Modified: 01/30/2025  

---

## **Overview:**  

Physical security devices—including **badge readers, security cameras, motion detectors, and alarm systems**—are essential for protecting **restricted areas, critical infrastructure, and sensitive data storage locations.**  

A **malicious insider** may attempt to **disable, manipulate, or bypass** these security systems to **conceal unauthorized access, theft, or sabotage.**  

Such activity can indicate **insider threat behavior**, such as preparing for **data exfiltration, hardware theft, or corporate espionage.**  

---

## **Example Scenario:**  

| **Name**                           | **Description**                                                                                      |
|------------------------------------|------------------------------------------------------------------------------------------------------|
| **Covering or Disabling a Security Camera** | An employee **blocks, disconnects, or disables a CCTV camera** covering a restricted area before accessing sensitive systems. |
| **Tampering with Badge Readers**   | A user **modifies a badge reader** to bypass authentication logs, allowing unauthorized access to secured locations. |
| **Bypassing Door Sensors or Alarms** | A departing employee **uses an object to hold open a secured door**, preventing it from locking properly. |
| **Unusual Badge Swipes**           | A user **swipes multiple access cards** or uses a stolen badge to attempt access to a restricted area. |

---

## **Mitigations**  

1. **Monitor badge reader access logs** for anomalies such as **repeated failed access attempts or badge cloning.**  
2. **Use AI-powered video analytics** to detect security camera tampering, obstruction, or disabling attempts.  
3. **Enable tamper alerts** on **badge readers, security cameras, and alarm systems** to notify security teams in real-time.  
4. **Implement access control monitoring** to detect **tailgating, unusual after-hours access, or forced entry attempts.**  
5. **Conduct regular security device audits** to ensure all **cameras, sensors, and badge readers are functioning properly.**  
6. **Educate employees on security policies** and the **consequences of tampering with physical security devices.**  

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
| **Camera Tampering Alert**            | Detects when a security camera is **disabled, obstructed, or disconnected**.    | [Example Link](#) | High           |
| **Unusual Badge Reader Activity**     | Flags **multiple failed badge swipes** or **attempts to use a stolen badge.**   | [Example Link](#) | High           |
| **After-Hours Access Attempt**        | Identifies badge access attempts **outside of normal work hours.**              | [Example Link](#) | Medium         |
| **Forced Entry Alert**                 | Detects attempts to **hold open secured doors or bypass motion sensors.**       | [Example Link](#) | Critical       |

---

### **Additional Considerations**  

1. **Why It’s Critical:**  
   - **Tampering with security devices** can indicate **preparation for data theft, sabotage, or unauthorized access.**  
   - Detecting **early signs of physical security bypassing** helps prevent **security breaches, intellectual property theft, and financial loss.**  

2. **Broader Monitoring:**  
   - **Integrate physical security logs with SIEM tools** to correlate **badge access events with network or data access anomalies.**  
   - Use **machine learning-based anomaly detection** to flag **unusual security device behavior.**  

---


