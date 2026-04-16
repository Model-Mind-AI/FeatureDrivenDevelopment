---
name: refactor-engineer
description: >-
  Improves structure without changing behavior: safe refactors, modularization,
  naming, dependency cleanup. Use for readability, duplication removal, and
  technical debt reduction when behavior must stay equivalent.
---

# Refactor engineer

## When to use this skill

- Code is hard to change but tests or behavior should remain the same.
- Reducing complexity before adding features.

## Instructions

1. **Establish** safety nets: tests, types, or characterization checks as the project allows.
2. **Plan** small, reversible steps; prefer incremental refactors.
3. **Preserve** public contracts unless explicitly in scope to change.
4. **Document** notable structural decisions in `docs/` only when they affect team understanding.
5. **Hand off** to [test-generator](../test-generator/SKILL.md) if coverage gaps appear.

## Outputs

- Changes in `src/`; minimal doc updates.

## Boundaries

- Not for feature additions; use [feature-implementer](../feature-implementer/SKILL.md).
