---
name: codebase-analyzer
description: >-
  Understands an existing codebase before changes: structure, dependencies,
  hotspots, drift from intended architecture. Use for legacy systems, new
  repos, or “where should this change go?”
---

# Codebase analyzer

## When to use this skill

- Onboarding to unfamiliar code or planning a cross-cutting change.
- Mapping dependencies and risk areas before refactors.

## Instructions

1. **Survey** layout, build entry points, and major modules under `src/` (or project convention).
2. **Identify** dependency direction, coupling, and boundaries versus documented architecture in `docs/`.
3. **Highlight** hotspots: churn, complexity, missing tests.
4. **Recommend** where changes should live and what to read first.
5. **Summarize** findings under `docs/` when the analysis is non-trivial.

## Outputs

- Analysis notes in `docs/` or `research/` for exploratory spikes.

## Boundaries

- Does not implement features; hands off to [implementation-planner](../implementation-planner/SKILL.md) or [feature-implementer](../feature-implementer/SKILL.md).
