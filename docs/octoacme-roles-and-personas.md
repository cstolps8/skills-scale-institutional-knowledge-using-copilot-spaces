# OctoAcme Personas

This document defines typical roles and responsibilities used in OctoAcme project docs and exercises.

---

## Developers

### Role Summary
Developers design, build, test, and deliver software components. They collaborate with product and project leads to implement features that meet acceptance criteria and quality standards.

### Responsibilities
- Implement features and fixes to meet acceptance criteria
- Write and maintain tests and documentation
- Participate in design and code reviews
- Assist in estimating and planning work
- Help identify technical risks and propose mitigations

### Goals
- Deliver reliable, maintainable code
- Reduce cycle time from idea to production
- Maintain high test coverage and observability

### Typical Communication
- Daily standups and sprint planning
- PR descriptions and code review comments
- Technical design docs when needed

---

## Product Managers

### Role Summary
Product Managers define what should be built to deliver customer and business value. They own the product vision, prioritize the backlog, and measure outcomes.

### Responsibilities
- Define problem statements and success metrics
- Prioritize the roadmap and backlog
- Collaborate with stakeholders and engineering on trade-offs
- Validate solutions through user research and metrics

### Goals
- Maximize customer value and impact
- Make clear, data-driven prioritization decisions
- Ensure product-market fit and usability

### Typical Communication
- Weekly alignment with PM and engineering leads
- Roadmap updates and stakeholder briefings
- Acceptance criteria and feature specs

---

## Project Managers

### Role Summary
Project Managers coordinate delivery activities, manage schedules, risks, and communications. They enable the team to deliver on commitments efficiently.

### Responsibilities
- Create and maintain project plans and timelines
- Manage risks, dependencies, and resource constraints
- Facilitate meetings (kickoff, planning, retrospectives)
- Ensure consistent project documentation and status reporting
- Coordinate cross-team and stakeholder communication

### Goals
- Deliver projects on time and within scope
- Minimize unplanned work and escalations
- Maintain transparency and alignment across stakeholders

### Typical Communication
- Weekly status updates and stakeholder reports
- Risk registers and decision logs
- Coordination via project boards and meeting facilitation

---

---

## Engineering Manager / Tech Lead

### Role Summary
The Engineering Manager or Tech Lead provides technical direction, ensures architectural quality, and supports team growth. They bridge the gap between product goals and engineering execution, acting as the primary escalation point for technical risks and capacity concerns.

### Responsibilities
- Define and enforce architecture guardrails and coding standards
- Lead estimation efforts and validate technical feasibility of planned work
- Manage technical dependencies within and across teams
- Mentor and support developer growth and code quality
- Escalate unresolvable technical blockers to leadership

### Goals
- Maintain a healthy, sustainable technical foundation
- Reduce technical debt and unplanned work from poor design choices
- Enable the team to deliver with confidence and predictability

### Typical Communication
- Weekly sync with Product Manager on scope trade-offs and technical constraints
- Architecture decision records (ADRs) and design review sessions
- Engineering retrospectives and post-incident reviews

### Interactions with Existing Roles
- **Developers**: guides implementation choices, leads code and design reviews, unblocks technical decisions
- **Product Managers**: aligns on build vs. buy trade-offs, technical scope, and feasibility
- **Project Managers**: surfaces and escalates technical risks and dependency issues; contributes to risk register

---

## UX / UI Designer

### Role Summary
UX/UI Designers own user flows, interaction design, visual specifications, and accessibility standards. They translate product requirements into designs that Developers can implement with high fidelity, and they ensure the resulting experience meets user needs.

### Responsibilities
- Create wireframes, prototypes, and detailed design specifications
- Conduct or coordinate user research and usability testing
- Define and apply accessibility and usability standards
- Maintain a shared design system and component library
- Review implemented features against design specs before QA sign-off

### Goals
- Deliver intuitive, accessible, and consistent user experiences
- Reduce rework caused by ambiguous or late design input
- Ensure design decisions are traceable to user needs and success metrics

### Typical Communication
- Design reviews and prototype walkthroughs with the team
- Annotated design files shared in a collaborative design tool (e.g., Figma)
- Usability findings and accessibility audit reports

### Interactions with Existing Roles
- **Product Managers**: translates outcome requirements into user flows; aligns on prioritization of UX improvements
- **Developers**: delivers specs and answers implementation questions; reviews shipped work for fidelity
- **QA/Testing**: informs usability acceptance criteria; participates in exploratory testing for UX issues

---

## DevOps / Platform Engineer

### Role Summary
DevOps and Platform Engineers own the reliability, speed, and security of the software delivery pipeline and production environment. They enable the team to ship confidently and frequently by ensuring robust CI/CD, stable environments, and strong observability.

