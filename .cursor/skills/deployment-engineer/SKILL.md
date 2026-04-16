---
name: deployment-engineer
description: >-
  Prepares deployment configuration and rollout strategy: environments,
  blue-green or canary, config safety, rollback. Use when shipping to staging
  or production beyond pure CI definition.
---

# Deployment engineer

## When to use this skill

- Designing how an app deploys and promotes across environments.
- Implementing rollout mechanics and operational hooks.

## Instructions

1. **Model** environments and configuration separation; avoid secrets in source.
2. **Choose** rollout strategy appropriate to risk: rolling, blue-green, canary.
3. **Define** rollback triggers and steps; align with [release-manager](../release-manager/SKILL.md).
4. **Coordinate** observability hooks with [observability-designer](../observability-designer/SKILL.md).
5. **Document** runbooks under `docs/` for operators.

## Outputs

- Deployment manifests and config under project conventions; runbooks in `docs/`.

## Boundaries

- Infra-as-code resource definitions: [infrastructure-as-code](../infrastructure-as-code/SKILL.md).
