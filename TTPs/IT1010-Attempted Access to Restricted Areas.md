# **Attempted Access to Restricted Areas**

ID: IT1010

Tactic: Initial Discovery

Platform: Linux / Mac / Mobile / Windows

Permissions Required: Standard

Data Sources: Badge System / CCTV

Version: 1.1

Created: 04/28/2020

Last Modified: 01/15/2025

---

## **Overview:**

Access to restricted areas is based on job requirements, and employees should not attempt to access secure locations unless authorized. Unauthorized access attempts could indicate malicious intent, such as spying on confidential meetings, stealing sensitive documents, or tampering with critical systems. Monitoring physical access logs and using video surveillance helps detect and prevent unauthorized entry into restricted areas.

---

## **Example Scenario:**

| **Name**                          | **Description**                                                                                      |
|-----------------------------------|------------------------------------------------------------------------------------------------------|
| Unauthorized Access to Secure Area | An employee repeatedly attempts to enter a restricted area where a confidential meeting is taking place but does not have access. After multiple failed badge attempts, they follow a group of authorized employees into the area (tailgating). |
| Access Attempt to Data Center      | An employee without proper authorization tries to enter a data center by using a coworker’s badge or seeking assistance from security personnel. |
| Tailgating                 | An employee follows behind an authorized individual entering a restricted area without scanning their badge. CCTV footage confirms the unauthorized entry. |

---

## **Mitigations**

1. Monitor badge logs for access denial events and investigate repeated attempts to restricted areas.  
2. Use video surveillance systems to monitor entry points to sensitive areas.  
3. Implement anti-tailgating measures, such as turnstiles or mantraps, to prevent unauthorized entry.  
4. Provide regular training to employees about the importance of not allowing others to tailgate into secure areas.  
5. Conduct regular audits of physical access permissions to ensure only authorized personnel can access restricted areas.

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

| **Name**                | **Description**                                                                                 | **Link**          | **Risk Score** |
|-------------------------|-------------------------------------------------------------------------------------------------|-------------------|:--------------:|
| Badge Denial Alert       | Detects repeated access denial events for restricted areas.                                     | [Example Link](#) | Medium         |
| Tailgating Detection Alert | Uses CCTV and access logs to identify potential tailgating incidents.                         | [Example Link](#) | High           |
| Unauthorized Badge Use Alert | Flags badge use outside normal employee hours or in locations unrelated to their job duties. | [Example Link](#) | High           |
| Access Request Escalation Alert | Monitors for unusual requests to escalate access permissions to restricted areas.          | [Example Link](#) | Medium         |
