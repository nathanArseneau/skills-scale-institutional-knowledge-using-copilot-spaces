# OctoAcme Personas

This document defines typical roles and responsibilities used in OctoAcme project docs and exercises.

---

## Developers

### Role Summary
Developers design, build, test, and deliver software components. They collaborate with product and project leads to implement features that meet acceptance criteria and quality standards.

### Responsibilities
- Implement features and fixes to meet acceptance criteria
- Write and maintain tests and documentation
- Participate in design and code reviews
- Assist in estimating and planning work
- Help identify technical risks and propose mitigations

### Goals
- Deliver reliable, maintainable code
- Reduce cycle time from idea to production
- Maintain high test coverage and observability

### Typical Communication
- Daily standups and sprint planning
- PR descriptions and code review comments
- Technical design docs when needed

---

## Product Managers

### Role Summary
Product Managers define what should be built to deliver customer and business value. They own the product vision, prioritize the backlog, and measure outcomes.

### Responsibilities
- Define problem statements and success metrics
- Prioritize the roadmap and backlog
- Collaborate with stakeholders and engineering on trade-offs
- Validate solutions through user research and metrics

### Goals
- Maximize customer value and impact
- Make clear, data-driven prioritization decisions
- Ensure product-market fit and usability

### Typical Communication
- Weekly alignment with PM and engineering leads
- Roadmap updates and stakeholder briefings
- Acceptance criteria and feature specs

---

## Project Managers

### Role Summary
Project Managers coordinate delivery activities, manage schedules, risks, and communications. They enable the team to deliver on commitments efficiently.

### Responsibilities
- Create and maintain project plans and timelines
- Manage risks, dependencies, and resource constraints
- Facilitate meetings (kickoff, planning, retrospectives)
- Ensure consistent project documentation and status reporting
- Coordinate cross-team and stakeholder communication

### Goals
- Deliver projects on time and within scope
- Minimize unplanned work and escalations
- Maintain transparency and alignment across stakeholders

### Typical Communication
- Weekly status updates and stakeholder reports
- Risk registers and decision logs
- Coordination via project boards and meeting facilitation

---

## QA Lead

### Role Summary
The QA Lead owns the quality assurance strategy, test coverage, and release readiness sign-off. They bridge product requirements and engineering to ensure features meet acceptance criteria before shipping.

### Responsibilities
- Define and maintain the test strategy, test plans, and coverage targets
- Coordinate manual and automated testing across feature areas
- Run regression suites and approve production readiness
- Track and triage bugs; escalate blocking issues to the PM
- Participate in sprint planning to estimate QA effort and flag testability concerns

### Goals
- Prevent defects from reaching production
- Continuously improve test automation coverage
- Ensure every release meets the Definition of Done quality bar

### Typical Communication
- Sprint planning and backlog refinement with Developers and PM
- QA sign-off comments on pull requests and the project board QA column
- Bug triage reports shared with PdM and PM
- Pre-release readiness checklist reviewed with DevOps Engineer

### Interaction Points with Existing Roles
- **Developers**: Collaborates on test automation, acceptance criteria, and PR reviews before moving items to the QA column.
- **Product Manager (PdM)**: Reviews acceptance criteria definitions; surfaces quality trade-offs during backlog prioritization.
- **Project Manager (PM)**: Reports QA status and blocking defects during weekly delivery sync; participates in retrospectives.
- **DevOps Engineer**: Coordinates pre-deployment smoke tests and environment readiness.

---

## DevOps Engineer

### Role Summary
The DevOps Engineer maintains the CI/CD pipelines, infrastructure, and deployment tooling that allow the team to ship reliably and quickly.

### Responsibilities
- Build and maintain CI/CD pipelines (automated build, test, deploy)
- Manage deployment environments (dev, staging, production) and infrastructure-as-code
- Monitor system health, respond to incidents, and drive post-mortems
- Advise the team on branching strategy, secret management, and security scanning
- Collaborate on release plans and rollback procedures

### Goals
- Enable fast, safe, repeatable deployments
- Maximize system uptime and reduce mean time to recovery (MTTR)
- Keep infrastructure costs and complexity manageable

### Typical Communication
- Release planning sessions with PM and QA Lead
- CI/CD status in the project board and PR checks
- Incident and post-mortem reports shared with PM and Developers
- Infrastructure change proposals reviewed with tech leads

### Interaction Points with Existing Roles
- **Developers**: Reviews branching conventions, pipeline configuration, and deployment scripts; pairs on resolving build/deploy failures.
- **Project Manager (PM)**: Participates in release planning; flags environment risks in the risk register.
- **QA Lead**: Coordinates test environment provisioning and pre-release smoke test execution.
- **Stakeholder Representative**: Communicates deployment schedules and maintenance windows.

---

## Stakeholder Representative

### Role Summary
The Stakeholder Representative acts as the voice of external stakeholders or customer groups throughout the project lifecycle, ensuring their interests, feedback, and priorities are surfaced to the delivery team.

### Responsibilities
- Gather and synthesize stakeholder requirements, constraints, and feedback
- Review and approve key deliverables (project charter, release notes, demos)
- Escalate business-critical concerns to the PM and PdM
- Communicate project status and milestones back to external stakeholders
- Participate in project initiation, milestone reviews, and retrospectives

### Goals
- Ensure stakeholder expectations align with delivery outcomes
- Reduce miscommunication and late-stage scope surprises
- Maintain trust and transparency with business stakeholders

### Typical Communication
- Monthly stakeholder updates coordinated with PM
- Review meetings at project milestones (initiation, release, retro)
- Ad-hoc feedback via shared decision logs

### Interaction Points with Existing Roles
- **Product Manager (PdM)**: Co-authors the problem statement and success metrics; validates that roadmap priorities reflect stakeholder needs.
- **Project Manager (PM)**: Receives regular status reports; escalates blockers or business risks.
- **Developers**: Participates in sprint demos to provide timely feedback on delivered features.
- **UI/UX Designer**: Reviews design prototypes and usability test results from a business-value perspective.

---

## UI/UX Designer

### Role Summary
The UI/UX Designer defines interface and experience requirements, ensuring that features are usable, accessible, and aligned with customer needs.

### Responsibilities
- Create wireframes, prototypes, and annotated design specs for features
- Conduct usability reviews and accessibility audits
- Collaborate with Product Managers to translate requirements into design solutions
- Provide design review feedback on implemented features before QA sign-off
- Maintain the design system and ensure visual consistency

### Goals
- Deliver intuitive, accessible, and visually consistent user experiences
- Reduce design-to-development rework through clear, well-documented specs
- Validate that shipped features match intended UX outcomes

### Typical Communication
- Design review sessions with PdM and Developers during planning and execution
- Annotated design artifacts shared in the project repo or design tool
- Usability feedback shared with PdM and QA Lead before release

### Interaction Points with Existing Roles
- **Product Manager (PdM)**: Partners on feature discovery, user stories, and success metrics tied to usability.
- **Developers**: Provides design specs, answers implementation questions, and reviews UI fidelity in PRs.
- **QA Lead**: Shares usability and accessibility test criteria to include in QA sign-off.
- **Stakeholder Representative**: Presents design prototypes for early stakeholder feedback.

---

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.
- See [`octoacme-role-interactions-and-handoffs.md`](octoacme-role-interactions-and-handoffs.md) for a RACI-lite matrix and Definition of Ready/Done checklists that show how all roles collaborate across project phases.

