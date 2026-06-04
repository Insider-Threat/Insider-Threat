# Getting Started

This project is intended to help security, legal, privacy, HR, and risk teams describe insider threat behaviors in a shared language. It is not a product-specific rule pack. Treat it as a program and detection planning reference.

## Quick Start

1. Start with the matrix in the main README.
2. Pick the tactics that match your current priorities: proactive measures, initial discovery, collection, exfiltration, or business impact.
3. Review the TTP pages for likely scenarios, mitigations, affected groups, and detection ideas.
4. Use `TTPs/ttp_primary.csv` to filter by tactic, data source, platform, or permission level.
5. Use the maturity matrix to score your current coverage and identify practical next steps.

## Suggested Program Workflow

1. **Scope:** Decide which business units, data types, and employee populations are in scope.
2. **Data Sources:** Identify which information sources are already available and which require onboarding.
3. **Prioritize:** Select a small number of high-risk TTPs instead of trying to detect everything at once.
4. **Define Review Criteria:** Decide what evidence, context, and business exceptions matter for each selected TTP.
5. **Triage:** Review expected business behavior, false positives, and risk indicators.
6. **Respond:** Define escalation paths that include security, HR, legal, privacy, and business owners.
7. **Mature:** Revisit the maturity matrix quarterly or after major business/process changes.

## Good First TTPs

These TTPs usually provide strong early value because they map to common program concerns:

- `IT1024` Upload to 3rd Party File Share
- `IT1025` External Email with Attachments
- `IT1026` Upload to Removable Storage Device
- `IT1039` Exposure of Sensitive/Confidential Information in Public Repositories
- `IT1040` Use of File Share Site with External User
- `IT1042` Multiple Employees Leaving to Same Company
- `IT1051` Unauthorized OAuth Application Consent
- `IT1052` Sensitive Data in External AI Tools
- `IT1053` Personal Cloud Sync Client
- `IT1054` Copying Sensitive Data to Clipboard
- `IT1055` Excessive AI Token or Compute Usage
- `IT1056` Unauthorized AI Use for External Work
- `IT1057` Unauthorized Browser Extension or Plugin Use
- `IT1058` Sensitive Data in Meeting Transcripts or Recordings
- `IT1059` Unapproved AI Agent or Automation Workflow
- `IT1060` Mass Export from SaaS Application
- `IT1061` Productivity Monitoring Evasion
- `IT1062` Unapproved Remote Access Tool Use

## Operating Principles

- Pair monitoring concepts with documented business process.
- Use HR or employment signals only with appropriate legal, privacy, and governance review.
- Prefer risk correlation over single-event alerting whenever possible.
- Document false positives and expected business exceptions.
- Review sensitive monitoring use cases regularly to maintain trust and compliance.
