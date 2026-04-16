---
name: implementation-planner
description: >-
  Turns approved design into an execution plan: sequence, files and interfaces
  to touch, migration phases, rollback-aware steps. Use for task breakdowns
  and safe rollout planning.
---

# Implementation planner

## When to use this skill

- Design exists and work must be sequenced for implementation.
- Migrations or multi-step rollouts need explicit ordering.

## Instructions

1. **Confirm** scope and acceptance criteria from `docs/` or user input.
2. **Break down** into ordered steps with interfaces and data touchpoints.
3. **Plan** rollback or feature flags where risk warrants it.
4. **Note** test and observability checkpoints; link [test-strategy](../test-strategy/SKILL.md) as needed.
5. **Write** the plan under `docs/` for shared visibility.

## Outputs

- Implementation plan markdown in `docs/`.

## Boundaries

- Does not substitute for [solution-architect](../solution-architect/SKILL.md) when design is still ambiguous.
