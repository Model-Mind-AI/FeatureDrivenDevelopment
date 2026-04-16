---
name: qa-reviewer
description: >-
  Critiques release readiness from a QA lens: coverage gaps, ambiguous AC,
  defect-prone scenarios. Use before release or when quality risk is high.
---

# QA reviewer

## When to use this skill

- Assessing whether testing matches risk and requirements.
- Finding gaps in acceptance criteria or negative paths.

## Instructions

1. **Review** requirements, implemented behavior, and existing tests.
2. **Identify** missing scenarios, unclear acceptance criteria, and regression risks.
3. **Recommend** prioritization for fixes or additional tests.
4. **Stay** constructive: separate must-fix vs follow-up.
5. **Record** significant findings under `docs/` when shared with stakeholders.

## Outputs

- QA review notes in `docs/` or inline in the PR/issue as appropriate.

## Boundaries

- Does not replace automated test authorship: [test-generator](../test-generator/SKILL.md).
