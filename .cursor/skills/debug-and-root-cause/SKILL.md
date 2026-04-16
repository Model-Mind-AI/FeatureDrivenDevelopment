---
name: debug-and-root-cause
description: >-
  Diagnoses failures in tests, CI, or production symptoms: hypotheses,
  reproduction, isolation, fix plan. Use for bugs, flakes, and build breaks.
---

# Debug and root cause

## When to use this skill

- Something fails intermittently or consistently and needs systematic diagnosis.
- Narrowing whether the bug is code, config, data, or environment.

## Instructions

1. **Capture** symptoms, scope, recent changes, and impact.
2. **Form** hypotheses; design minimal reproduction or experiments.
3. **Isolate** the layer (application, dependency, infra) with evidence.
4. **Propose** a fix with risk and rollback; involve [secure-code-review](../secure-code-review/SKILL.md) if security-sensitive.
5. **Document** root cause and prevention under `docs/` when incidents are significant.

## Outputs

- Fix in `src/` or config; postmortem-style notes in `docs/` when warranted.

## Boundaries

- Major incident command: [incident-response](../incident-response/SKILL.md). Test strategy gaps: [test-strategy](../test-strategy/SKILL.md).
