---
name: legacy-modernization
description: >-
  Plans and executes safe upgrades of older systems: framework migrations,
  platform moves, strangler patterns, phased cutover. Use when modernizing
  stacks or decomposing monoliths.
---

# Legacy modernization

## When to use this skill

- Upgrading frameworks, runtimes, or infrastructure with coexistence periods.
- Replacing subsystems incrementally.

## Instructions

1. **Assess** current state with [codebase-analyzer](../codebase-analyzer/SKILL.md); capture risks and constraints.
2. **Define** phases: coexistence, dual-write, validation, cutover, rollback.
3. **Identify** compatibility risks and migration tests.
4. **Coordinate** with [deployment-engineer](../deployment-engineer/SKILL.md) and [release-manager](../release-manager/SKILL.md) for rollout.
5. **Record** the roadmap under `docs/` and spikes under `research/` when exploring options.

## Outputs

- Modernization plan in `docs/`; code changes in `src/` per phase.

## Boundaries

- Greenfield design without legacy constraints: [solution-architect](../solution-architect/SKILL.md).
