---
name: software-delivery-orchestrator
description: >-
  Classifies requests, picks workflows, tracks artifact dependencies, and hands
  off to the right Model Mind skills or subagents. Use for “build this feature,”
  “take this from idea to release,” or coordinating multi-phase delivery—not
  for tiny one-file edits unless routing is unclear.
---

# Software delivery orchestrator

## When to use this skill

- The user wants end-to-end delivery guidance or does not know which skill applies.
- Work spans requirements, design, implementation, testing, or release.
- Parallel specialist review would add value (see [model-mind-foundations](../model-mind-foundations/SKILL.md)).

## Instructions

1. **Classify** the request: greenfield feature, change to existing behavior, fix, refactor, release, or research.
2. **Inventory** what already exists under `docs/`, `research/`, and `src/` relevant to the ask.
3. **Choose** the smallest set of skills that fully own the problem; avoid invoking many skills for a trivial task.
4. **Sequence** work: clarify requirements and scope before deep architecture; align architecture before broad implementation.
5. **Hand off** with a short brief: goal, constraints, artifacts to read or create, and the next skill’s deliverable.
6. **Subagents**: propose parallel review when the artifact is high-risk or multi-disciplinary; synthesize one outcome after reviews.

## Outputs

- A routing plan (which skills, in what order) saved or appended under `docs/` when the plan is non-trivial.
- Optional checklist of artifacts to create or update under `docs/` and `research/`.

## Boundaries

- Does not replace domain skills: it coordinates them.
- Does not silently bypass human escalation rules in [model-mind-foundations](../model-mind-foundations/SKILL.md).
