# **Unauthorized AI Use for External Work**  

ID: IT1056  

Tactic: Business Impact  

Platform: Linux / Mac / Mobile / Windows  

Permissions Required: Standard  

Data Sources: Application Logs / Billing Records / Browser History / Expense Reports / SaaS Audit Logs  

Version: 1.0  

Created: 05/28/2026  

Last Modified: 05/28/2026  

---

## **Overview:**  

Employees may use company-provided AI tools, subscriptions, model access, or API credits to support work outside their authorized job responsibilities. This can include side businesses, school work, job applications, freelance projects, social media content, outside consulting, or work for another employer.  

This behavior creates several risks: unauthorized use of company funds, misuse of licensed tools, exposure of company context or data, reputational harm, and unclear ownership of generated work product. Even when no sensitive data is submitted, the organization may still absorb cost and compliance risk for activity that does not support the business.  

AI tools make this behavior easier because one account can support writing, coding, research, translation, media creation, automation, and analysis across many personal or external use cases.  

---

## **Example Scenario:**  

| **Name** | **Description** |
|---------|---------------|
| **Freelance Content Generation** | An employee uses a company-paid AI account to generate marketing copy, graphics, or proposals for a personal freelance client. |
| **Outside Coding Work** | A developer uses corporate AI coding tools to support a side project or outside contract unrelated to their employer. |
| **Job Search Assistance** | A user relies heavily on company AI tools to create resumes, interview materials, or work samples for another employer. |
| **External Consulting Support** | An employee uses approved enterprise AI access to research, draft, or analyze materials for an unauthorized consulting engagement. |

---

## **Mitigations:**  

1. **Define acceptable personal and business use** of company-provided AI tools in policy and user guidance.  
2. **Require users to acknowledge AI acceptable-use expectations** before receiving access to paid tools or model APIs.  
3. **Review usage patterns** for signs of non-business activity, especially when costs, timing, or content categories are unusual.  
4. **Coordinate with HR, legal, privacy, and procurement** when policy, licensing, or employment concerns arise.  
5. **Separate personal experimentation from enterprise AI access** by offering approved sandbox options where appropriate.  
6. **Review AI access during role changes and offboarding** to ensure accounts, credits, and subscriptions are removed or transferred.  

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
| **Personal AI Usage Review** | Reviews AI activity that appears unrelated to assigned business responsibilities. | [Example Link](#) | Medium |
| **After-Hours AI Spend Review** | Identifies unusual consumption outside expected work hours or project timelines. | [Example Link](#) | Low |
| **External Work Product Review** | Flags patterns suggesting company AI resources are being used for outside clients, job searches, or personal ventures. | [Example Link](#) | High |
| **Unapproved Subscription Review** | Reviews AI subscriptions or expense items that bypass procurement or approved tooling processes. | [Example Link](#) | Medium |

---

### **Additional Considerations**  

1. **Why It’s Critical:**  
   - Company-funded AI access can be misused as a business asset even when no data exfiltration occurs.  
   - Unauthorized outside work can create conflicts of interest, licensing concerns, and reputational risk.  

2. **Broader Monitoring:**  
   - Review AI usage with expense, procurement, timekeeping, HR, and acceptable-use context.  
   - Clearly distinguish low-risk personal experimentation from repeated or costly use that supports external work.  

---

