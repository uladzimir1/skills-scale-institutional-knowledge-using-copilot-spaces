# OctoAcme — Risk Register Template

## Purpose
Provide a consistent format for tracking project risks, their likelihood and impact, mitigation plans, and current status. The Risk Manager owns this register; the Project Manager ensures it is reviewed regularly.

## How to Use
- Add a new row for each identified risk.
- Review the register at every weekly sync and update the **Status** column.
- Escalate any risk rated High/High (Impact × Likelihood) to the Project Manager and sponsor immediately.
- Close risks that have been fully mitigated or are no longer relevant.

---

## Risk Register

| ID | Description | Category | Impact (H/M/L) | Likelihood (H/M/L) | Risk Score | Owner | Mitigation Plan | Contingency Plan | Status | Date Identified | Last Updated |
|----|-------------|----------|:-:|:-:|:-:|-------|-----------------|------------------|--------|----------------|--------------|
| R-001 | _Example: Key dependency team unavailable during sprint_ | Schedule | H | M | High | PM | Identify backup contacts; pre-align on dependencies early | Adjust sprint scope; pull in next-priority items | Open | YYYY-MM-DD | YYYY-MM-DD |

---

## Risk Score Guide

| Impact \ Likelihood | Low | Medium | High |
|---------------------|-----|--------|------|
| **High** | Medium | High | Critical |
| **Medium** | Low | Medium | High |
| **Low** | Low | Low | Medium |

### Thresholds
- **Critical / High**: Escalate to PM and sponsor; weekly review minimum.
- **Medium**: Review at weekly sync; ensure mitigation is in progress.
- **Low**: Monitor; review monthly or at phase transitions.

---

## Risk Categories
- **Schedule** — threats to timeline or milestone delivery
- **Scope** — uncontrolled growth or unclear requirements
- **Resource** — staffing, skills, or budget constraints
- **Technical** — architectural, infrastructure, or integration risks
- **Quality** — test coverage gaps, defect trends, or acceptance criteria issues
- **External** — third-party dependencies, regulatory, or market changes
- **Security** — vulnerabilities, compliance, or data risks

---

## Review Cadence
- **Weekly**: Risk Manager reviews and updates Status and Last Updated columns.
- **Sprint Retrospective**: Evaluate whether any risks materialized and capture learnings.
- **Phase Transitions**: Reassess all open risks before moving to the next lifecycle phase.
