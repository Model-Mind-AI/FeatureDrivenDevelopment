This is the Model Mind software development process for leveraging AI in VSCode, Cursor, and Claude Code.

This will be a plugin and should have the following skills:

[[Orchestration skills]]
[[Product and discovery skills]]
[[Architecture and design skills]]
[[Engineering implementation skills]]
[[Quality and validation skills]]
[[Security and compliance skills]]
[[Delivery and operations skills]]
[[Research]]
## Output
When using these skills they should output the following:
- any documentation to a /docs folder that is an obsidian vault
- any research of other products, technologies, etc should get saved in a /research folder
- all code should get created and managed in the /src folder
- /brand should hold all branding information like style guide and examples.
- /brand/images should hold any images that will be used in the application that is developed such as logos.

## Subagent taxonomy

Subagents should exist where specialization or parallel analysis clearly helps.

Use subagents for:

- parallel review
- specialized evaluation
- heavy analysis on separate concerns
- independent critique before synthesis

Do **not** use subagents for simple linear tasks.

### Recommended subagents

#### Cross-cutting specialist subagents

- **requirements-analyst**  
    Extracts actors, goals, constraints, edge cases, ambiguities.
- **architecture-critic**  
    Challenges coupling, scalability, resilience, and boundary choices.
- **security-analyst**  
    Focuses only on threats, auth, data exposure, secrets, misuse paths.
- **test-analyst**  
    Focuses only on test coverage, failure modes, and regression risk.
- **performance-analyst**  
    Focuses only on latency, throughput, contention, caching, scale bottlenecks.
- **compliance-analyst**  
    Focuses only on audit, privacy, retention, approval, and policy gaps.
- **code-reviewer**  
    Focuses only on maintainability, clarity, duplication, complexity, and style.
- **devops-analyst**  
    Focuses only on deployment, observability, rollback, environment drift.

#### Domain subagents

- **frontend-specialist**
- **backend-specialist**
- **database-specialist**
- **api-specialist**
- **integration-specialist**
- **cloud-specialist**
- **legacy-modernization-specialist**

---

## 4. Rules for when to use subagents

These should be global rules in the plugin.

### Use subagents when:

- the request spans multiple disciplines
- an artifact is high risk
- independent review improves quality
- multiple concerns can be analyzed in parallel
- a final synthesis is needed from multiple specialist perspectives

### Typical patterns

**Pattern 1: parallel review**  
For an architecture doc:

- architecture-critic
- security-analyst
- performance-analyst
- devops-analyst

Then synthesize into one recommendation.

**Pattern 2: design-to-build**  
For a feature request:

- requirements-analyst
- solution-architect
- test-analyst

Then hand to feature-implementer.

**Pattern 3: defect triage**  
For a bug:

- debug-and-root-cause
- test-analyst
- code-reviewer

Then synthesize likely cause and fix plan.

### Avoid subagents when:

- the task is small
- the cost of orchestration exceeds the benefit
- the work is purely editorial
- there is no clear specialist boundary

---

## 5. Shared operating rules for all skills

These are the core enterprise rules every skill follows.

### A. Lifecycle alignment

Every skill should preserve alignment across:

- business objective
- requirements
- architecture
- implementation
- testing
- deployment
- observability
- security

### B. Traceability

Every major output should answer:

- what requirement does this support?
- what assumptions does it rely on?
- what dependencies exist?
- what tests prove it?
- what operational signals will validate it in production?

### C. Secure by default

Every skill should assume:

- least privilege
- input validation
- output encoding
- secret isolation
- authenticated and authorized access
- auditability where relevant
- no insecure defaults

### D. Production readiness

Every substantial implementation should consider:

- error handling
- retries/timeouts
- telemetry
- rollback
- config separation
- idempotency where relevant
- failure-mode analysis

### E. Enterprise documentation minimum

For meaningful work, generate or update:

- requirement artifact
- design note or architecture note
- implementation plan
- test approach
- deployment/release impact
- operational considerations

### F. Change impact awareness

Whenever something changes, identify what else must be reviewed:

- requirements
- stories
- API contracts
- schemas
- tests
- docs
- deployment config
- monitoring

### G. Human escalation rules

Skills should explicitly flag:

