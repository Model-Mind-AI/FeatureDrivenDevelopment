---
name: infrastructure-as-code
description: >-
  Designs and critiques infrastructure definitions: Terraform, Bicep,
  CloudFormation, Kubernetes manifests; modularity, parity, secrets, least
  privilege. Use for cloud and cluster foundations.
---

# Infrastructure as code

## When to use this skill

- Defining or changing cloud resources, clusters, or platform primitives as code.
- Improving environment parity and reducing drift.

## Instructions

1. **Structure** modules for reuse; separate environments clearly.
2. **Handle** secrets via approved mechanisms; least privilege IAM and network posture.
3. **Plan** state, locking, and review workflows for changes.
4. **Align** with [deployment-engineer](../deployment-engineer/SKILL.md) for app-level rollout.
5. **Document** architecture and operational ownership in `docs/`.

## Outputs

- IaC under project paths; design notes in `docs/`.

## Boundaries

- Application code: [backend-engineer](../backend-engineer/SKILL.md). Incident response: [incident-response](../incident-response/SKILL.md).
