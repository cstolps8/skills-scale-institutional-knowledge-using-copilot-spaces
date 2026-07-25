# OctoAcme — Decision Log Template

## Purpose
Capture significant project decisions in a structured, searchable format so that the rationale, context, and trade-offs are preserved for the team and future contributors. A good decision log prevents revisiting settled questions, speeds up onboarding, and surfaces patterns for continuous improvement.

## When to Log a Decision
Log a decision when it:
- Affects project scope, architecture, or delivery approach
- Involves trade-offs between two or more viable options
- Cannot be easily reversed without meaningful cost or delay
- Is likely to be questioned or revisited (by new team members or in a retrospective)
- Requires stakeholder alignment or formal approval

Routine implementation choices (e.g., variable naming, minor UI tweaks) do not require a log entry.

## Decision Cadence
- **Ongoing**: any team member may open a decision record at any time by creating a new entry below or a linked issue.
- **Weekly delivery sync**: the Project Manager reviews open (pending) decisions and escalates any that are blocked.
- **Sprint / milestone planning**: close or archive decisions that are no longer relevant; summarize key decisions in the milestone retrospective.
- **Release sign-off**: confirm that all decisions affecting the release are in an `Accepted` or `Superseded` state with no pending items.

## Decision Record Format

Use the template below for each decision. Copy it and add a new section for every significant decision.

---

### Decision Record: [Short Title]

| Field | Value |
|---|---|
| **ID** | DR-001 *(increment per record)* |
| **Date** | YYYY-MM-DD |
| **Status** | `Proposed` / `Accepted` / `Rejected` / `Superseded` |
| **Decider(s)** | Name(s) and role(s) of people who made the final call |
| **Consulted** | Name(s) and role(s) of people whose input was sought |
| **Informed** | Name(s) and role(s) of people who were notified of the outcome |

**Context**
Describe the situation, constraints, and forces that make this decision necessary. Include relevant background, timeline pressures, technical limitations, or compliance requirements.

**Decision**
State the decision clearly and concisely. If the decision was made between options, state which option was chosen.

**Options Considered**

| Option | Pros | Cons |
|---|---|---|
| Option A | … | … |
| Option B | … | … |
| Option C *(if applicable)* | … | … |

**Rationale**
Explain why the chosen option was selected over the alternatives. Reference data, user research, technical analysis, or stakeholder input as appropriate.

**Consequences**
Describe the expected outcomes — both positive and negative. Note any follow-up actions, risk mitigations, or items that this decision opens or closes.

**Follow-up Actions**

| Action | Owner | Due Date |
|---|---|---|
| … | … | … |

**Links / References**
- Related issues, PRs, or ADRs: #…
- Supporting documents or meeting notes: …

---

## Decision Log Index

Maintain a running index here so the log is easy to scan. Add a row for each new decision record.

| ID | Date | Title | Status | Decider |
|---|---|---|---|---|
| DR-001 | YYYY-MM-DD | *Example: Choose primary database engine* | Accepted | PM, Tech Lead |
| DR-002 | YYYY-MM-DD | *Example: Defer internationalization to v2* | Accepted | PdM |

## Tips for Effective Decision Logging
- Write the **Context** section before discussing options — shared context improves the quality of the discussion.
- Date entries accurately; retroactive entries are allowed but should be flagged.
- When a decision is superseded, update the old record's status to `Superseded` and link to the new record.
- Store this log close to the code or in the project wiki so it stays discoverable.
- Reference decision records in PR descriptions and retrospective notes to maintain a traceable history.
