#### 14. `codebase-analyzer`

**Purpose:** Understand an existing codebase before changes.  
**Use for:** legacy systems, unfamiliar repos, dependency mapping, “where should this change go?”  
**Owns:**

- code structure analysis
- dependency graph reasoning
- architectural drift detection
- hotspot identification

#### 15. `implementation-planner`

**Purpose:** Turn approved design into a concrete technical execution plan.  
**Use for:** task plans, file-by-file change plans, migration steps, rollout phases.  
**Owns:**

- implementation sequence
- interfaces to change
- migration steps
- rollback-aware planning

#### 16. `feature-implementer`

**Purpose:** Build new features aligned to requirements and architecture.  
**Use for:** scaffolding, feature coding, endpoint creation, UI implementation, service logic.  
**Owns:**

- code generation
- incremental implementation
- feature completeness
- alignment to acceptance criteria

#### 17. `refactor-engineer`

**Purpose:** Improve code structure without changing behavior.  
**Use for:** cleanup, modularization, reducing complexity, removing duplication.  
**Owns:**

- safe refactor plans
- dependency untangling
- naming and boundary improvement
- technical debt reduction

#### 18. `legacy-modernization`

**Purpose:** Upgrade older systems safely.  
**Use for:** framework upgrades, platform migrations, decomposition, strangler patterns.  
**Owns:**

- modernization roadmap
- compatibility risks
- phased migration
- coexistence strategy

#### 19. `frontend-engineer`

**Purpose:** Implement UI and client behavior to enterprise standards.  
**Use for:** component architecture, state management, validation, accessibility-aware frontends.  
**Owns:**

- UI structure
- state flows
- error states
- accessibility implementation
- performance-sensitive client patterns

#### 20. `backend-engineer`

**Purpose:** Implement services, APIs, jobs, and domain logic.  
**Use for:** business logic, services, orchestration, persistence, background processing.  
**Owns:**

- domain services
- service boundaries
- persistence interactions
- background work design

#### 21. `platform-engineer`

**Purpose:** Build shared platform capabilities and reusable developer foundations.  
**Use for:** internal SDKs, shared libraries, scaffolds, service templates, platform hooks.  
**Owns:**

- cross-cutting engineering foundations
- reusable primitives
- template and boilerplate standards