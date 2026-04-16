---
name: integration-architect
description: >-
  Designs internal and external integrations: third-party APIs, enterprise
  systems, queues, buses, auth flows; retries, failure modes, sync vs async.
  Use for integration-heavy features or platform boundaries.
---

# Integration architect

## When to use this skill

- Connecting to external systems or stitching services together.
- Hardening unreliable network paths.

## Instructions

1. **Map** contracts, auth modes, and data ownership between systems.
2. **Choose** sync vs async patterns; define timeouts, retries, idempotency, and dead-letter behavior.
3. **Describe** failure modes and operational recovery; align with [observability-designer](../observability-designer/SKILL.md).
4. **Coordinate** with [api-designer](../api-designer/SKILL.md) for outward-facing APIs.
5. **Document** under `docs/` with sequence or flow descriptions.

## Outputs

- Integration design in `docs/`; explicit operational notes.

## Boundaries

- Vendor-specific runbooks may live with [deployment-engineer](../deployment-engineer/SKILL.md) or [incident-response](../incident-response/SKILL.md).
