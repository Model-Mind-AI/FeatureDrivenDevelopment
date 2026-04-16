---
name: observability-designer
description: >-
  Designs logs, metrics, traces, alerts, and dashboards for operability and
  SLO alignment. Use when defining how to measure and diagnose systems in
  production.
---

# Observability designer

## When to use this skill

- New services or features need telemetry design.
- Alerting is noisy or missing; SLOs need clarity.

## Instructions

1. **Define** user- and system-level metrics that matter; avoid metric sprawl.
2. **Specify** structured logging and correlation identifiers across boundaries.
3. **Design** traces for critical paths; sampling where needed.
4. **Align** alerts with actionable, low-noise thresholds; document runbooks with [deployment-engineer](../deployment-engineer/SKILL.md) or [incident-response](../incident-response/SKILL.md).
5. **Document** under `docs/` with dashboards and alert inventory as lists.

## Outputs

- Observability design in `docs/`; instrumentation guidance for `src/`.

## Boundaries

- Does not replace vendor-specific monitoring setup details owned by the team’s toolchain.