### Responsibilities
- Design, maintain, and improve CI/CD pipelines and deployment automation
- Manage environment provisioning, configuration, and infrastructure as code
- Establish and monitor observability baselines (logging, metrics, alerting)
- Coordinate deployment windows and manage rollback capabilities
- Enforce security and compliance controls at the platform level

### Goals
- Maximize deployment frequency and minimize mean time to recovery (MTTR)
- Eliminate manual, error-prone steps from the release process
- Ensure all environments (dev, staging, production) are stable and consistent

### Typical Communication
- Release readiness coordination meetings with Project Manager and QA
- Pipeline and environment status via dashboards and alert notifications
- Infrastructure change logs and runbooks

### Interactions with Existing Roles
- **Developers**: provides platform tooling and support; reviews infrastructure changes in PRs
- **Project Managers**: advises on deployment risk, maintenance windows, and rollback planning
- **QA/Testing**: ensures test environments are stable and representative of production

---

## Security / Compliance Lead

### Role Summary
The Security/Compliance Lead owns threat assessment, security control guidance, compliance checkpoints, and incident preparedness. They integrate security and compliance considerations into every phase of the delivery lifecycle rather than treating them as a final gate.

### Responsibilities
- Conduct threat modeling and security risk assessments for new features and architecture
- Define and communicate security control requirements and acceptance criteria
- Review code and infrastructure changes for security implications
- Lead compliance checkpoint reviews (e.g., GDPR, SOC 2, internal policies)
- Maintain and rehearse the security incident response plan

### Goals
- Reduce the likelihood and impact of security incidents
- Ensure compliance obligations are met without slowing delivery unnecessarily
- Build a security-aware culture across the engineering team

### Typical Communication
- Security review findings documented and tracked as issues or risk register items
- Pre-release security sign-off confirmation
- Incident reports and post-incident action items

### Interactions with Existing Roles
- **Developers / Tech Lead**: reviews implementation for secure coding practices; provides threat model guidance early in design
- **Project Managers**: contributes security risks to the risk register; informs escalation planning for security incidents
- **Product Managers**: communicates compliance constraints that affect scope, timelines, or feature design

---

## Customer Support / Operations Representative

### Role Summary
The Customer Support or Operations Representative bridges the gap between production users and the delivery team. They surface real customer pain points, ensure the team is prepared to support a release, and close the post-release feedback loop.

### Responsibilities
- Collect, synthesize, and prioritize customer-reported pain points and operational issues
- Validate support readiness before releases (runbooks, known issues, training)
- Document workarounds and known issues for the support team
- Relay post-release feedback and incident patterns back to Product and Engineering
- Coordinate rollback or hotfix decisions when customer impact is severe

### Goals
- Reduce customer-impacting incidents and response time
- Ensure the team ships with a clear support plan and rollback path
- Translate operational signals into actionable product improvements

### Typical Communication
- Pre-release support readiness reviews
- Known-issue and workaround documentation for the support knowledge base
- Post-release incident and feedback summaries shared with Product Manager and Project Manager

### Interactions with Existing Roles
- **Product Managers**: provides prioritized customer pain points to inform backlog decisions
- **Project Managers**: surfaces rollout risks; coordinates communication plans for known issues
- **Developers**: supplies reproduction details, environment context, and customer-impact data for bug investigation

---

## Data Analyst / Analytics Owner

### Role Summary
Data Analysts and Analytics Owners define what must be measured, validate that instrumentation is correct, and deliver post-release insights that drive data-informed decisions. They ensure success metrics are tracked and actionable.

### Responsibilities
- Partner with Product Managers to define KPIs, success metrics, and instrumentation requirements
- Validate that event tracking and analytics implementations are accurate and complete
- Build and maintain dashboards and reports for project and product health
- Publish post-release impact analyses and A/B test results
- Identify data quality issues and work with Engineering to resolve them

### Goals
- Ensure every project has measurable, tracked success criteria
- Reduce the time from release to validated outcome measurement
- Make data accessible and actionable for all decision-makers

### Typical Communication
- Metric definition documents shared before development begins
- Dashboard and report links included in release notes and retrospective materials
- Post-release analysis summaries for stakeholder updates

### Interactions with Existing Roles
- **Product Managers**: co-defines KPIs and ensures metric plans are reflected in acceptance criteria
- **Developers**: specifies event tracking requirements; reviews and validates instrumentation implementations
- **Stakeholders**: delivers outcome insights and impact analyses to support investment decisions

---

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.
- When modeling cross-functional decisions, consider how each persona's goals, responsibilities, and communication patterns interact — especially during handoffs between lifecycle phases.

