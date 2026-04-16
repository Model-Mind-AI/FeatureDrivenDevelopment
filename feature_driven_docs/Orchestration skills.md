These coordinate work across the lifecycle.

#### 1. `software-delivery-orchestrator`

**Purpose:** Route a request to the right workflow, skill, and subagents.  
**Use for:** “Build this feature,” “Help me deliver this project,” “Take this from idea to release.”  
**Owns:**

- task classification
- workflow selection
- artifact dependency tracking
- handoff between skills
- deciding when to invoke subagents

#### 2. `artifact-governance`

**Purpose:** Keep requirements, design, code, tests, and deployment artifacts aligned.  
**Use for:** checking consistency across features, architecture docs, stories, code, and tests.  
**Owns:**

- traceability
- version alignment
- change impact analysis
- “what must be updated because this changed?”

#### 3. `enterprise-standards-enforcer`

**Purpose:** Apply organizational rules across all outputs.  
**Use for:** architecture standards, secure coding rules, naming rules, compliance, documentation standards.  
**Owns:**

- style and standards
- secure defaults
- enterprise architecture conventions
- documentation and review rules