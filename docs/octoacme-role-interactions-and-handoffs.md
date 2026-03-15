# OctoAcme — Role Interactions & Handoffs

This document provides a lightweight RACI-style mapping of who does what across each project phase, plus Definition of Ready and Definition of Done checklists. Use it alongside [`octoacme-roles-and-personas.md`](octoacme-roles-and-personas.md) and the phase-specific process docs.

---

## RACI Key

| Symbol | Meaning |
|--------|---------|
| **R** | Responsible — does the work |
| **A** | Accountable — owns the outcome; approves |
| **C** | Consulted — provides input before decisions |
| **I** | Informed — kept up to date |

---

## Phase RACI Matrix

| Activity | PM | PdM | Developers | QA Lead | DevOps | UI/UX | Stakeholder Rep |
|---|---|---|---|---|---|---|---|
| **Initiation** | | | | | | | |
| Define problem statement & goals | C | **A/R** | I | I | I | C | C |
| Identify stakeholders & constraints | **A/R** | C | I | I | I | I | **R** |
| Create project charter / one-pager | **A/R** | C | I | I | I | I | C |
| Stakeholder kick-off review | **R** | R | I | I | I | I | **A** |
| **Planning** | | | | | | | |
| Prioritize & refine backlog | C | **A/R** | C | C | I | C | C |
| Define acceptance criteria | C | **A** | R | **R** | I | **R** | C |
| Draft test plan / QA approach | I | C | C | **A/R** | C | I | I |
| Create release plan & milestones | **A/R** | C | C | C | **R** | I | I |
| Define Definition of Done | **A** | R | R | **R** | R | C | I |
| Design specs & wireframes | I | C | C | I | I | **A/R** | I |
| **Execution** | | | | | | | |
| Implement features | I | C | **A/R** | C | C | C | I |
| UI fidelity review | I | C | C | C | I | **A/R** | I |
| Code review & merge | I | I | **A/R** | C | C | I | I |
| Move items to QA column | I | I | **R** | **A** | I | I | I |
| QA testing & sign-off | I | C | C | **A/R** | C | C | I |
| CI/CD pipeline maintenance | I | I | C | I | **A/R** | I | I |
| Risk register updates | **A/R** | C | C | C | C | I | I |
| **Release** | | | | | | | |
| Pre-release readiness checklist | **A** | C | C | **R** | **R** | I | I |
| Deployment to production | I | I | C | C | **A/R** | I | I |
| Post-deploy smoke test | I | I | C | **R** | **A** | I | I |
| Release announcement | **A/R** | R | I | I | I | I | **R** |
| **Retrospective & Close** | | | | | | | |
| Facilitate retrospective | **A/R** | C | R | R | R | R | I |
| Document lessons learned | **A/R** | R | R | R | R | R | I |
| Update process docs | **A** | C | R | C | C | C | I |
| Stakeholder close-out review | **R** | C | I | I | I | I | **A** |

---

## Key Handoff Points

### Planning → Execution
- **PdM → Developers + QA Lead**: Backlog items with written acceptance criteria are groomed and estimated before sprint start.
- **UI/UX → Developers**: Annotated design specs are available in the design tool or repo before development begins.
- **QA Lead → PM**: Test plan is reviewed and approved before sprint kick-off.

### Execution → QA
- **Developers → QA Lead**: Items are moved to the **QA** column on the project board only when:
  - PR is merged to the target branch.
  - Automated tests pass in CI.
  - A brief test notes comment is added to the issue.
- **DevOps → QA Lead**: Staging environment is confirmed healthy before QA begins.

### QA → Release
- **QA Lead → PM + DevOps**: QA sign-off issued when all test cases pass and no P1/P2 defects are open.
- **DevOps → PM**: Deployment plan and rollback procedure confirmed.
- **PM → Stakeholder Rep**: Release timing communicated at least one business day in advance.

### Release → Retrospective
- **PM**: Schedules retro within one week of release.
- **QA Lead + DevOps**: Bring post-deploy metrics and incident data to the retro.
- **Stakeholder Rep**: Shares post-release stakeholder feedback at retro or close-out review.

---

## Definition of Ready (DoR)

A backlog item is **Ready** to be pulled into a sprint when all of the following are true:

- [ ] Problem / user story is clearly described with a "who, what, why" format
- [ ] Acceptance criteria are written and agreed by PdM and QA Lead
- [ ] Design specs or wireframes attached (if UI work is involved)
- [ ] Dependencies identified and unblocked (or explicitly accepted risk)
- [ ] Estimate provided by the development team
- [ ] Item is small enough to complete within one sprint; large items are split

---

## Definition of Done (DoD)

An item is **Done** when all of the following are true:

- [ ] Code implemented and merged to the target branch
- [ ] Automated unit/integration tests written and passing in CI
- [ ] Security scan passes (no new high/critical findings)
- [ ] Code reviewed and approved by at least one peer
- [ ] Acceptance criteria verified by QA Lead (item moved through the **QA** board column)
- [ ] UI/UX review completed for any user-facing changes
- [ ] Documentation updated (API docs, runbooks, README) if applicable
- [ ] No P1 or P2 defects open against the item
- [ ] Release notes entry drafted

---

## Related Documents

- [`octoacme-roles-and-personas.md`](octoacme-roles-and-personas.md) — full role descriptions and interaction points
- [`octoacme-project-management-overview.md`](octoacme-project-management-overview.md) — principles, lifecycle, and artifacts
- [`octoacme-project-planning.md`](octoacme-project-planning.md) — backlog and planning activities
- [`octoacme-execution-and-tracking.md`](octoacme-execution-and-tracking.md) — day-to-day delivery and board workflow
- [`octoacme-release-and-deployment.md`](octoacme-release-and-deployment.md) — deployment and release process
- [`octoacme-retrospective-and-continuous-improvement.md`](octoacme-retrospective-and-continuous-improvement.md) — retro format and action tracking
