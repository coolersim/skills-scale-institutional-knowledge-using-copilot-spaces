# OctoAcme — Release & Deployment Guide

## Purpose
Standardize how OctoAcme releases features to production to reduce risk and improve observability.

## Release Types
- Patch: hotfixes addressing critical production issues
- Minor: incremental features and improvements
- Major: significant functionality or breaking changes

## Pre-release requirements
- All acceptance criteria met and PRs merged
- Passing CI and security scans
- Release notes drafted
- Rollback / mitigation plan documented
- Smoke tests prepared

## Deployment Checklist
- [ ] Deployment window scheduled (if needed)
- [ ] Backup or snapshot (if applicable)
- [ ] Deploy to staging and run smoke tests
- [ ] Deploy to production (automated pipeline preferred)
- [ ] Run post-deploy verifications
- [ ] Announce release to stakeholders and support

## Rollback & Incident Playbook
- If a deployment fails or causes a critical issue:
  - Trigger incident response and notify on-call
  - Rollback to last known-good release if necessary
  - Triage root cause and capture action items
- **Security incidents**: the Security Lead owns communication and response; escalate immediately per the [Risk Management & Communication Guide](octoacme-risks-and-communication.md).

## Release Notes Template
- Release name / number:
- Date:
- Summary:
- Notable changes:
- Migration steps (if any):
- Known issues:

## Responsibility Summary

| Activity | Accountable |
|---|---|
| Release readiness sign-off | Release Manager |
| Deployment execution | Release Manager |
| Release notes | Technical Writer |
| Security scan approval | Security Lead |
| Customer communications | Customer Success Lead |

For a full breakdown, see the [Ownership & RACI Matrix](octoacme-ownership-and-raci.md).

## Related Templates
- [Release Readiness Checklist](templates/octoacme-release-readiness-checklist.md) — complete before every production deployment
- [Role Handoff Checklist](templates/octoacme-role-handoff-checklist.md) — use when Release Manager or other roles rotate
