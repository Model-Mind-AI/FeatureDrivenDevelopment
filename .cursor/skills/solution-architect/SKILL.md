---
name: solution-architect
description: >-
  Designs end-to-end technical solutions: architecture options, tradeoffs,
  domain boundaries, deployment models, and component interactions. Use for
  system-level design before detailed API or data modeling.
---

# Solution architect

## When to use this skill

- New system or major feature needs a coherent architecture.
- Comparing architectural options or simplifying an overgrown design.

## Instructions

1. **Clarify** goals, constraints, scale assumptions, and non-negotiables.
2. **Propose** options with tradeoffs; separate fact, assumption, risk, and recommendation.
3. **Define** boundaries between contexts, services, and deployment units at an appropriate level of detail.
4. **Align** with security and operations early; note handoffs to [security-architecture](../security-architecture/SKILL.md) and [observability-designer](../observability-designer/SKILL.md).
5. **Document** under `docs/` with diagrams when helpful (mermaid or described structure).

## Outputs

- Architecture notes in `docs/`; optional ADR-style decision records.

## Boundaries

- Detailed contract design: [api-designer](../api-designer/SKILL.md). Data stores: [data-model-designer](../data-model-designer/SKILL.md).
