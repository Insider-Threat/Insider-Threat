# **Unauthorized OAuth Application Consent**  

ID: IT1051  

Tactic: Initial Discovery  

Platform: Linux / Mac / Mobile / Windows  

Permissions Required: Standard  

Data Sources: Application Logs / Authentication Logs / Cloud Logs / Identity & Access Management (IAM) / SaaS Audit Logs  

Version: 1.0  

Created: 05/28/2026  

Last Modified: 05/28/2026  

---

## **Overview:**  

Employees may grant **third-party OAuth applications** access to corporate email, files, calendars, contacts, or collaboration platforms without security approval. This can happen through **consent phishing**, convenience-based use of unapproved productivity tools, or intentional authorization of an external application to retain access to company data.  

Unlike password-based access, OAuth tokens may continue working after the initial login and can allow data access through approved cloud APIs. This creates risk when applications request broad scopes such as **mail read**, **offline access**, **file read/write**, or access to all user data.  

Organizations should monitor OAuth application grants, application publisher reputation, scope changes, and high-risk consent activity as part of insider threat detection.  

---

## **Example Scenario:**  

| **Name** | **Description** |
|---------|---------------|
| **Unapproved Productivity App** | An employee grants a personal task-management application access to corporate email and files to make their work easier, exposing confidential business data to an unmanaged vendor. |
| **Consent Phishing Link** | A user clicks a phishing link and approves an application requesting mail and file permissions, giving an external actor persistent access through OAuth tokens. |
| **Departing Employee Data Access** | Before resigning, an employee authorizes a third-party sync application with offline access so they can continue retrieving documents after leaving. |
| **Broad Permission Request** | A low-reputation application requests permissions that exceed its business purpose, such as reading all mailbox content or accessing every file the user can reach. |

---

## **Mitigations:**  

1. **Restrict user consent** for high-risk OAuth scopes and require administrator approval for sensitive application permissions.  
2. **Review and approve third-party SaaS applications** before allowing access to corporate data.  
3. **Monitor OAuth consent events** for new applications, unusual publishers, broad scopes, and consent activity by high-risk users.  
4. **Revoke unused or suspicious application grants** and rotate affected sessions or tokens when suspicious consent is identified.  
5. **Educate employees** on consent phishing and the risk of approving applications that request unnecessary access.  
6. **Use CASB, IAM, or SaaS security posture tools** to inventory application grants and detect risky integrations.  

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
| **New OAuth Grant Alert** | Detects when a user grants a new third-party application access to corporate data. | [Example Link](#) | Medium |
| **High-Risk Scope Alert** | Flags OAuth applications requesting sensitive permissions such as mail read, file read/write, or offline access. | [Example Link](#) | High |
| **Suspicious Publisher Alert** | Identifies application consent from unverified, newly created, or low-reputation publishers. | [Example Link](#) | High |
| **Departing User Consent Alert** | Correlates new application consent activity with resignation, termination, or high-risk HR status. | [Example Link](#) | High |

---

### **Additional Considerations**  

1. **Why It’s Critical:**  
   - OAuth grants can provide **persistent access** without requiring a user password after the initial consent.  
   - Unauthorized application consent can expose **email, files, contacts, calendars, and collaboration data** through trusted cloud APIs.  

2. **Broader Monitoring:**  
   - Correlate OAuth consent events with **file downloads, mailbox access, unusual sign-ins, and HR risk signals.**  
   - Review application grants for privileged users, executives, developers, and employees with access to sensitive repositories or customer data.  

---

