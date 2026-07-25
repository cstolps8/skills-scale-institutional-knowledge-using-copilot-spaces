# OctoAcme — Phase Gates Checklist

## Purpose
Define clear entry and exit criteria for each lifecycle phase so the team knows when it is ready to begin a phase and when it is safe to move on. Phase gates reduce rework, prevent scope creep, and create natural checkpoints for stakeholder alignment and risk review.

## How to Use
- Review the **Entry Criteria** before starting a phase. If items are not met, resolve them first or document and accept the risk with explicit approval.
- Complete the **Exit Criteria** checklist before transitioning to the next phase. Unresolved items must be tracked as open risks or carry-over work items with owners and due dates.
- The **Project Manager** is responsible for facilitating the gate review; the **Product Manager** and relevant leads must sign off.

---

## Phase 1 — Initiation

### Entry Criteria
- [ ] A problem statement or opportunity has been identified and articulated
- [ ] At least one executive or product sponsor has expressed support
- [ ] A Project Manager and Product Manager have been assigned

### Exit Criteria
- [ ] Project One-pager (problem, goal, SMART success metrics) is complete and shared
- [ ] Stakeholders and champions are identified with a preliminary communication plan
- [ ] High-level timeline and key milestones have been proposed
- [ ] Initial risk list is documented with owners
- [ ] Resource and team needs are estimated
- [ ] Go/no-go decision has been made and recorded (see [Decision Log Template](octoacme-decision-log-template.md))
- [ ] Project board or tracking tool has been created

**Sign-off required from:** Project Sponsor, Product Manager, Project Manager

---

## Phase 2 — Planning

### Entry Criteria
- [ ] Initiation phase exit criteria are complete
- [ ] Go/no-go has been confirmed
- [ ] Core team roles are assigned (including Engineering Manager/Tech Lead, QA lead)

### Exit Criteria
- [ ] Product backlog is prioritized with acceptance criteria on all items planned for the first sprint/milestone
- [ ] Definition of Done is documented and agreed by the team
- [ ] Dependencies (internal and external) are identified and tracked
- [ ] Release timeline and milestones are agreed and visible on the project board
- [ ] Initial test plan / QA approach is drafted and reviewed
- [ ] Security and compliance requirements are identified and reflected in acceptance criteria
- [ ] RACI (Responsible, Accountable, Consulted, Informed) is documented for key decisions and deliverables
- [ ] Risk register is populated with planning-phase risks, mitigations, and owners
- [ ] Planning kickoff held with full core team

**Sign-off required from:** Product Manager, Engineering Manager / Tech Lead, Project Manager

---

## Phase 3 — Execution

### Entry Criteria
- [ ] Planning phase exit criteria are complete
- [ ] Sprint or milestone backlog is ready (prioritized, estimated, and criteria-complete)
- [ ] Development environment and CI/CD pipeline are stable and accessible to all team members
- [ ] Team has reviewed the Definition of Done

### Exit Criteria (per sprint or milestone)
- [ ] All committed backlog items are in `Done` state on the project board or carry-overs are re-planned with owner and revised due date
- [ ] Acceptance criteria have been verified (by QA or defined reviewer) for all completed items
- [ ] CI checks (automated tests, linting, security scanning) are passing on the target branch
- [ ] Code reviews are complete; no outstanding critical review comments on merged PRs
- [ ] Risk register is reviewed and updated; new risks are documented
- [ ] Sprint retrospective has been held and action items are tracked
- [ ] Decisions made during the sprint are logged (see [Decision Log Template](octoacme-decision-log-template.md))

**Sign-off required from:** QA Lead, Engineering Manager / Tech Lead, Project Manager

---

## Phase 4 — Release

### Entry Criteria
- [ ] Execution phase exit criteria are complete for the planned scope
- [ ] Release scope is agreed and frozen (no new scope without explicit change control)
- [ ] Rollback plan is documented and reviewed

### Exit Criteria
- [ ] All acceptance criteria for release scope are verified and signed off by QA
- [ ] CI/CD pipeline is green: automated tests, security scanning, and linting passing
- [ ] Release notes and changelog are authored and reviewed
- [ ] Rollback plan is tested or rehearsed where feasible
- [ ] Post-deploy verification steps are defined and assigned
- [ ] Support team is briefed: known issues, workarounds, and escalation path documented
- [ ] Staged or canary deployment completed (if applicable) with no blocking issues
- [ ] Production deployment completed and post-deploy checks passed
- [ ] Stakeholder release announcement sent

**Sign-off required from:** Product Manager, QA Lead, DevOps / Platform Engineer, Security / Compliance Lead (for security-relevant changes)

---

## Phase 5 — Retrospective & Close

### Entry Criteria
- [ ] Release phase exit criteria are complete
- [ ] Post-deploy monitoring period has elapsed (typically 48–72 hours or as defined per project)

### Exit Criteria
- [ ] Retrospective has been held with the core team
- [ ] Retrospective action items are captured in the project backlog with owners and due dates
- [ ] Lessons learned are documented and shared with relevant stakeholders
- [ ] Risk register is closed or archived with final statuses
- [ ] Decision log is complete and archived with the project record
- [ ] Project documentation is up to date and accessible
- [ ] Success metrics are reviewed against targets; outcome summary is shared with stakeholders
- [ ] Any carry-over work or follow-on projects are initiated through the Initiation phase

**Sign-off required from:** Project Manager, Product Manager

---

## RACI Quick Reference

The table below summarizes accountability across lifecycle phases for common decisions. Customize per project as needed.

| Decision / Activity | PM | PdM | Tech Lead | QA Lead | DevOps | Security | Support |
|---|---|---|---|---|---|---|---|
| Go/no-go (Initiation) | A | C | C | — | — | C | — |
| Scope prioritization | C | A | C | I | I | C | C |
| Architecture choice | C | I | A | I | C | C | — |
| Release sign-off | A | C | C | C | C | C | C |
| Incident escalation | A | I | C | C | C | A | C |
| Retrospective actions | A | C | C | C | C | C | C |

*Key: R = Responsible, A = Accountable, C = Consulted, I = Informed*
*(A single Accountable owner per row is the decision-maker or final approver.)*
