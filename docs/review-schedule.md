# Review Schedule

Keeping the repository fresh works best when updates are lightweight, regular, and tied to real changes in work patterns, tooling, and insider risk. This schedule is intended for maintainers who want a practical cadence without turning the project into a heavy governance process.

## Recommended Cadence

| **Cadence** | **Focus** | **Output** |
|---|---|---|
| Monthly | Quick scan for new workplace behaviors, SaaS/AI changes, public discussion themes, and obvious README or link issues | Small issue list or minor content refresh |
| Quarterly | Review TTP coverage, data sources, use cases, maturity matrix alignment, and stale wording | Prioritized update batch |
| Semiannual | Re-score program guidance against current insider threat patterns and business processes | Maturity matrix refresh and gap review |
| Annual | Review project structure, taxonomy, documentation clarity, and whether major categories are missing | Roadmap for larger content improvements |
| Event-driven | Update after major shifts such as new AI tools, layoffs, mergers, remote-work changes, new SaaS platforms, regulatory changes, or notable insider threat incidents | Targeted TTP or guidance update |

## Monthly Review

- Scan recent workplace, SaaS, AI, remote-work, and insider-risk themes.
- Check whether new behaviors fit an existing TTP before creating a new one.
- Review open notes, issues, or candidate ideas.
- Fix broken links, awkward wording, and obvious matrix layout issues.
- Confirm newly added TTPs are present in the README matrix and `TTPs/ttp_primary.csv`.

## Quarterly Review

- Review the balance of TTPs across tactics.
- Identify gaps in modern SaaS, AI, collaboration, remote work, identity, and business-process misuse.
- Confirm data sources are described at a program level.
- Revisit `docs/use-cases.md` to ensure new TTPs appear in the right program scenarios.
- Update `docs/getting-started.md` if new TTPs become strong first-priority examples.
- Review the maturity matrix for stale categories or unclear scoring language.

## Annual Review

- Reassess whether the five major tactics still fit the project.
- Review old TTPs for outdated tooling assumptions or overly technical language.
- Look for duplicate or overlapping TTPs that should be merged.
- Identify missing business-facing guidance for HR, legal, privacy, finance, procurement, and security.
- Review whether the project still helps a new reader understand what to do first.

## Candidate TTP Intake

When considering a new TTP, ask:

1. Is this a distinct behavior, or is it a scenario inside an existing TTP?
2. Is it useful at a program level without needing product-specific detection logic?
3. Does it map to a clear tactic, data source, and business risk?
4. Would a security, HR, legal, privacy, or risk leader understand why it matters?
5. Can the TTP include practical mitigations and review questions?

## Definition of Done

For most content updates, a complete refresh includes:

- TTP markdown added or updated.
- `TTPs/ttp_primary.csv` updated.
- README matrix updated if a new TTP was added.
- Relevant docs updated, usually `docs/use-cases.md`, `docs/data-sources.md`, or `docs/getting-started.md`.
- Links and index consistency checked.

