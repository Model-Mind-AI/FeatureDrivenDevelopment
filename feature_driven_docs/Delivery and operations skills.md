#### 30. `ci-cd-designer`

**Purpose:** Design build, test, release, and promotion pipelines.  
**Use for:** GitHub Actions, Azure DevOps, GitLab CI, release gating, artifact promotion.  
**Owns:**

- pipeline stages
- gates
- branch/release rules
- deployment workflow design

#### 31. `deployment-engineer`

**Purpose:** Prepare deployment configuration and rollout strategy.  
**Use for:** app deployment, infra hooks, blue-green/canary, rollback design.  
**Owns:**

- release strategy
- env promotion
- config safety
- rollback mechanics

#### 32. `infrastructure-as-code`

**Purpose:** Design and critique infra definitions.  
**Use for:** Terraform, Bicep, CloudFormation, Kubernetes manifests, environment config.  
**Owns:**

- infra modularity
- environment parity
- secret handling
- least privilege infra patterns

#### 33. `release-manager`

**Purpose:** Coordinate release readiness and production cutover.  
**Use for:** go-live checklists, release notes, risk reviews, deployment windows.  
**Owns:**

- release checklist
- stakeholder readiness
- deployment runbooks
- rollback go/no-go logic

#### 34. `incident-response`

**Purpose:** Guide production incident triage and stabilization.  
**Use for:** outages, degraded performance, error spikes, rollback or hotfix decisions.  
**Owns:**

- severity framing
- triage flow
- containment steps
- communication guidance
- immediate corrective action