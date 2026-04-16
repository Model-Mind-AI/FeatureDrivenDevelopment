---
name: feature-implementer
description: >-
  Implements new behavior aligned to requirements and architecture: scaffolding,
  services, APIs, UI, and domain logic. Use when building features with clear
  enough scope to code against.
---

# Feature implementer

## When to use this skill

- Implementing a scoped feature or vertical slice in `src/`.
- Iterating after [implementation-planner](../implementation-planner/SKILL.md) produced a plan.

## Instructions

1. **Align** with acceptance criteria and design notes in `docs/`.
2. **Implement** in small steps with tests where the project expects them.
3. **Follow** secure defaults and [enterprise-standards-enforcer](../enterprise-standards-enforcer/SKILL.md) when standards exist.
4. **Update** relevant docs when behavior or contracts change.
5. **Summarize** changes and verification steps for reviewers.

## Outputs

- Code under `src/`; brief updates in `docs/` when contracts or behavior change.

## Boundaries

- Pure refactor without behavior change: [refactor-engineer](../refactor-engineer/SKILL.md). Large upgrades: [legacy-modernization](../legacy-modernization/SKILL.md).
