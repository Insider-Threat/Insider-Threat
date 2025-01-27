# **Destruction of Physical Device**

ID: IT1030

Tactic: Business Impact

Platform: Linux / Mac / Mobile / Windows

Permissions Required: Admin

Data Sources: Application / Authentication / Endpoint / Network / Tools / Email / Physical Security Logs / CCTV

Version: 1.1

Created: 04/28/2020

Last Modified: 01/27/2025

---

## **Overview:**

The intentional destruction of physical devices, such as servers, laptops, or storage media, can have catastrophic consequences for business operations. This type of insider threat can result in data loss, operational downtime, financial losses, and reputational harm. Monitoring physical security and implementing access controls can help mitigate such risks.

---

## **Example Scenario:**

| **Name**                              | **Description**                                                                                      |
|---------------------------------------|------------------------------------------------------------------------------------------------------|
| **Malicious Destruction of Servers**  | A disgruntled employee gains access to the server room and physically damages the hard drives of servers hosting critical applications, causing operational downtime. |
| **Backup System Sabotage**            | An insider intentionally destroys backup storage devices by smashing hard drives or disconnecting critical components to disrupt recovery efforts. |
| **Laptop Destruction Before Return**  | An employee about to resign physically damages their company-issued laptop, rendering it unusable, to conceal unauthorized activity or exfiltrated data. |
| **Tampering with Endpoint Devices**   | A user sabotages multiple workstations by physically damaging internal components, such as removing memory modules or damaging the motherboard, to cause widespread disruption. |

---

## **Mitigations**

1. Ensure regular and automated backups are performed to minimize the impact of physical device destruction.  
2. Implement strict physical access controls, including badge systems and biometric verification, for server rooms and critical infrastructure.  
3. Deploy physical security measures, such as CCTV, to monitor critical areas for unauthorized activity or tampering.  
4. Restrict administrative privileges on devices to prevent insiders from disabling recovery mechanisms, such as RAID configurations or backup systems.  
5. Establish clear processes for securing and auditing physical devices, particularly during termination or resignation periods.  

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
| Physical Access Alert          | Flags unauthorized access to server rooms or other critical infrastructure areas.               | [Example Link](#) | High           |
| Device Shutdown Alert          | Detects unexpected or forced shutdowns of critical devices.                                     | [Example Link](#) | Medium         |
| Hardware Tampering Alert       | Monitors for tampering signals from device logs, such as sudden disconnection or hardware failures. | [Example Link](#) | High           |
| CCTV Motion Alert              | Tracks unusual activity or unauthorized entry near physical infrastructure during off-hours.    | [Example Link](#) | Medium         |

