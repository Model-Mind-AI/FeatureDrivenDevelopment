---
name: ci-cd-designer
description: >-
  Designs build, test, release, and promotion pipelines: stages, gates,
  branch rules, artifact promotion. Use for GitHub Actions, Azure DevOps,
  GitLab CI, or comparable systems.
---

# CI/CD designer

## When to use this skill

- Setting up or overhauling CI/CD for a repo or service.
- Defining quality gates and release promotion.

## Instructions

1. **Define** pipeline stages: build, test, analysis, package, deploy, promote.
2. **Specify** branch and environment mapping; protect production deploys.
3. **Include** secret handling patterns and least privilege for pipeline identities.
4. **Align** test stages with [test-strategy](../test-strategy/SKILL.md); security scans with [secure-code-review](../secure-code-review/SKILL.md) expectations.
5. **Document** under `docs/` with pipeline diagrams or step lists.

## Outputs

- Pipeline design in `docs/`; implementation in project CI files as requested.

## Boundaries

- Runtime incident handling: [incident-response](../incident-response/SKILL.md).
