# **Unapproved Remote Access Tool Use**  

ID: IT1062  

Tactic: Business Impact  

Platform: Linux / Mac / Mobile / Windows  

Permissions Required: Standard  

Data Sources: Application Logs / Collaboration Logs / Endpoint Logs / Network Traffic / Process Monitoring / Remote Access Logs  

Version: 1.0  

Created: 06/04/2026  

Last Modified: 06/04/2026  

---

## **Overview:**  

Employees may install, launch, or use unapproved remote desktop, remote support, remote management, or meeting-control tools that allow another person to access or operate a corporate device. This can include commercial remote access tools, portable support utilities, browser-based remote sessions, screen-sharing control features, or long collaboration sessions used primarily to pass keyboard and mouse control.

This behavior can enable unauthorized outsourcing, policy evasion, credential misuse, data exposure, or unapproved third-party access through a trusted employee device. It is especially concerning when the session is long-running, occurs outside normal work patterns, has no clear business purpose, or shows little normal meeting activity such as audio, video, chat, or multiple attendees.

Organizations should distinguish approved IT support and business collaboration from unmanaged access paths that allow unvetted users to work through an employee's laptop.

---

## **Example Scenario:**  

| **Name** | **Description** |
|---------|---------------|
| **Unapproved Remote Desktop Tool** | An employee installs a tool such as a remote support or desktop-control application so an outside person can access their corporate laptop. |
| **Meeting-Based Device Control** | A user starts a long screen-sharing meeting with no audio or video and grants remote control to another person. |
| **Portable Remote Support Utility** | A contractor runs a portable remote access tool that does not follow normal software approval or endpoint management processes. |
| **Third-Party Work Through Trusted Device** | An unauthorized helper performs assigned work through the employee's active session, avoiding direct authentication by the third party. |

---

## **Mitigations:**  

1. **Define approved remote access and support tools** for IT, vendors, contractors, and employees.  
2. **Restrict or block unapproved remote desktop and remote management applications** on managed endpoints.  
3. **Require business justification and approval** for third-party support sessions, remote control, and vendor access.  
4. **Review meeting-control capabilities** such as remote control, unattended screen share, and long sessions with limited participant activity.  
5. **Educate employees** that allowing another person to operate through their device may violate security, privacy, employment, and contractual expectations.  
6. **Coordinate suspicious cases with HR, legal, privacy, management, and security** before drawing conclusions from tool use alone.  

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
| **Unapproved Remote Access Tool Review** | Reviews remote desktop, remote support, or remote management tools outside the approved software list. | [Example Link](#) | High |
| **Long Remote Control Session Review** | Identifies long screen-sharing or remote-control sessions with limited normal meeting activity. | [Example Link](#) | Medium |
| **Portable Remote Tool Review** | Reviews portable or user-installed remote access utilities that bypass normal software management. | [Example Link](#) | High |
| **Third-Party Access Pattern Review** | Correlates remote access activity with outsourcing concerns, unusual work patterns, or unmanaged external support. | [Example Link](#) | High |

---

### **Additional Considerations**  

1. **Why It's Critical:**  
   - Remote access tools can allow an unapproved person to operate through a trusted employee device and session.  
   - This can bypass normal account provisioning, vendor approval, access review, and identity controls.  

2. **Broader Monitoring:**  
   - Review this behavior with endpoint, network, collaboration, identity, HR, legal, privacy, and management context.  
   - Distinguish legitimate IT support, accessibility needs, and approved vendor assistance from unauthorized device control.  

---

