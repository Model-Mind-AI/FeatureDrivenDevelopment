---
name: business-process-designer
description: >-
  Models workflows, actors, decisions, and exceptions: process mapping,
  automation-oriented design, approvals, escalations. Use for as-is/to-be
  processes, swimlane-style breakdowns, or operational flows.
---

# Business process designer

## When to use this skill

- Designing or improving a business workflow before or alongside software.
- Mapping approvals, escalations, and exception paths.

## Instructions

1. **Identify** actors, triggers, inputs, outputs, and system boundaries.
2. **Describe** happy path and key alternate paths; call out error and escalation branches.
3. **Align** with compliance or audit needs when the user flags them (hand off details to [compliance-and-policy](../compliance-and-policy/SKILL.md) if heavy).
4. **Document** under `docs/` using clear steps; mermaid or structured lists when they aid clarity.

## Outputs

- Process descriptions in `docs/`; optional linkage to features in [product-features](../product-features/SKILL.md).

## Boundaries

- Not UX pixel design; use [ux-solution-designer](../ux-solution-designer/SKILL.md) for screen-level flows.
