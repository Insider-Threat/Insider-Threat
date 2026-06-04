# Data Sources

Insider threat program reviews depend on connecting behavior to context. The table below maps common information sources to the risk areas they most often support.

| **Data Source** | **Useful For** | **Example Signals** |
|---|---|---|
| Identity and authentication logs | Account misuse, unusual access, OAuth consent, privilege activity | Impossible travel, failed logins, new app consent, risky sessions |
| Endpoint information | Collection, staging, removable media, sync clients, process behavior | File copies, archive creation, USB insertion, sync client execution |
| DLP events | Sensitive data movement and policy violations | Sensitive labels, blocked uploads, clipboard events, email/file violations |
| Email logs | External forwarding, attachments, competitor correspondence, data movement | Large attachments, auto-forwarding, external recipients, unusual volume |
| SaaS audit logs | Cloud file sharing, AI tools, OAuth grants, collaboration activity | Public links, external users, mass downloads, app permissions |
| AI usage and billing records | AI cost governance, token usage, model access, non-business usage | Usage spikes, high-cost model selection, subscription spend, project attribution |
| Browser and extension inventory | Unapproved plugins, page capture, scraping, unmanaged sync | New extensions, broad permissions, AI assistants, personal sync destinations |
| Meeting and transcript records | Sensitive meeting content, AI notes, recording exposure | External shares, broad permissions, third-party note takers, transcript exports |
| Workflow automation logs | AI agents, bots, low-code workflows, connected SaaS actions | New connectors, broad scopes, automated file movement, unowned workflows |
| Cloud storage logs | Data exposure, unauthorized sharing, bulk access | Public buckets, anonymous links, unusual download patterns |
| Source code repository logs | IP exposure, credential leakage, unusual cloning | Public repo creation, secret commits, unusual clone/export behavior |
| HR data | Risk context and response routing | Resignation notice, role change, leave status, department turnover |
| Physical security logs | Restricted-area access and device tampering | Badge access, denied entry, after-hours access, alarm events |
| Financial and business systems | Fraud, misappropriation, timekeeping, insider trading risk | Payment changes, access to confidential deal data, time edits |
| Productivity and presence signals | Timekeeping misuse, availability concerns, productivity-monitoring evasion | Artificial activity, unusual solo meetings, anti-idle tools, lockscreen avoidance |

## Minimum Useful Information Sources

A small program can start with:

- Identity/authentication logs
- Endpoint file and process information
- Email metadata
- Cloud file-sharing audit logs
- DLP or sensitivity-label events
- HR status context with proper governance

## Useful Context Fields

The most useful reviews usually include:

- User, department, manager, role, and employment status
- Device identity and management state
- Source application and destination application
- Data sensitivity label or repository classification
- File count, byte volume, and time window
- External domain, recipient, app publisher, or storage provider
- Prior baseline for the user and peer group

## Data Governance Notes

- Limit access to HR and employee-risk context.
- Document who can view insider threat alerts and why.
- Separate security review from employment decisions.
- Review use cases with legal, privacy, HR, and security leadership.
