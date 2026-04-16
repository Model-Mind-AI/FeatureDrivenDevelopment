#### 22. `test-strategy`

**Purpose:** Define the test approach for the solution.  
**Use for:** coverage planning, risk-based test design, test pyramid decisions.  
**Owns:**

- test levels
- automation strategy
- regression planning
- traceability to requirements

#### 23. `test-generator`

**Purpose:** Generate concrete tests from code and requirements.  
**Use for:** unit tests, integration tests, API tests, UI tests, regression tests.  
**Owns:**

- test case generation
- fixtures
- mocks
- happy path and edge case coverage

#### 24. `qa-reviewer`

**Purpose:** Critique readiness from a QA perspective.  
**Use for:** test gap analysis, acceptance criteria validation, release readiness review.  
**Owns:**

- missing test coverage
- ambiguity detection
- defect-prone scenario review

#### 25. `debug-and-root-cause`

**Purpose:** Diagnose failures and propose grounded fixes.  
**Use for:** runtime bugs, CI failures, production defects, flaky tests.  
**Owns:**

- symptom analysis
- hypothesis trees
- reproduction design
- root cause isolation

#### 26. `observability-designer`

**Purpose:** Ensure software is measurable and diagnosable.  
**Use for:** logs, traces, metrics, alerts, dashboards, diagnostics.  
**Owns:**

- telemetry design
- structured logging
- SLO-aligned metrics
- alert design
- post-release visibility