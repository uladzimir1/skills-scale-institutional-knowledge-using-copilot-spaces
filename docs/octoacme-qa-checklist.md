# OctoAcme — QA Checklist

## Purpose
Provide a consistent quality gate checklist that the QA Lead and Developers use to validate work before marking items Done and before initiating a release. This checklist complements the Definition of Done.

---

## Per-Story / Per-Feature QA Checklist

### Requirements & Acceptance Criteria
- [ ] Acceptance criteria are clearly documented and understood by the developer and QA Lead.
- [ ] Edge cases and negative paths are identified and covered in test scenarios.
- [ ] Requirements have been reviewed with the Business Analyst or Product Manager.

### Code Quality
- [ ] Code has been reviewed and approved by at least one peer (PR review).
- [ ] No critical or high-severity static analysis / linting issues remain.
- [ ] New code follows existing coding standards and patterns.

### Testing
- [ ] Unit tests cover new logic; existing tests remain green.
- [ ] Integration tests added or updated where applicable.
- [ ] Test cases are documented (e.g., in the PR or test plan).
- [ ] Happy path and key edge cases are covered by automated tests.

### Functional Validation
- [ ] Feature works as expected on the target environment (staging/dev).
- [ ] No known regressions introduced in related functionality.
- [ ] UI/UX changes reviewed against design specifications (if applicable).

### Security & Compliance
- [ ] No hardcoded secrets or credentials introduced.
- [ ] Security scanning in CI passes (no new critical/high vulnerabilities).
- [ ] Data handling follows applicable privacy and compliance requirements.

### Documentation
- [ ] In-code documentation (comments, docstrings) updated where needed.
- [ ] User-facing documentation updated if the feature affects end users.
- [ ] Release notes entry drafted (if applicable).

---

## Pre-Release QA Checklist

### Scope Confirmation
- [ ] All planned features/fixes for this release are complete and in the release branch.
- [ ] Outstanding defects reviewed; P1/P2 issues are resolved or have an accepted deferral.
- [ ] Change log / release notes are complete and reviewed.

### Environment & Build
- [ ] CI build is green on the release branch.
- [ ] Deployment to staging is successful.
- [ ] Configuration and environment variables validated for production.

### Regression Testing
- [ ] Regression test suite executed (automated and/or manual).
- [ ] Smoke test on staging passes for all critical user flows.
- [ ] Performance and load considerations reviewed (if applicable).

### Security
- [ ] Dependency vulnerability scan results reviewed; no unresolved critical issues.
- [ ] Penetration or security review completed (if applicable for release scope).

### Readiness Sign-Off
- [ ] QA Lead sign-off obtained.
- [ ] Product Manager acceptance confirmed.
- [ ] Rollback / mitigation plan documented and communicated.
- [ ] Support and operations teams notified of release scope and timing.

---

## Defect Severity Guide

| Severity | Description | Expected Resolution |
|----------|-------------|---------------------|
| **P1 – Critical** | System down, data loss, or security breach | Must fix before release |
| **P2 – High** | Major feature broken with no workaround | Must fix before release |
| **P3 – Medium** | Feature impaired; workaround available | Target fix in current or next sprint |
| **P4 – Low** | Minor cosmetic or usability issue | Backlog; fix when capacity allows |
