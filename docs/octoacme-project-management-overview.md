# OctoAcme Project Management Overview

## Purpose
Provide a concise, shareable introduction to how OctoAcme runs projects so new teammates can quickly understand our approach, roles, and key artifacts.

## Scope
Applies to all cross-functional projects that deliver product features, services, or integrations.

## Principles
- Customer-first: prioritize customer value and usability.
- Iterative delivery: deliver small, testable increments.
- Clear ownership: each project has a named Project Manager (PM) and Product Lead.
- Data-informed decisions: measure impact and iterate based on evidence.
- Psychological safety: encourage feedback and learning.

## Core Roles
- Project Manager (PM): coordinates delivery, schedules, risk, communications.
- Product Manager (PdM): defines outcomes, prioritizes backlog, and measures success.
- Engineering Manager / Tech Lead: provides technical direction, architecture oversight, and mentoring.
- Developers: implement features, collaborate on design and testability.
- UX / UI Designer: creates user flows, design specs, and validates implementation fidelity.
- QA/Testing: validate quality and acceptance criteria.
- DevOps / Platform Engineer: owns CI/CD, environments, and deployment automation.
- Security / Compliance Lead: owns threat modeling, security controls, and compliance checkpoints.
- Customer Support / Operations Representative: surfaces customer pain points and ensures support readiness.
- Data Analyst / Analytics Owner: defines success metrics, validates instrumentation, and publishes insights.
- Stakeholders: provide inputs and approvals.

See [Roles and Personas](octoacme-roles-and-personas.md) for full role definitions.

## Key Artifacts
- Project Charter / One-pager
- Roadmap and Release Plan
- Sprint/Iteration Backlog
- Acceptance Criteria & Definition of Done
- Risk Register
- Decision Log (see [Decision Log Template](octoacme-decision-log-template.md))
- Phase Gate Sign-offs (see [Phase Gates Checklist](octoacme-phase-gates-checklist.md))
- Handoff Records (see [Handoff Checklist](octoacme-handoff-checklist.md))
- Retrospective notes and action items

## Lifecycle (high-level)
1. Initiation: problem statement, stakeholders, high-level timeline.
2. Planning: scope, resources, milestones, dependencies.
3. Execution: build, test, review, iterate.
4. Release: deploy, verify, announce.
5. Close & Retrospective: capture learnings and next steps.

## Communication Cadence
- Weekly sync between PM + PdM
- Twice-weekly standups for delivery team (or as agreed)
- Monthly stakeholder updates
- Ad-hoc escalations as needed

## How to use these docs
- Keep the Project Charter updated in the project repo.
- Log significant decisions using the [Decision Log Template](octoacme-decision-log-template.md) throughout the lifecycle.
- Use the [Phase Gates Checklist](octoacme-phase-gates-checklist.md) to confirm readiness before transitioning between lifecycle phases.
- Use the [Handoff Checklist](octoacme-handoff-checklist.md) to ensure clean knowledge and accountability transfer at each phase boundary.
- Refer to [Roles and Personas](octoacme-roles-and-personas.md) for full role definitions and interaction models for all team members.
- Add process-specific docs into `.copilot/` if you want Copilot Spaces to use them as context.
