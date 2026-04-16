---
name: enterprise-standards-enforcer
description: >-
  Applies organizational engineering and documentation standards to outputs:
  naming, secure defaults, architecture conventions, and review expectations.
  Use when enforcing team rules, hardening drafts, or normalizing artifacts
  before review.
---

# Enterprise standards enforcer

## When to use this skill

- Output must match internal conventions.
- You need a consistency pass before merge or publication.
- The user references “our standards,” style guides, or compliance templates.

## Instructions

1. **Discover** in-repo standards: `.cursor/rules/`, `docs/` policy or standards folders, `AGENTS.md`, and explicit files the user names.
2. **Default baseline** when nothing is found: clear structure, explicit assumptions and risks, secure defaults per [model-mind-foundations](../model-mind-foundations/SKILL.md), and traceable references to requirements.
3. **Apply** naming, documentation structure, API and error-handling patterns, logging and secrets handling, and test expectations as documented by the project.
4. **Gap list**: if a standard is missing, state the gap and propose minimal conventions rather than inventing a large new framework without consent.
5. **Separate** fact, assumption, risk, and recommendation in review-style output.

## Outputs

- Annotated suggestions or a normalized copy of the artifact; place supporting rationale in `docs/` when the review is substantial.

## Boundaries

- Does not override explicit product or legal decisions; escalate per [model-mind-foundations](../model-mind-foundations/SKILL.md).
- Does not replace [compliance-and-policy](../compliance-and-policy/SKILL.md) for regulated control mapping.
