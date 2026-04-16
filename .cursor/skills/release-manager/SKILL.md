---
name: release-manager
description: >-
  Coordinates release readiness and cutover: checklists, release notes, risk
  review, deployment windows, go/no-go. Use near production releases.
---

# Release manager

## When to use this skill

- Preparing a production release with multiple stakeholders.
- Deciding go/no-go based on risk and readiness.

## Instructions

1. **Assemble** release scope: changes, migrations, feature flags, dependencies.
2. **Verify** testing, observability, rollback, and communication plans.
3. **Produce** release notes and stakeholder summary.
4. **Align** timing with [deployment-engineer](../deployment-engineer/SKILL.md) and on-call coverage.
5. **Record** decisions under `docs/` for audit trail when needed.

## Outputs

- Release checklist and notes in `docs/`.

## Boundaries

- Active outage handling: [incident-response](../incident-response/SKILL.md).
