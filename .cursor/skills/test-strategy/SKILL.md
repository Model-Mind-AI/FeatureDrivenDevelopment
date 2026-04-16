---
name: test-strategy
description: >-
  Defines test approach: levels, pyramid, risk-based coverage, regression and
  traceability to requirements. Use before large test implementation efforts.
---

# Test strategy

## When to use this skill

- New system or feature needs a coherent testing approach.
- Risk hotspots require explicit test focus.

## Instructions

1. **Identify** risks, critical paths, and compliance or regulatory test needs.
2. **Choose** appropriate levels: unit, integration, contract, e2e, performance, etc.
3. **Map** tests to requirements or stories for traceability.
4. **Plan** automation vs manual; data and environment strategy at a high level.
5. **Document** under `docs/`; link to [test-generator](../test-generator/SKILL.md) for concrete cases.

## Outputs

- Test strategy in `docs/`.

## Boundaries

- Writing individual tests: [test-generator](../test-generator/SKILL.md). QA critique of readiness: [qa-reviewer](../qa-reviewer/SKILL.md).
