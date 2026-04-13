# OctoAcme Project Management Docs

## Overview

OctoAcme's project management approach follows a lightweight, end-to-end lifecycle: **Initiation → Planning → Execution → Release → Close & Retrospective**. The process starts with validating the business need and success criteria via a Project One-pager (problem, SMART objective, success metrics), aligning stakeholders and resourcing, and making a clear go/no-go decision before investing in detailed planning. Once approved, the team turns the initiative into an actionable plan by running a kickoff, creating a prioritized and estimated backlog with acceptance criteria, defining a Definition of Done, and mapping milestones, dependencies, and a release plan.

Roles and ownership are intentionally explicit to keep delivery moving. A **Project Manager (PM)** coordinates delivery mechanics—schedules, risks, dependencies, and communications—while the **Product Manager (PdM)** owns outcomes, prioritization, and measurement of success. **Developers** design and implement changes with testability and maintainability in mind, and **QA/Testing** validates acceptance criteria and overall product quality. Stakeholders provide inputs and approvals, and the team maintains key artifacts (charter/one-pager, roadmap/release plan, iteration backlog, risk register, retrospective action items) as a shared source of truth. Day-to-day delivery relies on a disciplined project board (columns: Backlog → Ready → In Progress → In Review → QA → Done) and a PR workflow where small, issue-linked PRs pass CI checks and required approvals before merging.

Communication is built around a consistent cadence and clear escalation paths. The team maintains regular standups, weekly delivery syncs, sprint demos, and a weekly PM + PdM sync, with monthly stakeholder updates on an agreed schedule. Risks and dependencies are tracked in a **risk register** (impact, likelihood, owner, mitigation, status) and reviewed weekly; when blockers persist, escalation proceeds from team triage → PM → Product Lead → Sponsor for business-impacting issues. Status updates are structured around progress, next steps, risks/blockers, and asks/decisions to keep communication actionable.

Quality assurance is embedded throughout execution and release, not treated as a final gate. Testing expectations scale with the change: unit tests for new logic, integration tests where applicable, end-to-end smoke tests for critical flows, security scanning in CI, and manual QA when needed for feature acceptance. Releases require readiness checks (criteria met, CI green, release notes drafted, rollback/mitigation planned), staged validation (staging + smoke tests), post-deploy verification, and a **retrospective** that converts learnings into owned action items with due dates and measurable success criteria tracked back into the backlog.

## Process Documents

- [Project Management Overview](octoacme-project-management-overview.md)
- [Project Initiation Guide](octoacme-project-initiation.md)
- [Project Planning](octoacme-project-planning.md)
- [Execution & Tracking](octoacme-execution-and-tracking.md)
- [Risks & Communication](octoacme-risks-and-communication.md)
- [Release & Deployment](octoacme-release-and-deployment.md)
- [Retrospective & Continuous Improvement](octoacme-retrospective-and-continuous-improvement.md)
- [Roles & Personas](octoacme-roles-and-personas.md)

## Templates & Checklists

- [Risk Register Template](octoacme-risk-register-template.md)
- [Change Control Log](octoacme-change-control-log.md)
- [QA Checklist](octoacme-qa-checklist.md)
- [Definition of Done](octoacme-definition-of-done.md)
- [Release Readiness Checklist](octoacme-release-readiness-checklist.md)
