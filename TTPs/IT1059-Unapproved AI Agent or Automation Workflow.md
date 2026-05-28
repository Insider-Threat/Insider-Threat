# **Unapproved AI Agent or Automation Workflow**  

ID: IT1059  

Tactic: Business Impact  

Platform: Linux / Mac / Mobile / Windows  

Permissions Required: Standard  

Data Sources: AI Usage Logs / Application Logs / Cloud Logs / SaaS Audit Logs / Workflow Automation Logs  

Version: 1.0  

Created: 05/28/2026  

Last Modified: 05/28/2026  

---

## **Overview:**  

Employees may create or connect AI agents, workflow automations, bots, or low-code integrations that act on corporate systems without appropriate review. These workflows may read email, summarize documents, move files, update tickets, create tasks, query repositories, send messages, generate content, or trigger actions across SaaS applications.

Unapproved AI agents and automations can create data exposure, operational disruption, cost spikes, inaccurate business actions, unclear accountability, and vendor risk. The concern is not only the AI model itself, but the permissions and connected systems granted to the workflow.

Organizations should treat AI agents and automations as business processes that need ownership, approved use cases, access boundaries, and review paths.

---

## **Example Scenario:**  

| **Name** | **Description** |
|---------|---------------|
| **AI Agent Connected to Email** | A user connects an AI assistant to corporate email and allows it to summarize or draft messages without approved review. |
| **Automated File Movement** | A workflow moves documents between SaaS platforms or cloud folders without validating sensitivity, audience, or retention expectations. |
| **Unapproved Ticket Updates** | An automation updates customer or internal tickets based on generated summaries, creating inaccurate records or business impact. |
| **Broad SaaS Connector Access** | An employee grants an automation platform access to files, chat, calendars, repositories, or CRM data beyond its business need. |

---

## **Mitigations:**  

1. **Define an approval process** for AI agents, bots, low-code workflows, and SaaS automations that access corporate data.  
2. **Require business ownership** for automations that read, move, create, delete, or modify information.  
3. **Limit connector permissions** to the minimum data and actions required for the approved workflow.  
4. **Review vendor, privacy, and data handling risks** before connecting AI or automation tools to sensitive systems.  
5. **Maintain an inventory** of approved agents, workflows, owners, connected systems, and access scopes.  
6. **Create exception and shutdown procedures** for workflows that create cost, security, privacy, or operational risk.  

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
| **New Automation Review** | Reviews newly created AI agents, bots, workflows, or low-code integrations. | [Example Link](#) | Medium |
| **High-Risk Connector Review** | Identifies workflows with broad access to email, files, chat, calendars, repositories, CRM, or finance systems. | [Example Link](#) | High |
| **Automated Action Review** | Reviews automations that send messages, move files, update records, delete data, or trigger business actions. | [Example Link](#) | High |
| **Unowned Workflow Review** | Identifies automations without a clear business owner, approval record, or documented use case. | [Example Link](#) | Medium |

---

### **Additional Considerations**  

1. **Why It's Critical:**  
   - AI agents and automations can act with the permissions of the user or service account that created them.  
   - A small workflow can quickly affect many systems, records, or users.  

2. **Broader Monitoring:**  
   - Review automations with SaaS governance, identity, procurement, privacy, business process owners, and security.  
   - Separate approved workflow innovation from unmanaged automations that create unclear risk.  

---
