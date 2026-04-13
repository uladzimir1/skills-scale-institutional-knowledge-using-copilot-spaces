# OctoAcme — Definition of Done

## Purpose
Establish a shared, explicit agreement on what "Done" means for backlog items and releases. The QA Lead and Product Manager maintain this document; the entire team is accountable for applying it.

---

## Definition of Done — Story / Task Level

A backlog item is **Done** when all of the following are true:

### Development
- [ ] All acceptance criteria specified in the issue/story are met.
- [ ] Code is written, reviewed, and merged to the main branch via an approved PR.
- [ ] No unresolved review comments on the merged PR.

### Testing
- [ ] Unit tests pass in CI (no new failures).
- [ ] Integration tests pass in CI (where applicable).
- [ ] Acceptance tests / manual verification performed against acceptance criteria.
- [ ] No P1 or P2 defects open against this item.

### Quality & Security
- [ ] Code passes static analysis and linting checks in CI.
- [ ] Security scan returns no new critical or high vulnerabilities.
- [ ] No hardcoded secrets or credentials introduced.

### Documentation & Communication
- [ ] Code comments and inline documentation are up to date.
- [ ] Relevant process or user documentation updated (if applicable).
- [ ] Release notes entry created (if this item is user-facing).

### Deployment Readiness
- [ ] Feature is deployable to staging; smoke test passes.
- [ ] Feature flag / configuration is ready if a controlled rollout is planned.

---

## Definition of Done — Sprint / Iteration Level

A sprint is **Done** when:

- [ ] All committed items meet the story-level DoD above.
- [ ] Sprint demo has been conducted and recorded.
- [ ] Any unfinished items have been triaged (deferred, rescoped, or carried over with a documented reason).
- [ ] Sprint retrospective has been held and action items are captured in the backlog.
- [ ] Risk register has been reviewed and updated.

---

## Definition of Done — Release Level

A release is **Done** when:

- [ ] All items in the release scope meet the story-level DoD.
- [ ] Full regression suite passes on the staging environment.
- [ ] QA Lead and Product Manager have signed off.
- [ ] Release notes are finalized and available.
- [ ] Production deployment is complete and post-deploy verification has passed.
- [ ] Monitoring and alerting are confirmed active.
- [ ] Support and operations teams have been notified.
- [ ] Rollback plan has been documented and tested (where applicable).
- [ ] Post-release retrospective or follow-up review is scheduled.

---

## Updating This Document
The Definition of Done should be reviewed at the start of each major project or at least once per quarter. Proposed changes are submitted as a Change Request to the Change Control Coordinator and must be approved by the QA Lead and Product Manager before taking effect.
