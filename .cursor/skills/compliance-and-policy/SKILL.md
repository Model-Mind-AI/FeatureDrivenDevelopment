---
name: compliance-and-policy
description: >-
  Maps regulated or enterprise policy requirements to controls and evidence:
  auditability, privacy, retention, approvals. Use when compliance constraints
  drive design or release.
---

# Compliance and policy

## When to use this skill

- GDPR, HIPAA, SOC, ISO, industry-specific rules, or internal policy packs apply.
- Evidence is required for audits or security reviews.

## Instructions

1. **Clarify** which frameworks and obligations apply; do not invent legal conclusions—flag legal review when needed.
2. **Map** controls to features, data flows, and operational practices.
3. **Identify** gaps: missing logging, retention, consent, access reviews, etc.
4. **Specify** required artifacts and evidence for reviews.
5. **Document** under `docs/` with clear separation of requirement vs implementation status.

## Outputs

- Compliance mapping and gap analysis in `docs/`.

## Boundaries

- Code-level exploit review: [secure-code-review](../secure-code-review/SKILL.md). Threat modeling workshops: [threat-modeler](../threat-modeler/SKILL.md).
