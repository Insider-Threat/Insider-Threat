# **Sensitive Data in External AI Tools**  

ID: IT1052  

Tactic: Exfiltration  

Platform: Linux / Mac / Mobile / Windows  

Permissions Required: Standard  

Data Sources: Application Logs / Browser History / DLP Events / Endpoint Logs / Network Traffic / SaaS Audit Logs  

Version: 1.0  

Created: 05/28/2026  

Last Modified: 05/28/2026  

---

## **Overview:**  

Employees may paste, upload, or submit sensitive company information to **external generative AI tools**, coding assistants, transcription services, summarization tools, or other AI-enabled platforms. This behavior may be unintentional, such as using an AI tool to summarize a customer document, or intentional, such as using a personal AI account to analyze proprietary research outside approved monitoring.  

Sensitive data submitted to unmanaged AI platforms can include **source code, customer records, legal documents, merger information, credentials, incident details, financial data, or intellectual property.** Depending on the tool and account type, the organization may lose visibility, retention control, or contractual protections over the submitted content.  

Organizations should treat unmanaged AI submissions as a modern data handling and exfiltration risk, especially when combined with high-risk employee status, bulk copying, or attempts to bypass approved enterprise AI tools.  

---

## **Example Scenario:**  

| **Name** | **Description** |
|---------|---------------|
| **Source Code Prompt Upload** | A developer pastes proprietary source code into a personal AI assistant to debug an issue, exposing trade secrets outside approved systems. |
| **Customer Data Summarization** | A sales employee uploads a spreadsheet containing customer contact information and deal details to an external AI tool to generate a summary. |
| **Legal Document Review** | An employee submits confidential contracts to a public AI service to identify key terms before an acquisition announcement. |
| **Credentials in Prompt History** | An engineer accidentally includes API keys, internal hostnames, or incident response notes in an AI prompt stored outside corporate retention controls. |

---

## **Mitigations:**  

1. **Provide approved enterprise AI tools** with contractual, logging, retention, and data protection controls.  
2. **Block or restrict unmanaged AI services** for users and data classifications that require stronger controls.  
3. **Apply DLP policies** to browser uploads, pasted content, file attachments, and API traffic where supported.  
4. **Classify sensitive data** and educate employees on what cannot be submitted to external AI systems.  
5. **Monitor for prompt, upload, and browser activity** involving sensitive labels, source code, credentials, or regulated data.  
6. **Review AI tool usage during offboarding or investigation workflows** when other insider risk indicators are present.  

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

## **Detection:**  

| **Name** | **Description** | **Link** | **Risk Score** |
|---------|---------------|--------|--------------|
| **Sensitive Prompt Submission Alert** | Detects attempts to paste or submit sensitive content to unmanaged AI tools. | [Example Link](#) | High |
| **AI File Upload Alert** | Flags uploads of documents, source code, spreadsheets, or classified files to external AI services. | [Example Link](#) | High |
| **Credential in AI Prompt Alert** | Identifies secrets, tokens, keys, or internal connection strings submitted through browser or API activity. | [Example Link](#) | Critical |
| **Departing User AI Usage Spike** | Correlates increased use of external AI tools with resignation, termination, or other elevated-risk HR indicators. | [Example Link](#) | Medium |

---

### **Additional Considerations**  

1. **Why It’s Critical:**  
   - AI tools can make it easy for insiders to move large amounts of sensitive content through ordinary browser workflows.  
   - Submitted data may be stored, logged, retained, or processed outside the organization’s approved security and compliance boundaries.  

2. **Broader Monitoring:**  
   - Combine AI usage telemetry with **DLP, browser, endpoint, proxy, and SaaS audit logs.**  
   - Monitor both intentional misuse and accidental disclosure, since many AI-related incidents begin as productivity shortcuts.  

---

