# OctoAcme — Execution & Tracking

## Purpose
Guidance for managing day-to-day execution and tracking progress toward project milestones.

## Team Rhythm
- Daily standups (15 min) — focus on progress, blockers, dependencies
- Weekly delivery sync — show progress, updates, and flagged risks
- Demo/Review at the end of each sprint or milestone

## Workflows
- Use the project board (e.g., GitHub Projects) with columns: Backlog, Ready, In Progress, In Review, QA, Done
- Pull Request workflow:
  - Small PRs (<= 400 lines when possible)
  - Include issue link and acceptance criteria in PR description
  - Run automated tests and linting in CI before requesting review
  - Require at least one approval before merging (or team-defined policy)

## Quality & Testing
- **Unit tests** for new logic — written by Developers with QA Automation Engineer input on coverage goals
- **Integration tests** where applicable — coordinated with QA Automation Engineer
- **End-to-end smoke tests** for critical flows before release — owned by QA Automation Engineer
- **Security scanning** in CI — triggered during PR workflow, escalated to Security Lead if issues found
- **Manual QA** for feature acceptance when needed — coordinated between Developers, QA Automation Engineer, and UX Designer for usability verification
- **Accessibility testing** — led by UX Designer, validated by QA Automation Engineer

## Testing Responsibilities
- **Developers:** Write unit tests, assist with testability, review test failures
- **QA Automation Engineer:** Design test strategy, maintain automation frameworks, set coverage targets, validate readiness
- **UX Designer:** Coordinate usability and accessibility testing
- **Security Lead:** Review security test coverage, escalate findings

## Reporting & Metrics
- Track velocity and burndown
- Monitor success metrics identified in the Project One-pager
- Use dashboards for key signals (errors, latency, usage)
- **Quality metrics:** Test coverage, automation pass rate, defect escape rate
- **Delivery metrics:** Cycle time, PR review time, rollback rate

## Blocker Escalation
- Level 1: Team-level triage in daily standup
- Level 2: PM escalates to Product Lead and dependent teams; escalate security blockers to Security Lead
- Level 3: Sponsor-level escalation for business-impacting issues

## Execution Checklist
- [ ] Branching and PR conventions documented in repo
- [ ] CI configured for tests, lint, and security scanning
- [ ] Test strategy and QA Automation approach documented
- [ ] Regular demos scheduled
- [ ] Risk register updated weekly (including security and quality risks)
- [ ] Accessibility compliance approach defined with UX Designer