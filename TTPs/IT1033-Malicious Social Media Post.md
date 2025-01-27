# **Malicious Social Media Post**

ID: IT1033

Tactic: Business Impact

Platform: Linux / Mac / Mobile / Windows

Permissions Required: Admin

Data Sources: Application / Authentication / Endpoint / Network / Tools / Email / Social Media Monitoring Tools

Version: 1.1

Created: 04/28/2020

Last Modified: 01/27/2025

---

## **Overview:**

Social media platforms allow users to rapidly share information with a vast audience. Insiders with access to sensitive or proprietary information can exploit these platforms to disclose data without authorization, potentially violating regulatory requirements and damaging the company's reputation. Additionally, disgruntled employees may post false information to tarnish the company’s image or undermine trust with customers and partners. Monitoring social media for mentions of the company and its products is vital to detect and mitigate these risks.

---

## **Example Scenario:**

| **Name**                              | **Description**                                                                                      |
|---------------------------------------|------------------------------------------------------------------------------------------------------|
| **Unauthorized Data Disclosure**      | A disgruntled employee posts confidential financial results on a public social media platform before the company’s official disclosure, violating compliance regulations. |
| **Reputational Damage via False Claims** | An insider posts false claims about unsafe practices or faulty products to damage the company’s reputation and stock value. |
| **Leaking Trade Secrets**             | A user shares proprietary designs, code snippets, or other intellectual property on social media or public forums for personal gain or retaliation. |
| **Spreading Internal Disputes Publicly** | An employee shares sensitive internal emails or communications, including disciplinary actions, to embarrass the company. |

---

## **Mitigations**

1. Use social media monitoring tools to track mentions of the company name, products, and key executives, enabling early detection of malicious posts.  
2. Establish clear policies on social media use for employees, including guidelines for sharing company-related information.  
3. Provide training to employees on the legal and reputational risks of unauthorized social media posts.  
4. Work with legal and public relations teams to establish protocols for responding to damaging social media posts.  
5. Implement Data Loss Prevention (DLP) tools to detect and block attempts to exfiltrate sensitive data for sharing on public forums or social media.  

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
| Social Media Monitoring Alert  | Flags mentions of company names, products, or proprietary information on public platforms.       | [Example Link](#) | High           |
| Data Exfiltration Alert        | Detects attempts to export sensitive data for posting on social media or forums.                | [Example Link](#) | High           |
| Behavioral Anomaly Alert       | Flags unusual behavior, such as accessing large amounts of sensitive data shortly before resignation or public disclosures. | [Example Link](#) | Medium         |

