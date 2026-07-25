# OctoAcme Project Management Process

This folder captures OctoAcme's lightweight, structured project management process from idea to continuous improvement.

## Lifecycle Overview
1. **Initiation**: validate business need, define measurable outcomes, identify stakeholders, and confirm go/no-go with a one-pager, initial risks, and resource view.
2. **Planning**: break work into shippable increments with prioritized backlog items, acceptance criteria, estimates, dependencies, and a release/milestone map.
3. **Execution**: deliver iteratively using the project board flow (**Backlog -> Ready -> In Progress -> In Review -> QA -> Done**) with small PRs when possible, required review, and CI checks before merge.
4. **Release**: ship with release readiness checks (acceptance criteria complete, CI/security passing, release notes, rollback planning, staged verification, and post-deploy checks).
5. **Retrospective**: after sprints, releases, or incidents, capture lessons learned and convert them into tracked action items with owners and due dates.

## Roles and Ownership
- **Project Managers (PMs)**: own delivery coordination, schedules, risk/dependency tracking, and status communication.
- **Product Managers (PdMs)**: own product outcomes, roadmap/backlog prioritization, and impact measurement.
- **Developers**: own technical implementation quality (design, code, reviews, and automated testing) and contribute to estimates and risk mitigation.
- **QA/Testing**: own acceptance validation, functional/regression verification, and release readiness confirmation.
- **Stakeholders**: own timely business/domain input, milestone decisions, and required approvals.

## Communication Cadence and Escalation
- Daily (or twice-weekly) standups for progress, blockers, and dependencies.
- Weekly PM/PdM delivery syncs for plan, risk, and milestone alignment.
- Sprint or milestone demos to share outcomes and gather feedback.
- Monthly stakeholder updates for status, risks, and decisions.
- Escalation path: **Team-level triage -> PM -> Product Lead -> Sponsor** (with security incidents routed through the security incident process).

## Risk Management and Single Source of Truth
- Risks are tracked in a living **risk register** with columns for ID, description, impact (High/Med/Low), likelihood (High/Med/Low), owner, mitigation plan, and status.
- The register is reviewed weekly and updated as risks are identified, assessed, mitigated, or resolved.
- Security incidents follow the security incident runbook and notify the Security on-call team, while non-security escalations follow the standard path defined above.
- Maintain a **single source of truth** for project status (project README or release doc). Use standard templates for weekly status updates (progress, next steps, risks/blockers, decisions needed) and incident communications to keep decisions and asks visible to all stakeholders.

## Quality and Release Discipline
- Unit tests for new logic, integration tests where appropriate, and smoke tests for critical flows.
- CI expectations include automated testing, linting, and security scanning.
- Merges and releases require clear acceptance criteria, review completion, and documented release/rollback notes.

## Continuous Improvement
Retrospectives are part of normal delivery cadence, not optional postmortems. Teams track improvement actions in backlog items or issues, assign owners and due dates, and review progress in weekly syncs.
