---
name: security-architecture
description: >-
  Defines secure design before build: trust boundaries, authn/authz, secrets
  strategy, data sensitivity, attack surface. Use early in design for sensitive
  features or privileged operations.
---

# Security architecture

## When to use this skill

- Designing or reviewing architecture for security-sensitive workflows.
- Defining how identity, secrets, and sensitive data are handled at design time.

## Instructions

1. **Identify** trust boundaries, assets, and threat-relevant actors.
2. **Specify** authentication and authorization models; least privilege defaults.
3. **Plan** secrets management, key rotation, and configuration hygiene.
4. **Align** with [threat-modeler](../threat-modeler/SKILL.md) for structured threat modeling; with [compliance-and-policy](../compliance-and-policy/SKILL.md) for regulatory controls.
5. **Record** decisions under `docs/` with clear rationale.

## Outputs

- Security architecture notes in `docs/`.

## Boundaries

- Code-level review: [secure-code-review](../secure-code-review/SKILL.md). Operational incident handling: [incident-response](../incident-response/SKILL.md).
