# **Sensitive Data in Meeting Transcripts or Recordings**  

ID: IT1058  

Tactic: Exfiltration  

Platform: Linux / Mac / Mobile / Windows  

Permissions Required: Standard  

Data Sources: Application Logs / Collaboration Logs / DLP Events / Meeting Platform Logs / SaaS Audit Logs  

Version: 1.0  

Created: 05/28/2026  

Last Modified: 05/28/2026  

---

## **Overview:**  

Employees may expose sensitive information through meeting recordings, transcripts, AI meeting notes, screen shares, chat exports, or automated summaries. Modern collaboration tools can capture product plans, legal discussions, customer details, credentials, financial information, HR matters, and internal strategy in formats that are easy to share or retain.

This risk may occur through accidental sharing, overly broad default permissions, personal account integrations, external meeting guests, or intentional distribution of recordings and transcripts outside approved channels. AI note-taking and transcription tools can increase the risk by producing searchable summaries that may be stored with third-party services.

Organizations should manage meeting artifacts as business records that may contain sensitive data, not as low-risk productivity outputs.

---

## **Example Scenario:**  

| **Name** | **Description** |
|---------|---------------|
| **External Transcript Sharing** | A user shares a transcript from an internal strategy meeting with an external collaborator. |
| **AI Meeting Notes Exposure** | An employee connects an unapproved AI note-taking tool that stores summaries of confidential meetings. |
| **Recording with Sensitive Screen Share** | A recorded meeting includes customer data, source code, credentials, financial forecasts, or HR content shown on screen. |
| **Broad Recording Permissions** | A meeting recording is saved to a shared workspace where users outside the intended audience can access it. |

---

## **Mitigations:**  

1. **Define recording and transcription expectations** for sensitive meetings, external guests, and regulated discussions.  
2. **Restrict default sharing permissions** for meeting recordings, transcripts, and AI-generated notes.  
3. **Require approval for third-party meeting assistants** that join calls, generate notes, or store transcripts.  
4. **Label and retain meeting artifacts** according to information governance and legal requirements.  
5. **Educate employees** on screen sharing, recording notices, transcript handling, and external guest risk.  
6. **Review meeting artifacts during sensitive events** such as investigations, M&A activity, restructuring, and product launches.  

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
| **External Recording Share Review** | Reviews recordings or transcripts shared with external users or broad audiences. | [Example Link](#) | High |
| **Unapproved Meeting Assistant Review** | Identifies third-party note-taking or transcription tools used outside approved channels. | [Example Link](#) | Medium |
| **Sensitive Meeting Artifact Review** | Reviews meeting artifacts tied to confidential topics, projects, customers, or legal matters. | [Example Link](#) | High |
| **Public or Broad Link Review** | Identifies recordings or transcripts available through public links or overly broad internal permissions. | [Example Link](#) | High |

---

### **Additional Considerations**  

1. **Why It's Critical:**  
   - Meeting artifacts can contain the same sensitive information as documents, email, and source systems.  
   - AI summaries can make confidential discussions easier to search, copy, and redistribute.  

2. **Broader Monitoring:**  
   - Review meeting records with legal, privacy, HR, records management, and business owners.  
   - Consider whether the issue is policy confusion, tool configuration, accidental oversharing, or intentional disclosure.  

---
