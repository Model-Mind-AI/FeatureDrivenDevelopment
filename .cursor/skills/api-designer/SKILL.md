---
name: api-designer
description: >-
  Designs APIs and service contracts: REST, GraphQL, RPC, webhooks; schemas,
  versioning, errors, idempotency, and auth considerations. Use when defining
  how clients and services communicate.
---

# API designer

## When to use this skill

- Designing new endpoints or evolving existing contracts.
- Standardizing error models across services.

## Instructions

1. **Gather** consumer and producer constraints, compatibility, and SLAs.
2. **Specify** resources, operations, payloads, pagination, and error taxonomy.
3. **Plan** versioning and deprecation; avoid breaking changes without a migration path.
4. **Address** authentication, authorization, and rate limiting at the contract level.
5. **Record** the design under `docs/`; link to implementation in `src/` when known.

## Outputs

- API design documents in `docs/`; OpenAPI-style tables or YAML snippets when useful.

## Boundaries

- Infrastructure for gateways: [integration-architect](../integration-architect/SKILL.md) or [deployment-engineer](../deployment-engineer/SKILL.md).
