# OctoAcme — Handoff Checklist

## Purpose
Ensure that knowledge, context, and accountability transfer cleanly at critical transition points in the project lifecycle. Clear handoffs reduce information loss, prevent duplicate work, and keep the downstream team unblocked.

## When to Use
Use the relevant section of this checklist at each of the following transitions:

1. **Initiation → Planning**: strategy and goals pass from sponsors/PdM to the delivery team
2. **Planning → Execution**: planned backlog and design artifacts pass from PM/PdM/Tech Lead to the delivery team
3. **Execution → Release**: completed, tested work passes from the delivery team to the release/deployment process
4. **Release → Retrospective & Close**: production state and outcomes pass from the release team to close activities

The **Project Manager** is responsible for facilitating each handoff review. Both the sending and receiving parties must confirm readiness before the transition is finalized.

---

## Handoff 1: Initiation → Planning

**From:** Project Sponsor, Product Manager  
**To:** Project Manager, Engineering Manager / Tech Lead, full core team

### Checklist

**Context & Goals**
- [ ] Project One-pager has been shared with the full planning team
- [ ] Problem statement, success metrics, and measurable outcomes are understood by all leads
- [ ] Stakeholder map and communication plan are shared and confirmed

**Scope & Constraints**
- [ ] High-level scope boundaries (in-scope vs. explicitly out-of-scope) are communicated
- [ ] Known constraints (budget, timeline, technology, compliance) are documented and shared
- [ ] Key dependencies (external teams, vendors, third-party APIs) are identified

**Risks & Decisions**
- [ ] Initial risk list is handed over with assigned owners
- [ ] Any go/no-go conditions or contingencies are communicated
- [ ] Decision log is seeded with any decisions already made during initiation

**Operational Readiness**
- [ ] Project tracking tool / board is set up and access is granted to the core team
- [ ] Communication channels (Slack workspace, email list, recurring meetings) are established
- [ ] Handoff confirmed by: Project Sponsor ☐ | Product Manager ☐ | Project Manager ☐

---

## Handoff 2: Planning → Execution

**From:** Product Manager, Project Manager, Engineering Manager / Tech Lead  
**To:** Development team, QA Lead, DevOps / Platform Engineer

### Checklist

**Backlog & Acceptance Criteria**
- [ ] Sprint or milestone backlog is finalized, prioritized, and visible on the project board
- [ ] Acceptance criteria are written and reviewed for all items entering the first sprint
- [ ] Definition of Done is documented and agreed by all contributors

**Design & Technical Artifacts**
- [ ] UX wireframes or design specs are available for items requiring UI work
- [ ] Architecture decisions and design docs are shared (link ADRs or design records)
- [ ] Security and compliance requirements are reflected in acceptance criteria or linked tickets

**Environments & Tooling**
- [ ] Development and staging environments are accessible and stable
- [ ] CI/CD pipeline is configured and passing on the baseline branch
- [ ] Repository access, branching conventions, and PR review policy are communicated

**Test Plan**
- [ ] Initial test plan or QA approach document is shared with QA Lead
- [ ] Test data and environment requirements are identified

**Risk & Dependency Awareness**
- [ ] Risk register is reviewed with the delivery team; owners are confirmed
- [ ] External dependencies and their owners are communicated to the team
- [ ] Handoff confirmed by: Product Manager ☐ | Engineering Manager / Tech Lead ☐ | QA Lead ☐ | DevOps ☐

---

## Handoff 3: Execution → Release

**From:** Development team, QA Lead  
**To:** DevOps / Platform Engineer, Project Manager, Security / Compliance Lead, Customer Support / Operations Representative

### Checklist

**Scope Confirmation**
- [ ] Release scope is agreed, documented, and frozen (change control applied to any additions)
- [ ] All items in release scope are in `Done` state with acceptance criteria verified
- [ ] Any items descoped from the release are re-planned or documented as carry-overs

**Quality & Security Gates**
- [ ] CI/CD pipeline is green: automated tests, linting, security scanning passing
- [ ] QA sign-off is documented for all release-scope items
- [ ] Security / Compliance Lead has reviewed and signed off on security-relevant changes
- [ ] No critical or high-severity open bugs in release scope (or exceptions are documented and accepted)

**Release Artifacts**
- [ ] Release notes and changelog are complete and reviewed
- [ ] Rollback plan is documented, reviewed, and (if feasible) rehearsed
- [ ] Deployment runbook is up to date and accessible to DevOps
- [ ] Feature flags or staged rollout configuration is confirmed (if applicable)

**Support Readiness**
- [ ] Known issues and workarounds are documented and shared with the Support Representative
- [ ] Support team has been briefed on new features, changes, and expected customer impact
- [ ] Escalation path for post-release issues is defined and communicated

**Monitoring & Observability**
- [ ] Key metrics and alerting thresholds are configured for the new release
- [ ] Post-deploy verification steps are defined and assigned to owners
- [ ] Handoff confirmed by: QA Lead ☐ | Tech Lead ☐ | DevOps ☐ | Security Lead ☐ | Support Rep ☐

---

## Handoff 4: Release → Retrospective & Close

**From:** DevOps / Platform Engineer, Project Manager  
**To:** Full team, Product Manager, Stakeholders

### Checklist

**Deployment Confirmation**
- [ ] Production deployment is complete and post-deploy verification steps passed
- [ ] Monitoring and alerting are active; no unresolved critical alerts in the first 48–72 hours
- [ ] Rollback procedure was not triggered, or if triggered, root cause is documented

**Outcome Measurement**
- [ ] Success metrics are being collected as expected (validated by Data Analyst / Analytics Owner)
- [ ] Initial outcome data is available for the retrospective discussion
- [ ] Stakeholder release announcement has been sent

**Documentation Close-out**
- [ ] All project documentation is up to date (risk register, decision log, runbooks)
- [ ] Retrospective is scheduled with the core team within one week of release
- [ ] Lessons learned template is distributed to team members before the retrospective

**Transition to Improvement**
- [ ] Carry-over work items and known issues are added to the backlog with owners
- [ ] Follow-on project or next-phase work is initiated through the Initiation phase if applicable
- [ ] Handoff confirmed by: Project Manager ☐ | Product Manager ☐ | DevOps ☐

---

## Handoff Health Checklist (all transitions)

Use the following quick check at any handoff to assess quality:

- [ ] The receiving team can describe the project goals, scope, and success metrics without referring to the sending team
- [ ] All open risks have a named owner on the receiving side
- [ ] No items are blocked waiting for information that should have been provided in this handoff
- [ ] Open decisions are logged with an expected resolution date
- [ ] Both sending and receiving parties agree the handoff is complete

If any of the above are unchecked, resolve them before finalizing the transition.
