# FDD Factory (Cursor skill pack)

This folder documents the **installable skill pack** aligned with `feature_driven_docs` in this repository. The skills themselves live under **`.cursor/skills/`** so Cursor loads them for this workspace.

## Assumptions

- **Scope:** One skill per domain capability from the Model Mind category documents, plus **`model-mind-foundations`** for shared rules and layout.
- **Outputs:** By default, artifacts go to repository-root **`docs/`**, **`research/`**, **`src/`**, and **`brand/`** (see foundations skill). Create these directories when writing new material.
- **SpecDriven:** The `SpecDriven` tree in this repo was used only as a loose reference for how spec-driven workflows can work; it was not copied into these skills.

## Skill inventory

| Area | Skills |
|------|--------|
| Foundations | `model-mind-foundations` |
| Orchestration | `software-delivery-orchestrator`, `artifact-governance`, `enterprise-standards-enforcer` |
| Product and discovery | `product-features`, `business-process-designer`, `ux-solution-designer`, `backlog-and-sprint-planner` |
| Architecture and design | `solution-architect`, `api-designer`, `data-model-designer`, `integration-architect`, `security-architecture`, `performance-and-scalability-architect` |
| Engineering | `codebase-analyzer`, `implementation-planner`, `feature-implementer`, `refactor-engineer`, `legacy-modernization`, `frontend-engineer`, `backend-engineer`, `platform-engineer` |
| Quality and validation | `test-strategy`, `test-generator`, `qa-reviewer`, `debug-and-root-cause`, `observability-designer` |
| Security and compliance | `secure-code-review`, `compliance-and-policy`, `threat-modeler` |
| Delivery and operations | `ci-cd-designer`, `deployment-engineer`, `infrastructure-as-code`, `release-manager`, `incident-response` |
| Research | `product-research` |

## Using elsewhere

To reuse this pack in another repository, copy the `.cursor/skills/*` directories (or a subset) into that project’s `.cursor/skills/` folder, preserving each `SKILL.md` and relative links between skills.
