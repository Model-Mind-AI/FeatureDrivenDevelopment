---
name: secure-code-review
description: >-
  Reviews code for vulnerabilities and unsafe patterns: auth flaws, injection,
  secrets exposure, insecure defaults. Use on changes touching trust boundaries,
  crypto, or sensitive data.
---

# Secure code review

## When to use this skill

- Reviewing PRs or diffs with security relevance.
- Hardening authentication, authorization, parsing, or deserialization.

## Instructions

1. **Scope** trust boundaries and data sensitivity for the change.
2. **Check** input validation, output encoding, authz checks, secrets handling, and dependency risk.
3. **Recommend** concrete remediations with severity and exploitability context.
4. **Escalate** architectural issues to [security-architecture](../security-architecture/SKILL.md) or [threat-modeler](../threat-modeler/SKILL.md).
5. **Record** significant findings in `docs/` when tracking remediation across teams.

## Outputs

- Review comments or a security review note in `docs/`.

## Boundaries

- Policy and regulatory mapping: [compliance-and-policy](../compliance-and-policy/SKILL.md).
