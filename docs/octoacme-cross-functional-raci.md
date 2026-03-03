# OctoAcme — Cross-Functional RACI & Handoff Guide

## Purpose
Clarify which roles are Responsible, Accountable, Consulted, or Informed at each phase of the project lifecycle, and provide handoff checklists for key milestones.

For role definitions, see [Roles and Personas](octoacme-roles-and-personas.md).

---

## RACI Key

| Symbol | Meaning |
|--------|---------|
| **R** | **Responsible** — does the work |
| **A** | **Accountable** — owns the outcome; final decision-maker |
| **C** | **Consulted** — provides input before decisions are made |
| **I** | **Informed** — notified of progress or decisions |

---

## Role-to-Ceremony Matrix

| Activity / Phase | Project Manager | Product Manager | Developer | UX Designer | Data Analyst | Technical Writer | Customer Support | Security Lead |
|---|---|---|---|---|---|---|---|---|
| **Initiation** | | | | | | | | |
| Define problem statement & goals | C | A/R | C | C | C | I | C | C |
| Stakeholder identification | A/R | C | I | I | I | I | C | C |
| Initial risk & security assessment | R | C | C | I | I | I | I | A/R |
| Go/no-go decision | A | R | C | C | C | I | I | C |
| **Planning** | | | | | | | | |
| Kickoff meeting facilitation | A/R | R | R | R | R | I | I | C |
| Backlog creation & prioritization | C | A/R | C | C | C | I | C | C |
| Analytics & success metrics definition | C | A | C | C | A/R | I | I | I |
| Design specs & prototypes | I | C | C | A/R | I | I | I | I |
| Documentation plan | C | C | C | C | I | A/R | C | I |
| Security & compliance requirements | C | C | C | I | I | I | I | A/R |
| **Execution** | | | | | | | | |
| Feature implementation | C | C | A/R | C | C | I | I | C |
| Security scanning & code review | I | I | R | I | I | I | I | A/R |
| Instrumentation & analytics setup | I | C | R | I | A/R | I | I | I |
| UX implementation validation | I | C | C | A/R | I | I | I | I |
| Documentation drafting | I | C | C | C | I | A/R | C | I |
| Support feedback triage | I | R | C | I | C | C | A/R | I |
| Risk register updates | A/R | C | C | I | I | I | I | C |
| **Release** | | | | | | | | |
| Release notes authorship | R | C | C | I | I | A/R | C | I |
| Support readiness sign-off | C | C | I | I | I | C | A/R | I |
| Security sign-off | C | C | C | I | I | I | I | A/R |
| Release communication | A/R | R | I | I | I | I | R | I |
| **Retrospective** | | | | | | | | |
| Retrospective facilitation | A/R | C | R | C | C | I | C | C |
| Metrics & outcome review | C | A | C | C | R | I | C | I |
| Process improvement actions | A/R | C | C | C | C | C | C | C |

---

## Handoff Checklists

### Kickoff Handoff (Initiation → Planning)

Before moving from initiation to planning, confirm the following:

- [ ] Problem statement and success metrics reviewed and approved by Product Manager
- [ ] Stakeholder list confirmed and communication plan drafted by Project Manager
- [ ] Initial risk register created; Security Lead consulted for security/compliance items
- [ ] UX Designer briefed on user research needs and design scope
- [ ] Data Analyst aligned on analytics requirements and tracking strategy
- [ ] Technical Writer aware of documentation scope
- [ ] Customer Support Representative consulted on known user pain points
- [ ] Go/no-go decision recorded and communicated to the team

### Release Readiness Handoff (Execution → Release)

Before deploying to production, confirm the following:

- [ ] All acceptance criteria met and PRs merged
- [ ] CI passing, including automated security scans (Security Lead sign-off)
- [ ] UX Designer has validated final implementation against design specs
- [ ] Data Analyst confirms instrumentation is in place and dashboards are ready
- [ ] Technical Writer has completed and reviewed release notes and feature docs
- [ ] Customer Support Representative confirms support docs and FAQs are updated
- [ ] Customer Support Representative confirms support tooling is ready for the release
- [ ] Rollback plan documented
- [ ] Stakeholder release communication drafted (Project Manager or Product Manager)

### Post-Release Handoff (Release → Retrospective)

After deploying, confirm the following:

- [ ] Post-deploy verification completed and release announced to stakeholders
- [ ] Data Analyst monitoring dashboards for anomalies in the first 24–48 hours
- [ ] Customer Support Representative tracking first-day/first-week issues
- [ ] Security Lead monitoring for security anomalies or incident reports
- [ ] Retrospective scheduled within one sprint/cycle of release
- [ ] Metrics and outcome data gathered by Data Analyst for retrospective review
- [ ] Action items from incident or support trends captured for the next planning cycle

---

## When to Involve Which Role

Use this guide to answer "who should I loop in?" at a glance.

| Situation | Roles to Involve |
|---|---|
| Unclear or changing requirements | Product Manager, UX Designer |
| User-reported bug or usability issue | Customer Support Representative → Developer, Product Manager |
| Security vulnerability or threat model | Security Lead, Developer, Project Manager |
| Missing or outdated documentation | Technical Writer, Developer |
| Success metrics unclear or missing | Data Analyst, Product Manager |
| Performance or usage data needed | Data Analyst |
| Design review before implementation | UX Designer, Developer, Product Manager |
| Cross-team dependency or risk | Project Manager, Product Manager |
| Compliance or regulatory question | Security Lead, Project Manager |
| Release communication to users | Product Manager, Technical Writer, Customer Support Representative |

---

## Related Documents

- [Roles and Personas](octoacme-roles-and-personas.md)
- [Project Initiation Guide](octoacme-project-initiation.md)
- [Project Planning](octoacme-project-planning.md)
- [Execution & Tracking](octoacme-execution-and-tracking.md)
- [Release & Deployment Guide](octoacme-release-and-deployment.md)
- [Risk Management & Communication](octoacme-risks-and-communication.md)
