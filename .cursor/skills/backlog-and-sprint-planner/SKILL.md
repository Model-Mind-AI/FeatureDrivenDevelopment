---
name: backlog-and-sprint-planner
description: >-
  Converts requirements into ordered, executable work: backlog structure, story
  slicing, dependencies, MVP vs later phases. Use for sprint plans, sequencing,
  and dependency mapping.
---

# Backlog and sprint planner

## When to use this skill

- Ordering work for a timebox or release train.
- Splitting epics into slices that can ship incrementally.

## Instructions

1. **Ingest** features and constraints from `docs/` or user input.
2. **Order** by value, risk reduction, dependencies, and learning.
3. **Slice** stories so each item is small enough to complete and test; mark MVP vs deferred.
4. **Surface** technical dependencies for [implementation-planner](../implementation-planner/SKILL.md) when needed.
5. **Record** the plan under `docs/` with rationale for ordering.

## Outputs

- Backlog or sprint plan markdown in `docs/`.

## Boundaries

- Does not estimate for the team unless the user provides estimation rules; focus on structure and dependencies.
