# OctoAcme — Risk Management & Communication

## Purpose
Explain how to identify, manage, and communicate risks and dependencies.

## Risk Register
Maintain a simple table with:
- ID
- Description
- Category (Technical, Schedule, Resource, Security, Quality, Dependency)
- Impact (High/Med/Low)
- Likelihood (High/Med/Low)
- Owner
- Mitigation plan
- Status

## Risk Categories & Owners
- **Technical Risks:** Owned by Developers, escalated to Tech Lead
- **Quality/Testing Risks:** Owned by QA Automation Engineer
- **Security Risks:** Owned by Security Lead, escalated to Security on-call for incidents
- **Schedule/Dependency Risks:** Owned by Project Manager
- **Customer Adoption Risks:** Owned by Customer Success Manager

## Risk Lifecycle
- Identify: during planning and ongoing execution
- Assess: estimate impact and likelihood (with risk owner)
- Mitigate: reduced via actions, contingency plans
- Monitor: review at weekly syncs and update status

## Security Risk & Incident Response
- Security risks are tracked in a separate security risk register
- For security incidents:
  - Notify Security Lead immediately
  - Follow the security incident runbook
  - Coordinate with Security on-call team
  - Conduct blameless post-incident review

## Stakeholder Communication
- Identify stakeholder groups and communication needs:
  - Engineering teams
  - Product & Project Leadership
  - Sales & Support (via Customer Success Manager)
  - Executive sponsors
  - Customers (via Customer Success Manager for product changes)
- Provide regular updates (weekly or milestone-based)
- Use a single source of truth (project README or release doc) for status

## Communication Templates

### Weekly Status Template
- Progress this week:
- Next steps:
- Risks & blockers:
- Quality metrics (test coverage, automation pass rate):
- Security review status:
- Ask / decisions needed:

### Customer-Facing Release Communication (led by Customer Success Manager)
- Release highlights and value proposition
- What changed and why
- How to migrate or upgrade (if applicable)
- Support contacts and resources
- Feedback channel

### Incident Communication
- Triage summary
- Actions being taken
- Expected timeline
- Impact scope
- Post-incident blameless retrospective scheduled

## Escalation Paths
- **Technical/Quality Issues:** Team → Developer Lead → Tech Lead → CTO
- **Project/Schedule Issues:** Team → PM → Product Lead → Sponsor
- **Security Issues:** Team → Security Lead → CISO → Sponsor
- **Customer/Business Impact:** Team → PM → Product Lead → Executive Sponsor
- For cross-functional issues, involve relevant role leads (see octoacme-roles-and-personas.md)