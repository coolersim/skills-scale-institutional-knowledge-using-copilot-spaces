# OctoAcme — Ownership & RACI Matrix

## Purpose
Clarify who is **Responsible**, **Accountable**, **Consulted**, and **Informed** for key activities across the project lifecycle. Use this matrix to resolve ownership ambiguity and ensure smooth handoffs between roles.

## RACI Key

| Letter | Meaning |
|--------|---------|
| **R** | **Responsible** — does the work |
| **A** | **Accountable** — ultimate decision-maker; one per activity |
| **C** | **Consulted** — provides input before or during the work |
| **I** | **Informed** — notified of outcome or progress |

## Roles Reference

| Abbreviation | Role |
|---|---|
| PM | Project Manager |
| PdM | Product Manager |
| Dev | Developers |
| RM | Release Manager |
| SL | Security Lead |
| TW | Technical Writer |
| SR | Stakeholder Representative |
| CS | Customer Success Lead |

For full role descriptions see [Roles & Personas](octoacme-roles-and-personas.md).

---

## RACI Matrix

### Initiation

| Activity | PM | PdM | Dev | RM | SL | TW | SR | CS |
|---|---|---|---|---|---|---|---|---|
| Define problem statement & goal | C | **A/R** | C | — | — | — | C | C |
| Identify stakeholders | **A/R** | C | — | — | — | — | **R** | C |
| Draft project one-pager | **R** | **A** | C | — | — | C | I | I |
| Initial risk identification | **A/R** | C | C | — | **R** | — | I | — |
| Go / No-Go decision | C | **A** | — | — | — | — | C | — |

---

### Planning

| Activity | PM | PdM | Dev | RM | SL | TW | SR | CS |
|---|---|---|---|---|---|---|---|---|
| Define scope & milestones | **A/R** | **R** | C | C | — | — | C | I |
| Break work into backlog items | C | **A** | **R** | — | — | — | I | — |
| Estimate effort | C | C | **A/R** | — | — | — | — | — |
| Define release strategy | C | C | C | **A/R** | C | — | I | I |
| Security & compliance review | **I** | I | C | I | **A/R** | — | — | — |
| Document plan & artifacts | C | C | C | I | I | **A/R** | I | I |

---

### Execution & Tracking

| Activity | PM | PdM | Dev | RM | SL | TW | SR | CS |
|---|---|---|---|---|---|---|---|---|
| Daily standup facilitation | **A/R** | I | **R** | I | — | — | — | — |
| Blocker escalation (Level 1–2) | **A/R** | C | C | I | C | — | I | — |
| Weekly status reporting | **A/R** | C | I | I | I | I | I | I |
| Risk register updates | **A/R** | C | C | I | **R** | — | I | — |
| Code review & quality | I | — | **A/R** | — | C | — | — | — |
| Security scan review | I | — | C | I | **A/R** | — | — | — |
| Documentation updates | C | C | C | I | I | **A/R** | — | — |

---

### Release & Deployment

| Activity | PM | PdM | Dev | RM | SL | TW | SR | CS |
|---|---|---|---|---|---|---|---|---|
| Release readiness sign-off | C | C | C | **A** | **R** | I | I | I |
| Deployment execution | I | — | **R** | **A** | I | — | — | — |
| Release notes | I | **R** | C | C | — | **A/R** | I | I |
| Stakeholder release announcement | C | C | — | C | — | C | **A** | **R** |
| Post-deploy verification | I | — | **R** | **A/R** | C | — | — | — |
| Customer onboarding / comms | I | I | — | I | — | C | C | **A/R** |

---

### Risk Escalation & Incident Communication

| Activity | PM | PdM | Dev | RM | SL | TW | SR | CS |
|---|---|---|---|---|---|---|---|---|
| Incident detection & triage | **R** | I | **R** | C | **A/R** | — | I | I |
| Incident communication (internal) | **A/R** | I | C | C | **R** | — | I | — |
| Customer-facing incident notice | C | C | — | I | C | I | **R** | **A/R** |
| Rollback decision | C | C | C | **A** | C | — | I | I |
| Post-incident retrospective | **A/R** | C | **R** | C | **R** | **R** | I | I |

---

### Retrospectives & Continuous Improvement

| Activity | PM | PdM | Dev | RM | SL | TW | SR | CS |
|---|---|---|---|---|---|---|---|---|
| Retrospective facilitation | **A/R** | C | **R** | C | C | C | I | I |
| Capture action items | **A/R** | C | C | C | C | **R** | I | I |
| Process documentation updates | C | C | C | I | I | **A/R** | — | — |
| Stakeholder feedback review | C | **A/R** | — | — | — | — | **R** | **R** |

---

## Usage Notes
- **One Accountable per row**: if multiple roles share accountability, clarify the primary owner in the project plan.
- **Keep it current**: review this matrix at project kickoff and after any significant team or scope change.
- For role-handoff details, use the [Role Handoff Checklist](templates/octoacme-role-handoff-checklist.md).
- For risk tracking, use the [Risk Register Template](templates/octoacme-risk-register-template.md).
