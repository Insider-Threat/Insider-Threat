# **Mass Export from SaaS Application**  

ID: IT1060  

Tactic: Collection  

Platform: Linux / Mac / Mobile / Windows  

Permissions Required: Standard  

Data Sources: Application Logs / Cloud Logs / DLP Events / SaaS Audit Logs / Sensitive Information Storage Locations  

Version: 1.0  

Created: 05/28/2026  

Last Modified: 05/28/2026  

---

## **Overview:**  

Employees may export unusually large volumes of data from SaaS applications such as CRM, HRIS, finance, ticketing, project management, source code, analytics, customer support, or collaboration platforms. Exports can include reports, CSV files, dashboards, archives, attachments, customer records, tickets, deal data, employee information, or project documentation.

Mass exports may be legitimate for business operations, audits, migrations, reporting, or analytics. They can also indicate collection before data exfiltration, unauthorized personal retention, competitive misuse, or misuse by a departing employee.

Organizations should review SaaS export behavior with business context, data sensitivity, user role, and expected process ownership.

---

## **Example Scenario:**  

| **Name** | **Description** |
|---------|---------------|
| **CRM Account Export** | A salesperson exports a large customer or prospect list before leaving for a competitor. |
| **HRIS Report Export** | A user exports employee records outside their normal responsibilities or without a clear business need. |
| **Ticketing System Archive** | A support user exports cases, attachments, or customer communications in bulk. |
| **Analytics Dashboard Download** | An employee repeatedly exports large reports containing sensitive performance, revenue, or product data. |

---

## **Mitigations:**  

1. **Define approved export use cases** for high-value SaaS applications and sensitive data sets.  
2. **Limit export permissions** to roles that need them and review access during role changes.  
3. **Require approval or business justification** for large exports, full-object exports, or sensitive report downloads.  
4. **Apply data classification and DLP controls** to exported files where supported.  
5. **Educate users** on acceptable handling of exported reports, CSV files, dashboards, and archives.  
6. **Review export activity** during offboarding, restructuring, investigations, and high-risk business events.  

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
| **Large SaaS Export Review** | Reviews unusually large exports from business applications compared with expected role or process. | [Example Link](#) | High |
| **Sensitive Report Export Review** | Identifies exports involving sensitive customer, employee, financial, legal, or product information. | [Example Link](#) | High |
| **Departing User Export Review** | Reviews export activity by users in resignation, termination, transfer, or restructuring contexts. | [Example Link](#) | High |
| **Repeated Export Review** | Identifies repeated report, dashboard, archive, or CSV exports over a short period. | [Example Link](#) | Medium |

---

### **Additional Considerations**  

1. **Why It's Critical:**  
   - SaaS applications often hold high-value business data that can be exported without touching traditional file shares.  
   - Export files are easy to email, upload, sync, print, or retain after access is removed.  

2. **Broader Monitoring:**  
   - Review SaaS exports with HR context, business owner approval, data sensitivity, and normal reporting processes.  
   - Distinguish approved reporting work from unusual collection, especially before departure or role change.  

---
