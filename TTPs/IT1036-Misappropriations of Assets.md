# **Misappropriations of Assets**

ID: IT1036

Tactic: Business Impact

Platform: Linux / Mac / Mobile / Windows

Permissions Required: Admin

Data Sources: Application / Authentication / Endpoint / Network / Tools / Email / Asset Management Systems

Version: 1.1

Created: 04/28/2020

Last Modified: 01/27/2025

---

## **Overview:**

Employees and contractors are entrusted with access to company assets, such as laptops, servers, applications, and cloud services, to perform their job functions. Misappropriation occurs when these resources are used without authorization for personal gain, such as installing unauthorized software, leveraging assets for external work, or exploiting company resources for non-business purposes. These actions can degrade system performance, disrupt business operations, and incur financial or reputational damage.

---

## **Example Scenario:**

| **Name**                          | **Description**                                                                                      |
|-----------------------------------|------------------------------------------------------------------------------------------------------|
| **Cryptocurrency Mining**         | An employee installs a cryptocurrency miner on company servers, significantly increasing resource usage and rendering the servers less available for business-critical applications. |
| **Personal Use of Cloud Services** | A user leverages company cloud resources, such as storage or compute instances, to host personal projects, incurring additional costs for the company. |
| **Unauthorized Hardware Use**     | A contractor borrows high-value equipment, such as laptops or networking gear, for personal use or external projects, without company approval. |
| **Software Piracy Using Assets**  | An employee uses company devices to download or distribute pirated software, exposing the company to legal and compliance risks. |

---

## **Mitigations**

1. Implement role-based access controls (RBAC) to ensure users only have access to the assets and systems required for their job responsibilities.  
2. Use endpoint protection and monitoring tools to detect and block unauthorized software installations or excessive resource usage.  
3. Conduct regular audits of asset usage, including cloud services, to identify anomalies or personal use.  
4. Maintain an asset management system to track the assignment and usage of physical and digital assets.  
5. Provide training to employees and contractors on acceptable use policies for company resources, emphasizing consequences for violations.  

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
| Resource Abuse Alert           | Flags excessive CPU, memory, or network utilization on company servers caused by unauthorized processes like cryptocurrency mining. | [Example Link](#) | High           |
| Unauthorized Software Installation Alert | Detects attempts to install or execute unauthorized applications on company devices.           | [Example Link](#) | High           |
| Cloud Resource Misuse Alert    | Monitors for unusual usage patterns in cloud environments, such as the creation of unapproved resources. | [Example Link](#) | Medium         |
| Asset Misuse Alert             | Flags unauthorized or prolonged usage of company hardware, such as borrowing devices for personal use. | [Example Link](#) | Medium         |
