---
name: artifact-governance
description: >-
  Keeps requirements, design, code, tests, and deployment artifacts aligned;
  traceability, version alignment, and change-impact analysis. Use when
  validating consistency across features, docs, stories, code, and tests, or
  asking “what else must change if this changes?”
---

# Artifact governance

## When to use this skill

- A change might affect multiple artifact types.
- Traceability from requirement to release is unclear or broken.
- Preparing an audit or release and need a consistency pass.

## Instructions

1. **Identify** the authoritative sources for requirements and design (typically under `docs/`).
2. **Map** requirements and decisions to: implementation in `src/`, tests, deployment or config docs, and operational runbooks as applicable.
3. **Report** gaps: missing links, outdated sections, contradictory statements, orphan code or tests.
4. **Change impact**: list artifacts and systems that should be reviewed or updated for the proposed change.
5. **Prefer revision** of existing documents over creating duplicate files; note renames or deprecations clearly.

## Outputs

- A traceability or governance note under `docs/` (markdown), with explicit gaps and recommended updates—not silent mass edits unless the user asked for edits.

## Boundaries

- Does not set organizational policy; applies [enterprise-standards-enforcer](../enterprise-standards-enforcer/SKILL.md) context when standards exist.
- Security findings are inputs to [secure-code-review](../secure-code-review/SKILL.md) and [threat-modeler](../threat-modeler/SKILL.md), not a full pen test here.
