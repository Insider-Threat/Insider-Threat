# **Excessive AI Token or Compute Usage**  

ID: IT1055  

Tactic: Business Impact  

Platform: Linux / Mac / Mobile / Windows  

Permissions Required: Standard  

Data Sources: Application Logs / Billing Records / Cloud Logs / Expense Reports / SaaS Audit Logs  

Version: 1.0  

Created: 05/28/2026  

Last Modified: 05/28/2026  

---

## **Overview:**  

Employees may misuse company-funded AI tools, model APIs, or compute resources in ways that create excessive cost, operational impact, or budget risk. This may include running unnecessary high-volume prompts, using expensive models for low-value tasks, leaving automated workflows running, repeatedly resubmitting large files, or generating content unrelated to business needs.  

Token usage, model selection, file processing, agentic workflows, embeddings, transcription, image/video generation, and fine-tuning can all create meaningful expense. Misuse may be intentional, accidental, or caused by poor process design. In some cases, a user may also attempt to hide personal or non-business usage inside normal corporate AI spend.  

Organizations should treat AI consumption as a managed business resource with ownership, review, approval paths, and clear acceptable-use expectations.  

---

## **Example Scenario:**  

| **Name** | **Description** |
|---------|---------------|
| **Runaway Prompt Workflow** | An employee creates an automated AI workflow that repeatedly processes the same large document set, driving unnecessary token usage and cost. |
| **Unapproved High-Cost Model Use** | A user consistently selects premium or high-cost models for routine tasks that could be handled by approved lower-cost options. |
| **Bulk File Reprocessing** | A team member repeatedly uploads large files for summarization or analysis without a defined business need, causing avoidable consumption charges. |
| **Hidden Personal Usage** | An employee uses a company AI account for personal projects, side work, or non-business content generation that is billed to the organization. |

---

## **Mitigations:**  

1. **Define acceptable AI usage** including approved business purposes, model selection expectations, and prohibited personal use.  
2. **Set budgets, quotas, or consumption thresholds** for users, teams, and applications where supported.  
3. **Review AI spend and usage reports** with business owners on a regular cadence.  
4. **Require approval for high-cost AI activities** such as large-scale processing, fine-tuning, advanced model usage, or automated workflows.  
5. **Educate users** on token usage, cost drivers, and responsible AI consumption.  
6. **Assign ownership** for AI cost governance across security, finance, procurement, IT, and business teams.  

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
| **AI Cost Spike Review** | Flags sudden or unexplained increases in AI spend for a user, team, app, or project. | [Example Link](#) | Medium |
| **High-Volume Token Usage Review** | Identifies unusually high prompt, file, or token usage compared with expected business activity. | [Example Link](#) | Medium |
| **Premium Model Usage Review** | Reviews use of expensive models or capabilities outside approved business cases. | [Example Link](#) | Medium |
| **Non-Business AI Usage Review** | Identifies usage patterns that suggest personal, side-project, or non-business activity. | [Example Link](#) | High |

---

### **Additional Considerations**  

1. **Why It’s Critical:**  
   - AI consumption can create material spend quickly, especially with automated workflows or large file processing.  
   - Cost misuse may also indicate broader governance gaps around AI access, procurement, data handling, and acceptable use.  

2. **Broader Monitoring:**  
   - Review AI usage alongside expense records, procurement approvals, business unit ownership, and project justification.  
   - Distinguish malicious misuse from poor training, unclear policy, or badly designed automation.  

---

