---
name: performance-and-scalability-architect
description: >-
  Designs for scale, resilience, and latency: load assumptions, performance
  budgets, concurrency, caching, queues, capacity inputs. Use when performance or
  scale is a primary risk or requirement.
---

# Performance and scalability architect

## When to use this skill

- Expected load, spikes, or strict latency goals.
- Suspected bottlenecks or need for horizontal scaling strategy.

## Instructions

1. **Establish** workload profiles and performance budgets (latency, throughput).
2. **Analyze** likely bottlenecks and contention points; propose caching, queues, sharding, or scaling patterns as appropriate.
3. **Define** resilience strategies: backpressure, degradation, timeouts.
4. **Provide** capacity planning inputs; tie observability needs to [observability-designer](../observability-designer/SKILL.md).
5. **Document** under `docs/` with explicit assumptions.

## Outputs

- Performance and scalability notes in `docs/`.

## Boundaries

- Load testing execution belongs with project tooling; this skill focuses on design and criteria.
