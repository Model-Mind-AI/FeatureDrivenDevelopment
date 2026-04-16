---
name: data-model-designer
description: >-
  Designs persistence and data movement: entities, relationships, storage
  choices, indexing, migrations, retention. Use for schemas, events, and
  reporting-oriented models.
---

# Data model designer

## When to use this skill

- Designing or changing databases, event payloads, or analytical models.
- Planning migrations with rollback and compatibility in mind.

## Instructions

1. **Elicit** consistency, availability, and privacy requirements.
2. **Model** entities and relationships; justify normalization or denormalization.
3. **Plan** migrations: phases, backfill, dual-write, and validation.
4. **Cover** retention and archival where relevant; flag compliance needs for [compliance-and-policy](../compliance-and-policy/SKILL.md).
5. **Document** under `docs/` with clear schema definitions or ER descriptions.

## Outputs

- Data design docs in `docs/`; migration notes alongside.

## Boundaries

- Does not replace [solution-architect](../solution-architect/SKILL.md) for full system topology.
