# OctoAcme — Risk Management & Communication

## Purpose
Explain how to identify, manage, and communicate risks and dependencies.

## Risk Register
Maintain a simple table with:
- ID
- Description
- Impact (High/Med/Low)
- Likelihood (High/Med/Low)
- Owner
- Mitigation plan
- Status

## Risk Lifecycle
- Identify: during planning and ongoing execution
- Assess: estimate impact and likelihood
- Mitigate: reduced via actions, contingency plans
- Monitor: review at weekly syncs and update status

## Stakeholder Communication
- Identify stakeholder groups and communication needs (e.g., engineering, sales, support)
- Provide regular updates (weekly or milestone-based)
- Use a single source of truth (project README or release doc) for status

## Communication Templates
Weekly Status Template:
- Progress this week:
- Next steps:
- Risks & blockers:
- Ask / decisions needed:

Incident Communication
- Triage summary
- Actions being taken
- Expected timeline
- Post-incident blameless retrospective scheduled

## Escalation Paths
- Team-level -> PM -> Product Lead -> Sponsor
- For security incidents, follow the security incident runbook and notify the **Security Lead** immediately; the Security Lead owns incident communication and coordinates with the PM and Stakeholder Representative.

## Related Templates & Guides
- [Risk Register Template](templates/octoacme-risk-register-template.md) — use for ongoing risk tracking and weekly updates
- [Weekly Status Update Template](templates/octoacme-weekly-status-update-template.md) — includes risks & blockers section for stakeholder reporting
- [Ownership & RACI Matrix](octoacme-ownership-and-raci.md) — clarifies risk and escalation ownership by role
- [Roles & Personas](octoacme-roles-and-personas.md) — see Security Lead, PM, and Stakeholder Representative for escalation participants
