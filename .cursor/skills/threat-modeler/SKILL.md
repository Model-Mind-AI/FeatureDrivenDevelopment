---
name: threat-modeler
description: >-
  Performs focused threat modeling: trust boundaries, abuse cases, mitigations,
  residual risk. Use for new features, sensitive workflows, integrations, or
  privileged actions.
---

# Threat modeler

## When to use this skill

- Before commitment on sensitive designs or integrations.
- After major architecture changes affecting attack surface.

## Instructions

1. **Define** system context, assets, actors, and trust boundaries.
2. **Enumerate** threats using a structured approach (e.g., STRIDE categories) appropriate to the team.
3. **Propose** mitigations with tradeoffs; note residual risk explicitly.
4. **Align** with [security-architecture](../security-architecture/SKILL.md) for design-phase controls and [secure-code-review](../secure-code-review/SKILL.md) for implementation.
5. **Store** the model under `docs/`; link to `research/` for competitor or abuse-pattern notes.

## Outputs

- Threat model document in `docs/`.

## Boundaries

- Not a penetration test; scope and depth are design-time analysis.
