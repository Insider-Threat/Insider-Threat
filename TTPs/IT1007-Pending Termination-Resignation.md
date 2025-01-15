# **Pending Termination/Resignation**

ID: IT1007

Tactic: Initial Discovery

Platform: Linux / Mac / Mobile / Windows

Permissions Required: Standard

Data Sources: HR Data / Application / Authentication / Endpoint / Network / Sensitive Information Storage Locations / Tools

Version: 1.0

Created: 04/28/2020

Last Modified: 01/15/2025

---

## **Overview:**

Identifying and investigating anomalous activity before an employee departs the company is critical to preventing the loss of sensitive or valuable data. Behavioral deviations, such as accessing unauthorized systems or downloading large volumes of files, may indicate malicious intent or preparations to exfiltrate data. Early detection helps mitigate risks during the notice period and ensures the security of company assets.

---

## **Example Scenario:**

| **Name**                | **Description**                                                                                      |
|-------------------------|------------------------------------------------------------------------------------------------------|
| Employee Resignation    | An employee resigns and, during their notice period, attempts to access applications they’ve never used before and downloads a large volume of files from file shares. |
| Pending Termination     | An employee learns they are being terminated and attempts to copy sensitive files to a USB drive or upload them to personal cloud storage. |

---

## **Mitigations**

1. Revoke access to sensitive applications, systems, and files immediately upon notice of resignation or termination.  
2. Implement enhanced monitoring during the notice period, focusing on unusual file downloads, data transfers, and system access.  
3. Use DLP tools to block unauthorized data transfers to external devices or cloud services.  
4. Require departing employees to return all company assets and sign a data protection acknowledgment.  
5. Establish a policy for HR and IT collaboration to track resignations and terminations in real time.  

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
| Anomalous Access Alert   | Detects attempts to access applications or systems not previously accessed by the employee.      | [Example Link](#) | High           |
| Data Download Alert      | Flags large-scale file downloads or unusual activity on file shares.                            | [Example Link](#) | High           |
| USB Activity Alert       | Monitors for data transfers to unauthorized USB devices.                                        | [Example Link](#) | Medium         |
| Cloud Upload Alert       | Detects uploads of sensitive files to personal or external cloud storage services.              | [Example Link](#) | High           |
| Privileged Access Alert  | Tracks attempts to elevate privileges or access restricted systems during the notice period.    | [Example Link](#) | Medium         |
