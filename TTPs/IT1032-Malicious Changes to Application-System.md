# **Malicious Changes to Application/System**

ID: IT1032

Tactic: Business Impact

Platform: Linux / Mac / Mobile / Windows

Permissions Required: Admin

Data Sources: Application / Authentication / Endpoint / Network / Tools / Email

Version: 1.1

Created: 04/28/2020

Last Modified: 01/27/2025

---

## **Overview:**

Users with elevated privileges can intentionally or accidentally make changes to critical applications or systems that result in outages, degraded performance, or data loss. These changes may include modifications to configurations, disabling security controls, or deleting essential components. Monitoring administrative activity and enforcing role-based access controls can reduce the risk of malicious or unintended disruptions.

---

## **Example Scenario:**

| **Name**                              | **Description**                                                                                      |
|---------------------------------------|------------------------------------------------------------------------------------------------------|
| **Malicious Application Changes**     | A disgruntled employee modifies a configuration in a critical application, rendering it inoperable and disrupting business operations. |
| **Disabling Security Settings**       | An insider disables logging or intrusion detection settings on a critical system, allowing unauthorized activity to go undetected. |
| **Unauthorized System Reconfiguration** | A user makes unauthorized changes to system settings, such as altering network routes or firewall rules, leading to outages or security vulnerabilities. |

---

## **Mitigations**

1. Enforce strict role-based access controls (RBAC) to limit administrative access to critical systems and applications.  
2. Require multi-factor authentication (MFA) for all administrative tasks, including system and application changes.  
3. Implement change management processes, requiring approvals and documentation for modifications to applications or systems.  
4. Regularly audit configuration changes and administrative activities for anomalies or unauthorized actions.  
5. Use monitoring tools to track changes to critical systems in real time and alert on deviations from approved configurations.  

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

| **Name**                       | **Description**                                                                                 | **Link**          | **Risk Score** |
|--------------------------------|-------------------------------------------------------------------------------------------------|-------------------|:--------------:|
| Configuration Change Alert     | Detects changes to critical application or system configurations outside approved processes.     | [Example Link](#) | High           |
| Security Settings Modification Alert | Flags changes to security settings, such as disabling logging, intrusion detection, or backups. | [Example Link](#) | High           |
| Behavioral Anomaly Alert       | Identifies unusual administrative activity, such as frequent or unexplained modifications to key systems. | [Example Link](#) | Medium         |
| Application Downtime Alert     | Monitors critical applications for unexpected downtime caused by configuration changes.          | [Example Link](#) | High           |


