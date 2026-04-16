---
name: model-mind-foundations
description: >-
  Shared rules for the Model Mind feature-driven workflow: artifact locations,
  traceability, security defaults, production readiness, subagent usage, and
  host-neutral patterns. Use when starting any Model Mind skill, setting up a
  repo layout, or aligning outputs across VS Code, Cursor, or Claude Code.
---

# Model Mind foundations

## Default repository layout

Assume these directories at the repository root unless the user specifies otherwise. Create them when producing new artifacts.

| Path | Use |
|------|-----|
| `docs/` | Product and technical documentation (Obsidian-friendly markdown is fine). |
| `research/` | Product comparisons, technical spikes, notes on libraries and approaches. |
| `src/` | Application and library code. |
| `brand/` | Brand guidelines, tone, and examples. |
| `brand/images/` | Logos and static images for the product. |

Prefer updating existing documents over duplicating them. Link related artifacts.

## Lifecycle alignment

Preserve alignment across: business objective → requirements → architecture → implementation → testing → deployment → observability → security.

## Traceability

For substantial outputs, make explicit:

- Which requirement or goal the work supports.
- Assumptions and open questions.
- Dependencies on other systems or teams.
- How tests or checks validate the change.
- What production signals will show it working.

## Secure by default

Assume least privilege, validated inputs, safe encoding of outputs, isolated secrets, authenticated and authorized access, auditability where relevant, and no insecure defaults.

## Production readiness

For non-trivial implementation, consider errors, retries and timeouts, telemetry, rollback, configuration separation, idempotency where it matters, and failure modes.

## Enterprise documentation minimum

For meaningful work, generate or update as appropriate: requirement artifact, design or architecture note, implementation plan, test approach, deployment or release impact, operational notes.

## Change impact

When something changes, call out what may need review: requirements, stories, API contracts, schemas, tests, docs, deployment config, monitoring.

## Human escalation

Flag explicitly: ambiguous business decisions, security-risk choices, irreversible migrations, compliance-sensitive edits, breaking public contracts, high-risk hotfixes.

## Subagents

Use specialized subagents or parallel review when multiple disciplines, high risk, or independent critique clearly helps—not for small linear tasks.

Cross-cutting examples: requirements analysis, architecture critique, security review, test coverage review, performance review, compliance review, code review, DevOps review. Domain examples: frontend, backend, database, API, integration, cloud, legacy modernization.

Orchestrate multiple perspectives, then synthesize one coherent recommendation.

## Host compatibility

Skills are host-neutral: prefer plain markdown, YAML, JSON, and code; avoid relying on a single IDE’s proprietary UI. Optional host-specific notes belong in individual skills, not here.
