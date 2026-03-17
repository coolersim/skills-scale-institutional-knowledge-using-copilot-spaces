# OctoAcme — Release Readiness Checklist

**Project / Feature:**
**Release version:**
**Target release date:**
**Release Manager:**
**Release type:** ☐ Patch  ☐ Minor  ☐ Major

---

## 1. Code & Quality Gate

| Check | Owner | Status |
|---|---|---|
| All in-scope PRs merged to the release branch | Developers | ☐ |
| CI pipeline passes (build + lint + unit tests) | Developers | ☐ |
| Integration and end-to-end tests pass | Developers / QA | ☐ |
| No open P0/P1 bugs against this release | PM | ☐ |
| Code review completed for all changes | Developers | ☐ |

## 2. Security Review

| Check | Owner | Status |
|---|---|---|
| Security scans (SAST/DAST/dependency) pass | Security Lead | ☐ |
| Outstanding security findings accepted or mitigated | Security Lead | ☐ |
| Secrets scanning shows no exposed credentials | Security Lead | ☐ |
| Penetration test results reviewed (if required) | Security Lead | ☐ |

## 3. Documentation & Release Notes

| Check | Owner | Status |
|---|---|---|
| Release notes drafted and reviewed | Technical Writer | ☐ |
| Public-facing documentation updated (if applicable) | Technical Writer | ☐ |
| Internal runbooks updated | Technical Writer | ☐ |
| Known issues documented | PM / Technical Writer | ☐ |

## 4. Deployment Preparation

| Check | Owner | Status |
|---|---|---|
| Deployment window scheduled and communicated | Release Manager | ☐ |
| Staging environment deployed and smoke-tested | Release Manager / Dev | ☐ |
| Database migrations tested in staging (if applicable) | Developers | ☐ |
| Feature flags configured for phased rollout (if used) | Developers | ☐ |
| Rollback plan documented and tested | Release Manager | ☐ |
| On-call rotation confirmed for release window | PM / Release Manager | ☐ |

## 5. Stakeholder Sign-Off

| Stakeholder | Role | Sign-Off | Date |
|---|---|---|---|
| | Project Manager | ☐ | |
| | Product Manager | ☐ | |
| | Security Lead | ☐ | |
| | Release Manager | ☐ | |
| | Stakeholder Representative | ☐ | |

## 6. Post-Release Plan

| Check | Owner | Status |
|---|---|---|
| Post-deploy verification steps documented | Release Manager | ☐ |
| Customer success / support notified of changes | Customer Success Lead | ☐ |
| Monitoring dashboards and alerts reviewed | Developers | ☐ |
| Retrospective scheduled | PM | ☐ |

---

## Release Decision

**Decision:** ☐ Go  ☐ No-Go  ☐ Conditional Go (conditions listed below)

**Conditions / Outstanding items:**

| # | Item | Owner | Due date |
|---|---|---|---|
| 1 | | | |
| 2 | | | |

**Notes:**

---

*For role ownership details, see [Ownership & RACI Matrix](../octoacme-ownership-and-raci.md) and [Roles & Personas](../octoacme-roles-and-personas.md).*
*For the deployment process, see [Release & Deployment Guide](../octoacme-release-and-deployment.md).*
