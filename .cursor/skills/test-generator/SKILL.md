---
name: test-generator
description: >-
  Produces concrete tests from requirements and code: unit, integration, API,
  UI, regression. Use when implementing or expanding automated tests.
---

# Test generator

## When to use this skill

- Adding or updating tests alongside implementation.
- Translating acceptance criteria into executable checks.

## Instructions

1. **Align** with [test-strategy](../test-strategy/SKILL.md) when one exists; otherwise infer minimal viable coverage.
2. **Generate** tests matching project frameworks and folder conventions.
3. **Cover** happy paths, edge cases, and failure modes relevant to the change.
4. **Use** fixtures, mocks, and factories consistent with existing code.
5. **Keep** tests deterministic and fast where possible.

## Outputs

- Test code under project test paths (often alongside `src/`); small notes in `docs/` if test data setup is unusual.

## Boundaries

- Root-cause debugging: [debug-and-root-cause](../debug-and-root-cause/SKILL.md). Strategic QA sign-off: [qa-reviewer](../qa-reviewer/SKILL.md).
