# OctoAcme — Release & Deployment Guide

## Purpose
Standardize how OctoAcme releases features to production to reduce risk and improve observability.

## Release Types
- Patch: hotfixes addressing critical production issues
- Minor: incremental features and improvements
- Major: significant functionality or breaking changes

## Release Roles & Responsibilities
- **Project Manager:** Coordinates release timeline and stakeholder communication
- **QA Automation Engineer:** Validates all acceptance criteria met, runs smoke tests, confirms readiness
- **Developers:** Ensure PRs merged, code reviewed, CI passing
- **Security Lead:** Reviews security scan results, approves security changes
- **Customer Success Manager:** Prepares release notes, coordinates customer announcements

## Pre-release requirements
- All acceptance criteria met and PRs merged
- Passing CI (tests, lint, security scans)
- QA Automation Engineer sign-off on test coverage and smoke test results
- Security Lead approval of any security-sensitive changes
- Release notes drafted by Customer Success Manager
- Rollback / mitigation plan documented
- Customer Success Manager confirms customer communication plan

## Deployment Checklist
- [ ] Deployment window scheduled (if needed)
- [ ] Backup or snapshot (if applicable)
- [ ] Deploy to staging and run smoke tests (QA Automation Engineer owns verification)
- [ ] Deploy to production (automated pipeline preferred)
- [ ] Run post-deploy verifications (automated + manual checks)
- [ ] Announce release to stakeholders and support (Customer Success Manager leads)
- [ ] Monitor for issues and escalate to Security Lead if security-related

## Rollback & Incident Playbook
- If a deployment fails or causes a critical issue:
  - Trigger incident response and notify on-call
  - Rollback to last known-good release if necessary
  - Triage root cause and capture action items
  - Security Lead joins if incident involves data or security
  - Customer Success Manager manages external communication

## Release Notes Template
- Release name / number:
- Date:
- Summary:
- Notable changes:
- Migration steps (if any):
- Known issues:
- Security updates (if any):
- Customer impact and value prop: