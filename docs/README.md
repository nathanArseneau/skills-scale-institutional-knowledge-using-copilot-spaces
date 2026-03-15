# OctoAcme Project Management Docs

Welcome to the central hub for OctoAcme's project management documentation. This README provides an overview of our processes and links to all process documents stored in this `docs/` folder. These artifacts are versioned and accessible to the entire team to accelerate onboarding, enable consistent execution, and reduce dependency risk.

## Overview

OctoAcme's project management approach follows a lightweight but structured lifecycle: **initiation → planning → execution → release → close/retrospective**. Work starts when a new initiative is ready to be explored, using a short **Project One-pager** to clarify the problem, SMART objective, success metrics, stakeholders, rough milestones, risks/dependencies, and resource needs. A clear **decision gate** is used to move forward only when success metrics and priority are aligned and team availability is confirmed. From there, planning turns the approved initiative into an actionable backlog with acceptance criteria, estimates, a Definition of Done, and an initial QA/testing approach.

Roles are explicitly defined to keep ownership clear and reduce ambiguity. The **Project Manager (PM)** coordinates delivery mechanics—timeline, risks, dependencies, and communications—while the **Product Manager (PdM)** defines outcomes, prioritizes the backlog, and measures success. **Developers** implement, test, and document changes while collaborating on design and review, and **QA/Testing** validates quality and acceptance criteria. Stakeholders contribute inputs and approvals, and the overall system emphasizes iterative delivery, clear accountability, and data-informed decision-making.

Day-to-day execution centers on a consistent team rhythm and visible workflow. Teams use a project board (e.g., GitHub Projects) with columns such as **Backlog, Ready, In Progress, In Review, QA, Done**, supported by short feedback loops like **daily standups** (progress/blockers/dependencies), a **weekly delivery sync** (progress + flagged risks), and **demos/reviews** at the end of sprints or milestones. Risks and dependencies are managed via a simple **risk register** (impact/likelihood/owner/mitigation/status) and reviewed regularly, with a defined escalation path from team triage up through PM/Product Lead and, when necessary, to sponsor-level escalation.

Quality assurance is built into the workflow through both engineering standards and release discipline. OctoAcme expects **unit tests for new logic**, broader **integration tests where applicable**, and **end-to-end smoke tests** for critical flows before release, plus **security scanning in CI** and **manual QA** when needed for feature acceptance. The PR process favors **small pull requests**, requires linking to issues and acceptance criteria, and expects CI (tests/linting) to pass before review—along with at least one approval prior to merge. Releases follow a checklist-driven process with release notes, rollback/mitigation planning, staged deployment, post-deploy verification, and stakeholder announcements, and continuous improvement is reinforced through retrospectives that produce owned, time-bound action items tracked like any other work.

## Process Documents

| Document | Description |
|---|---|
| [Project Management Overview](octoacme-project-management-overview.md) | High-level overview of OctoAcme's project management approach |
| [Project Initiation Guide](octoacme-project-initiation.md) | How to kick off a new initiative, including the Project One-pager and decision gate |
| [Project Planning](octoacme-project-planning.md) | Turning an approved initiative into an actionable backlog and sprint plan |
| [Execution & Tracking](octoacme-execution-and-tracking.md) | Day-to-day workflow, standups, board management, and risk tracking |
| [Risk Management & Communication](octoacme-risks-and-communication.md) | Risk register, escalation paths, and communication cadence |
| [Release & Deployment Guide](octoacme-release-and-deployment.md) | Release checklist, deployment steps, rollback planning, and stakeholder announcements |
| [Retrospective & Continuous Improvement](octoacme-retrospective-and-continuous-improvement.md) | Running retrospectives and tracking improvement action items |
| [Roles & Personas](octoacme-roles-and-personas.md) | Definitions and responsibilities for PM, PdM, Developers, QA/Testing, and Stakeholders |

## Contributing

When creating or updating process documentation, refer to the issue templates in [`.github/ISSUE_TEMPLATE/`](../.github/ISSUE_TEMPLATE/) for guidance on how to structure requests related to process docs.
