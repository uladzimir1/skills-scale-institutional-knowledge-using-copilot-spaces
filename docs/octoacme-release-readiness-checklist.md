# OctoAcme — Release Readiness Checklist

## Purpose
Ensure all necessary steps are completed before deploying a release to production. The Project Manager coordinates this checklist; the QA Lead, Product Manager, and engineering leads contribute sign-offs.

---

## Pre-Release Checklist

### Scope & Requirements
- [ ] All planned features and fixes for this release are complete and meet the Definition of Done.
- [ ] Outstanding P1 and P2 defects are resolved or have an accepted deferral approved by the Product Manager.
- [ ] The Business Analyst has confirmed that release scope matches agreed requirements.
- [ ] Any deferred items are logged in the backlog with documented rationale.

### Code & Build
- [ ] The release branch is created and all release commits are included.
- [ ] CI/CD pipeline is green on the release branch (all checks pass).
- [ ] Code has been reviewed and merged following the PR workflow.
- [ ] No open merge conflicts or unresolved PRs in the release scope.

### Quality Assurance
- [ ] QA checklist completed for all release items (see [QA Checklist](octoacme-qa-checklist.md)).
- [ ] Regression test suite executed; results reviewed and accepted by QA Lead.
- [ ] End-to-end smoke tests pass on the staging environment.
- [ ] QA Lead sign-off obtained.

### Security & Compliance
- [ ] Dependency vulnerability scan complete; no unresolved critical or high issues.
- [ ] Secrets and credentials have not been hardcoded or exposed.
- [ ] Compliance requirements reviewed (data privacy, accessibility, regulatory) if applicable.

### Risk & Change Management
- [ ] Risk register reviewed; no open Critical or High risks without a mitigation plan.
- [ ] All approved Change Requests for this release are implemented and verified.
- [ ] Change Control Coordinator has confirmed no pending unapproved changes.

### Documentation & Communication
- [ ] Release notes are complete, reviewed, and approved.
- [ ] User-facing documentation is updated.
- [ ] Internal runbooks and operational docs are updated (if applicable).
- [ ] Stakeholder communication prepared (announcement, known issues, timeline).

### Deployment Preparation
- [ ] Deployment plan is documented (steps, timing, responsible parties).
- [ ] Rollback plan is documented and validated.
- [ ] Environment variables and configuration reviewed for production.
- [ ] Feature flags set correctly for controlled rollout (if applicable).
- [ ] Operations / on-call team notified and briefed.

### Sign-Offs

| Role | Name | Sign-Off Date | Notes |
|------|------|:-------------:|-------|
| QA Lead | | | |
| Product Manager | | | |
| Project Manager | | | |
| Engineering Lead | | | |
| Risk Manager | | | |

---

## Post-Release Checklist

- [ ] Production deployment completed successfully.
- [ ] Post-deploy smoke tests passed in production.
- [ ] Monitoring dashboards and alerts verified as active.
- [ ] Release notes published to stakeholders.
- [ ] Any issues discovered post-deploy are logged and triaged immediately.
- [ ] Post-release retrospective or follow-up review scheduled (within 5 business days).

---

## Rollback Criteria
Initiate rollback if any of the following occur within the first hour of production deployment:
- Error rate increases above the agreed threshold.
- P1 defect is discovered in production.
- Data integrity issue is detected.
- Core user flow is broken.

The Project Manager and Engineering Lead jointly make the rollback decision. The Change Control Coordinator logs the rollback as a change event.
