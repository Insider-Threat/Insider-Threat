# **AirDrop to a Device**

ID: IT1027

Tactic: Exfiltration

Platform: Linux / Mac / Mobile / Windows

Permissions Required: Admin

Data Sources: Application / Authentication / Endpoint / Network / Tools / Email

Version: 1.1

Created: 04/28/2020

Last Modified: 01/27/2025

---

## **Overview:**

Apple AirDrop enables users to transfer files wirelessly to nearby devices. While convenient, this method bypasses many traditional monitoring tools, making it an attractive option for data exfiltration. By leveraging AirDrop, individuals can avoid detection while transferring sensitive information to personal or unapproved devices. Monitoring and restricting this functionality is essential to mitigate insider threats.

---

## **Example Scenario:**

| **Name**                                | **Description**                                                                                      |
|-----------------------------------------|------------------------------------------------------------------------------------------------------|
| **Data Exfiltration to Personal Device** | An employee planning to resign gathers sensitive data on their corporate laptop, including customer information and proprietary designs. They use AirDrop to transfer the files to their personal phone, bypassing traditional network monitoring tools. |
| **Unauthorized Peer-to-Peer Transfer**  | A contractor with limited network access uses AirDrop to transfer sensitive diagrams to another employee's personal device, avoiding email and file-sharing restrictions. |
| **Stealth Transfer During Internal Meeting** | During a confidential meeting, an insider uses AirDrop to transfer meeting notes and intellectual property to a personal iPad without connecting to the corporate network. |

---

## **Mitigations**

1. Disable AirDrop functionality on corporate devices unless explicitly required for business purposes.  
2. Implement mobile device management (MDM) solutions to restrict the use of AirDrop on managed devices.  
3. Enforce strict data transfer policies that prohibit unauthorized use of peer-to-peer file sharing tools like AirDrop.  
4. Educate employees on acceptable use policies and the risks of unauthorized file transfers.  
5. Use endpoint protection tools to monitor file access and flag suspicious activity, such as bulk file transfers.  

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
| Bulk File Transfer Alert       | Detects significant file transfers occurring on devices configured with AirDrop enabled.         | [Example Link](#) | High           |
| Peer-to-Peer Transfer Alert    | Monitors for peer-to-peer file sharing activities using AirDrop or similar tools.                | [Example Link](#) | Medium         |
| Behavioral Anomaly Alert       | Flags deviations in file access or transfer behavior, such as large-scale file activity.         | [Example Link](#) | Medium         |


