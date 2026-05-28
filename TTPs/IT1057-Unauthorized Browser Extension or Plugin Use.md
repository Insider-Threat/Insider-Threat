# **Unauthorized Browser Extension or Plugin Use**  

ID: IT1057  

Tactic: Collection  

Platform: Linux / Mac / Mobile / Windows  

Permissions Required: Standard  

Data Sources: Browser History / Browser Extension Inventory / DLP Events / Endpoint Logs / SaaS Audit Logs  

Version: 1.0  

Created: 05/28/2026  

Last Modified: 05/28/2026  

---

## **Overview:**  

Employees may install or use browser extensions, plugins, or add-ons that can access corporate web applications, browser sessions, form data, page content, screenshots, downloads, or clipboard activity. These tools may be installed for convenience, productivity, note-taking, translation, AI assistance, password management, shopping, development, or data extraction.

Unauthorized extensions can create insider threat risk even when the employee is not intentionally malicious. A plugin may sync data to a personal account, send content to an unmanaged vendor, scrape application pages, capture sensitive information, or introduce unclear data handling obligations.

Organizations should treat browser extensions as part of the corporate application and data access surface, especially for users who work heavily in SaaS applications.

---

## **Example Scenario:**  

| **Name** | **Description** |
|---------|---------------|
| **AI Browser Assistant** | A user installs an unapproved AI extension that can read active browser pages and summarize internal documents or customer records. |
| **Screen Capture Plugin** | An employee uses a browser plugin to capture pages from internal applications and save them to a personal account. |
| **Web Scraping Extension** | A user installs a plugin that extracts table data from a CRM, ticketing, or finance application. |
| **Personal Productivity Add-On** | A browser extension syncs notes, clips, or copied web content from corporate systems to an unmanaged personal service. |

---

## **Mitigations:**  

1. **Define an approved browser extension list** for managed browsers and high-risk user groups.  
2. **Restrict extensions with broad page access** unless there is a documented business need and vendor review.  
3. **Review extension permissions** such as read/write access to all websites, clipboard access, screenshots, downloads, and file access.  
4. **Educate users** on the risk of installing personal productivity, AI, scraping, or capture tools in corporate browsers.  
5. **Include browser extension review** in SaaS, privacy, procurement, and endpoint governance processes.  
6. **Remove or block unmanaged extensions** during offboarding, incident review, or when permissions create unacceptable risk.  

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
| **New Extension Review** | Reviews newly installed browser extensions against approved software and vendor expectations. | [Example Link](#) | Medium |
| **High-Permission Extension Review** | Identifies extensions requesting broad access to browser content, downloads, clipboard, or all websites. | [Example Link](#) | High |
| **Unmanaged Sync Extension Review** | Reviews extensions that send notes, clips, screenshots, or page content to personal or unmanaged services. | [Example Link](#) | High |
| **Scraping Tool Review** | Identifies extensions commonly used to extract data from SaaS applications or internal web portals. | [Example Link](#) | Medium |

---

### **Additional Considerations**  

1. **Why It's Critical:**  
   - Browser extensions often sit directly between users and sensitive SaaS applications.  
   - Extension permissions can allow collection or exposure of data without a traditional file download.  

2. **Broader Monitoring:**  
   - Review extension use with browser management, SaaS access, DLP, privacy, and procurement context.  
   - Distinguish approved productivity tooling from unmanaged tools with broad data access.  

---
