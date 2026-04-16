#### 8. `solution-architect`

**Purpose:** Design the full technical solution.  
**Use for:** system architecture, service boundaries, deployment models, integration design.  
**Owns:**

- architecture options
- tradeoff analysis
- domain boundaries
- system context
- component interactions

#### 9. `api-designer`

**Purpose:** Design APIs and service contracts.  
**Use for:** REST, GraphQL, RPC, webhooks, contract design.  
**Owns:**

- endpoint design
- schema design
- versioning
- error models
- idempotency
- auth considerations

#### 10. `data-model-designer`

**Purpose:** Design persistence and data movement.  
**Use for:** database schema, entity relationships, event schemas, reporting models.  
**Owns:**

- domain entities
- storage choices
- indexing
- migration planning
- retention rules

#### 11. `integration-architect`

**Purpose:** Design external and internal integrations.  
**Use for:** third-party APIs, enterprise systems, queues, event buses, auth flows.  
**Owns:**

- system contracts
- retries
- failure modes
- sync vs async patterns
- integration hardening

#### 12. `security-architecture`

**Purpose:** Define secure design before implementation.  
**Use for:** threat modeling, trust boundaries, authn/authz design, secrets strategy.  
**Owns:**

- threat models
- attack surface mapping
- data sensitivity zones
- privileged access patterns
- security controls by layer

#### 13. `performance-and-scalability-architect`

**Purpose:** Design for scale, resilience, and latency.  
**Use for:** load design, bottleneck analysis, concurrency, caching, queueing.  
**Owns:**

- scale assumptions
- performance budgets
- resilience strategies
- capacity planning inputs