- ambiguous business decisions
- security-risk decisions
- irreversible migration choices
- compliance-sensitive changes
- breaking public contract changes
- production hotfixes with elevated risk

---

## 6. Host compatibility rules for VSCode, Cursor, and Claude Code

These skills should be written to be **host-neutral** first.

### Host-neutral design principles

- do not rely on one IDE’s proprietary UI
- prefer plain text inputs and outputs
- assume access to files, folders, diffs, and terminals may vary
- keep artifact generation filesystem-friendly
- use markdown, yaml, json, and code blocks as default interfaces
- avoid host-specific assumptions unless gated by host detection rules

### Compatibility model

#### A. VSCode

Best for:

- file-aware workflows
- extension-driven commands
- task execution
- integrated terminal operations

Design assumptions:

- repo context may be available
- command palette patterns may be useful
- file-scoped actions and workspace actions should be supported

#### B. Cursor

Best for:

- codebase-aware generation and editing
- multi-file implementation workflows
- code modification loops
- inline coding assistance

Design assumptions:

- strong repo/code context
- request often starts from selected code or current file
- implementation and refactor skills should optimize for existing code context

#### C. Claude Code

Best for:

- repo reasoning
- terminal-driven workflows
- architecture/code synthesis
- deep debugging and refactor analysis

Design assumptions:

- file tree and terminal may be central
- long-form reasoning workflows matter
- implementation plans and code-review-style skills work especially well

### Host adaptation rule

Each skill should have:

- a **core workflow**
- optional **host-specific invocation patterns**

Example:  
`feature-implementer`

- core: plan change, identify files, implement, test, summarize
- VSCode mode: workspace task and file-scoped suggestions
- Cursor mode: selected code and multi-file edit workflow
- Claude Code mode: repo scan, terminal-backed validation, patch summary

---

## 7. Recommended plugin rules section

Your umbrella plugin should include a rules file that says something like this in substance:

### Global plugin rules

- Use the smallest skill that fully owns the problem.
- Invoke subagents only when specialization adds value.
- Preserve traceability from requirement to release.
- Prefer revising existing artifacts over creating duplicates.
- Optimize for secure, maintainable, production-ready output.
- Make host behavior portable across VSCode, Cursor, and Claude Code.
- Separate fact, assumption, risk, and recommendation in major outputs.
- Flag uncertainty explicitly.
- Never finalize architecture, security, migration, or deployment recommendations without surfacing key tradeoffs.

---

## 8. How to package this practically

I would organize it like this:

### Option A: one umbrella plugin with many skills

Best if you want a single installable system.

Structure:

- shared rules
- shared templates
- all skills
- all subagent definitions
- host compatibility references

### Option B: one core plugin plus capability packs

Best if you want modular adoption.

Example packs:

- `software-factory-core`
- `software-factory-product-design`
- `software-factory-engineering`
- `software-factory-quality-security`
- `software-factory-devops`

For enterprise use, this is often the best long-term structure.

---

## 9. My recommendation for version 1

Start with these 12 as the core set:

- software-delivery-orchestrator
- enterprise-standards-enforcer
- product-features
- solution-architect
- api-designer
- data-model-designer
- codebase-analyzer
- implementation-planner
- feature-implementer
- test-strategy
- secure-code-review
- ci-cd-designer

Then add subagents:

- requirements-analyst
- architecture-critic
- security-analyst
- test-analyst
- performance-analyst
- devops-analyst

That gives you a very strong enterprise baseline without overbuilding.

## 10. Recommended command-style capability model

You asked earlier whether capabilities should be separate skills. For this suite, I would use:

- **skills = domains**
- **commands/modes = operations within a domain**

Example for `product-features`:

- create
- edit
- expand
- critique
- decompose
- validate

Example for `solution-architect`:

- design
- revise
- compare
- harden
- simplify
- review tradeoffs

That keeps the taxonomy clean.

## 11. The next artifact to define

The most useful next step is to define this suite in a real feature document with these columns:

- skill name
- purpose
- triggers
- inputs
- outputs
- internal operations
- subagents used
- host notes for VSCode/Cursor/Claude Code
- boundaries with other skills

I can draft that next as a full **plugin architecture feature document v1** in a table or in a structured document format.