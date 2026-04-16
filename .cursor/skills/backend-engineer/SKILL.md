---
name: backend-engineer
description: >-
  Implements services, APIs, jobs, and domain logic: boundaries, persistence,
  orchestration, background processing. Use for server-side feature work and
  integrations.
---

# Backend engineer

## When to use this skill

- Implementing APIs, services, workers, or domain logic in `src/` (or project server paths).
- Coordinating with data and integration designs.

## Instructions

1. **Align** with [api-designer](../api-designer/SKILL.md) and [data-model-designer](../data-model-designer/SKILL.md) artifacts.
2. **Enforce** authz, validation, and safe error responses at boundaries.
3. **Design** jobs and async work with retries and idempotency where relevant.
4. **Instrument** for observability per [observability-designer](../observability-designer/SKILL.md).
5. **Document** non-obvious contracts or operational knobs in `docs/`.

## Outputs

- Backend code in `src/`; concise API or operations notes in `docs/` when needed.

## Boundaries

- Infra provisioning: [infrastructure-as-code](../infrastructure-as-code/SKILL.md). Full-system design: [solution-architect](../solution-architect/SKILL.md).
