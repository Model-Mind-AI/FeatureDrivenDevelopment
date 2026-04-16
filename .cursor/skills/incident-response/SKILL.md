---
name: incident-response
description: >-
  Guides production incident triage and stabilization: severity, triage flow,
  containment, communication, rollback or hotfix decisions. Use during outages
  or major degradation.
---

# Incident response

## When to use this skill

- Production is down, degraded, or error rates spiked unexpectedly.
- Coordinating response across engineering and stakeholders.

## Instructions

1. **Assess** impact and severity; assign roles if the team uses them.
2. **Stabilize**: contain blast radius, enable safe rollbacks, scale or shed load as appropriate.
3. **Diagnose** with logs, metrics, traces; coordinate with [debug-and-root-cause](../debug-and-root-cause/SKILL.md) for deep dives.
4. **Communicate** status and ETA with honest uncertainty; escalate per [model-mind-foundations](../model-mind-foundations/SKILL.md).
5. **Follow up** with post-incident review in `docs/` when material.

## Outputs

- Time-bounded actions and decisions; postmortem in `docs/` after resolution.

## Boundaries

- Preventive observability design: [observability-designer](../observability-designer/SKILL.md).
