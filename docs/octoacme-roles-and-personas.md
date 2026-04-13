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

## Risk Manager

### Role Summary
The Risk Manager is responsible for identifying, evaluating, tracking, and managing project risks throughout the project lifecycle. They work closely with the Project Manager and relevant stakeholders to design and execute mitigation plans that protect project outcomes.

### Responsibilities
- Maintain the project risk register (identification, assessment, mitigation, and status)
- Proactively identify risks during planning, execution, and review phases
- Facilitate risk review meetings and present risk status updates
- Define risk mitigation and contingency plans in collaboration with affected teams
- Escalate high-impact risks to the Project Manager and sponsors
- Track risk owners and ensure mitigation actions are completed on time

### Goals
- Minimize the likelihood and impact of project risks
- Ensure risks are surfaced early, not reactively
- Maintain a clear and up-to-date view of project risk posture

### Typical Communication
- Weekly risk register updates shared with PM and stakeholders
- Risk summary section in status reports
- Ad-hoc escalations for newly identified high-impact risks

### Interaction with Existing Roles
| Role | Interaction |
|------|-------------|
| Project Manager | Reports risk status; co-owns escalation decisions |
| Product Manager | Aligns on risk impact to product scope and timelines |
| Developers | Collects technical risk input; validates mitigation feasibility |
| QA Lead | Coordinates on quality risks and test coverage gaps |
| Change Control Coordinator | Reviews change requests for new or increased risk |

---

## Quality Assurance Lead

### Role Summary
The QA Lead oversees quality standards and testing processes across the project. They coordinate reviews and testing activities, ensure deliverables meet defined acceptance criteria, and champion a quality-first culture within the delivery team.

### Responsibilities
- Define and maintain the team's Definition of Done and QA checklist
- Plan and coordinate testing activities (unit, integration, regression, UAT)
- Review acceptance criteria for completeness and testability before work begins
- Track and report on defect trends, test coverage, and quality metrics
- Coordinate sign-off on releases from a quality perspective
- Work with Developers to embed quality practices throughout development

### Goals
- Ensure that all delivered features meet acceptance criteria and quality standards
- Reduce defect escape rate to production
- Drive continuous improvement of testing practices and tooling

### Typical Communication
- QA status updates in sprint reviews and release readiness meetings
- Defect and test coverage reports
- Collaboration with Developers on test plans and PR reviews

### Interaction with Existing Roles
| Role | Interaction |
|------|-------------|
| Developers | Collaborates on test plans; reviews PRs for test coverage |
| Product Manager | Validates acceptance criteria and UAT requirements |
| Project Manager | Reports QA status and release readiness blockers |
| Risk Manager | Flags quality risks and test coverage gaps |
| Change Control Coordinator | Reviews changes for QA impact and regression risk |

---

## Change Control Coordinator

### Role Summary
The Change Control Coordinator manages all proposed changes to project scope, process, or deliverables. They ensure changes are properly evaluated, approved, communicated, and documented before implementation to protect project stability.

### Responsibilities
- Maintain the change control log and process
- Receive, review, and route change requests for evaluation and approval
- Assess the impact of proposed changes on scope, schedule, cost, and quality
- Facilitate change approval meetings and document decisions
- Communicate approved or rejected changes to all impacted stakeholders
- Monitor the implementation of approved changes and verify completion

### Goals
- Prevent uncontrolled scope creep and unplanned changes
- Ensure all changes are traceable, evaluated, and approved
- Maintain stakeholder alignment when project scope or plans evolve

### Typical Communication
- Change request notifications to relevant stakeholders
- Change log updates shared at planning and status meetings
- Decision summaries and impact assessments for sponsors and leads

### Interaction with Existing Roles
| Role | Interaction |
|------|-------------|
| Project Manager | Collaborates on assessing schedule and resource impact |
| Product Manager | Evaluates scope and priority impact of change requests |
| Risk Manager | Assesses new risks introduced by changes |
| QA Lead | Identifies testing requirements for approved changes |
| Developers | Communicates approved changes for estimation and planning |

---

## Business Analyst

### Role Summary
The Business Analyst acts as the bridge between business stakeholders and technical teams. They gather, analyze, and document requirements, translate stakeholder needs into clear and actionable work items, and ensure shared understanding across the project.

### Responsibilities
- Elicit and document business and functional requirements from stakeholders
- Translate business needs into user stories, acceptance criteria, and process flows
- Facilitate requirements workshops and review sessions
- Validate that delivered solutions meet documented requirements
- Maintain traceability between business objectives and backlog items
- Support the Product Manager in backlog refinement and prioritization

### Goals
- Ensure requirements are complete, unambiguous, and agreed upon before work begins
- Reduce rework caused by misunderstood or incomplete requirements
- Maintain clear communication and shared understanding across business and technical teams

### Typical Communication
- Requirements workshops and stakeholder interviews
- User stories, acceptance criteria, and process documentation
- Regular check-ins with Product Manager and Developers during delivery

### Interaction with Existing Roles
| Role | Interaction |
|------|-------------|
| Product Manager | Supports roadmap and backlog refinement; validates priorities |
| Developers | Clarifies requirements; answers questions during implementation |
| Project Manager | Flags scope and requirements risks; contributes to planning |
| QA Lead | Provides acceptance criteria and supports UAT planning |
| Change Control Coordinator | Documents requirements changes triggered by change requests |

---

## RACI Summary

The table below provides a high-level RACI (Responsible, Accountable, Consulted, Informed) mapping across key project activities for all defined roles.

| Activity | Project Manager | Product Manager | Developer | QA Lead | Risk Manager | Change Control Coordinator | Business Analyst |
|----------|:-:|:-:|:-:|:-:|:-:|:-:|:-:|
| Project planning & scheduling | A/R | C | C | C | C | C | C |
| Backlog prioritization | C | A/R | C | C | I | I | R |
| Requirements definition | I | A | I | C | I | I | R |
| Risk identification & tracking | C | I | C | I | A/R | C | C |
| Change request evaluation | A/R | C | C | C | C | R | C |
| Test planning & QA | I | C | R | A/R | C | I | C |
| Release readiness sign-off | A/R | C | R | R | C | C | I |
| Stakeholder communication | A/R | R | I | I | C | C | C |
| Retrospectives | A/R | R | R | R | R | R | R |

**Key:** R = Responsible, A = Accountable, C = Consulted, I = Informed

---

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.

