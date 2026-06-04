# Program Planning

This guide keeps the project focused on program design rather than implementation details. Use it to decide which insider threat behaviors matter, which teams should be involved, and what kind of evidence is needed to understand risk.

## Planning Questions

| **Question** | **Why It Matters** |
|---|---|
| What business assets are most sensitive? | Helps prioritize TTPs tied to intellectual property, customer data, finances, operations, or regulated data. |
| Which employee populations need extra context? | Helps identify groups such as executives, developers, finance users, privileged admins, or R&D teams. |
| Which business processes create insider risk? | Helps connect monitoring to offboarding, restructuring, travel, third-party work, investigations, and access changes. |
| Which teams need to be involved? | Insider threat work usually requires security, HR, legal, privacy, compliance, and business leadership. |
| What response paths already exist? | Helps avoid unclear ownership when an alert or concern needs review. |

## Prioritization Model

Start with a small set of TTPs that align to real business risk. A practical first pass is to score each candidate behavior across four dimensions:

| **Dimension** | **High-Level Scoring Prompt** |
|---|---|
| Business impact | Would this behavior create financial, legal, operational, reputational, or safety impact? |
| Likelihood | Is this behavior realistic for your environment and workforce? |
| Visibility | Can the organization observe enough context to assess the behavior responsibly? |
| Readiness | Are ownership, escalation, and review processes clear enough to act? |

## Program Review Checklist

- Identify the business owner for each high-priority risk area.
- Confirm legal, privacy, and HR expectations before expanding monitoring.
- Document what activity is expected, acceptable, suspicious, or prohibited.
- Define who reviews concerns and what evidence is needed before escalation.
- Maintain a list of approved business exceptions.
- Review TTP priorities after major organizational changes, layoffs, mergers, new SaaS tools, or policy changes.
- Use the [Review Schedule](https://github.com/Insider-Threat/Insider-Threat/blob/master/docs/review-schedule.md) to keep repository updates on a monthly, quarterly, semiannual, and annual cadence.

## Response Framing

High-level insider threat workflows should avoid jumping from one signal to a conclusion. A stronger review process asks:

1. What happened?
2. Is the activity expected for this user, role, project, or business unit?
3. What data, system, or process was involved?
4. Is there a policy, legal, privacy, or HR context?
5. Does the activity require coaching, control improvement, investigation, or incident response?

## Useful Program Outputs

- Prioritized list of TTPs by business unit or data type.
- Maturity matrix scores and improvement plan.
- Documented review/escalation process.
- Approved monitoring use cases.
- Business exception list.
- Quarterly program review notes.
