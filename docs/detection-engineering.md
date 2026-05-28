# Detection Engineering Guide

The TTPs in this repository are intentionally vendor-neutral. Use this guide to convert them into practical detections in SIEM, UEBA, DLP, endpoint, SaaS security, or case-management platforms.

## Detection Design Pattern

For each TTP, define:

| **Field** | **Purpose** |
|---|---|
| Objective | What behavior should this detect? |
| Required telemetry | Which logs or events must exist? |
| Logic | What events, thresholds, joins, or sequences matter? |
| Risk context | Which users, roles, data types, or HR signals increase severity? |
| False positives | What normal business activity looks similar? |
| Tuning | How thresholds, allowlists, and peer baselines should be adjusted |
| Response | Who reviews the alert and what evidence is needed? |

## Common Correlation Ideas

- **Resignation plus bulk access:** HR departure signal followed by large downloads, file copies, or external sharing.
- **Sensitive data plus unmanaged destination:** DLP-labeled files moved to personal email, cloud sync, AI tools, or public repos.
- **New access plus unusual behavior:** Newly granted access followed by activity outside normal scope.
- **Staging plus upload:** Archive creation or local copying followed by external transfer.
- **OAuth consent plus data access:** New third-party application grant followed by mailbox or file API activity.

## Severity Model

Use a simple starting model:

| **Severity** | **Description** |
|---|---|
| Low | Weak signal, low sensitivity data, expected business context |
| Medium | Unusual behavior or sensitive data, but plausible business reason |
| High | Sensitive data, unmanaged destination, risky user context, or multiple correlated signals |
| Critical | Credential exposure, confirmed exfiltration, destructive activity, or privileged misuse |

## Tuning Checklist

- Exclude approved business applications and sanctioned vendors.
- Tune by user role and peer group.
- Separate first-time activity from repeated activity.
- Add thresholds for file count, byte volume, recipient count, and time window.
- Suppress known migrations, backups, legal holds, and approved investigations.
- Review detections after organizational changes, mergers, restructures, or new SaaS rollouts.

## Response Checklist

- Preserve relevant logs and file metadata.
- Review user context with authorized HR/legal/privacy partners.
- Confirm whether data was sensitive, regulated, or business-critical.
- Identify destination accounts, domains, applications, or devices.
- Revoke access, tokens, shares, or sessions when required.
- Document disposition: benign, policy issue, suspicious, confirmed incident.

