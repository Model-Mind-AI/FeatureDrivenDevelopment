---
name: platform-engineer
description: >-
  Builds shared platform capabilities: internal SDKs, libraries, templates,
  scaffolds, and cross-cutting developer foundations. Use when many teams
  reuse the same primitives or patterns.
---

# Platform engineer

## When to use this skill

- Creating or evolving shared libraries, CLI tooling, or service templates.
- Standardizing how product teams bootstrap or integrate.

## Instructions

1. **Define** consumers, versioning, and compatibility promises.
2. **Design** APIs for clarity and safe defaults; document extensively.
3. **Align** with [enterprise-standards-enforcer](../enterprise-standards-enforcer/SKILL.md) for org-wide consistency.
4. **Plan** rollout and migration for existing adopters.
5. **Place** reusable code under appropriate `src/` packages; keep `docs/` as the source of truth for usage.

## Outputs

- Platform code and templates under `src/`; documentation in `docs/`.

## Boundaries

- Product feature delivery is [feature-implementer](../feature-implementer/SKILL.md); this skill owns reusable foundations.
