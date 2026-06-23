# FRAME+CORE

Immutable AI engineering kernel.

Purpose:
- preserve architectural integrity
- reduce hallucinations
- maintain long-term consistency
- optimize autonomous development

---

# PRIORITY ORDER

1. Architectural integrity
2. Simplicity
3. Reusability
4. Maintainability
5. Performance
6. Developer convenience

Higher-priority rules override lower-priority rules.

---

# DECISION MAKING

When blocked or when multiple valid solutions exist:

1. Define the problem.
2. Present three viable options.
3. Compare tradeoffs.
4. Recommend one option.
5. Wait for user approval.

(1-3-1 Technique)

---

# CORE RULES

## Architecture
- Never violate layer boundaries
- Never place business logic in UI
- Reuse before creating new systems
- Prefer extension over rewrites
- Avoid duplicate implementations
- Preserve composability

---

## DRY PRINCIPLE

Before creating:

- components
- services
- utilities
- abstractions

Search for existing implementations first.

Prefer extension over duplication.

Duplicate business logic is forbidden except where decoupling explicitly overrides reuse.

---

## Complexity
- Prefer the simplest viable solution
- Avoid premature optimization
- Avoid unnecessary abstractions
- Minimize dependencies
- Avoid enterprise patterns unless justified

---

## Consistency
- Follow existing architecture
- Follow existing naming conventions
- Preserve design system consistency
- Preserve API consistency
- Preserve folder structures

---

## Safety
- Never store secrets insecurely
- Validate external input
- Fail predictably
- Preserve backward compatibility when possible
- Never bypass security systems

---

## Scope expansion rules
Never introduce:
- additional systems
- abstractions
- optimizations
- features
unless explicitly requested.

---

# DEFAULT ANT LAYER MODEL

Use this model unless the project defines
a more specific architecture.

## 1. Intent Layer
Allowed:
- rendering
- input handling
- intent capture

Forbidden:
- business logic
- DB access
- orchestration logic

---

## 2. Orchestration Layer
Allowed:
- workflows
- state transitions
- business coordination

Forbidden:
- rendering
- infrastructure operations

---

## 3. Execution Layer
Allowed:
- DB operations
- APIs
- external effects
- filesystem
- queues

Forbidden:
- UI concerns
- orchestration logic

---

# EXECUTION PROTOCOL

Before implementation:
1. Read relevant docs
2. Load only memory relevant to the affected system or task.
3. Identify impacted systems
4. Preserve architecture
5. Implement minimally
6. Verify behavior
7. Update documentation

---

# PLANNING PROTOCOL

For tasks involving multiple steps:

1. Analyze scope.
2. Create an execution plan.
3. Create a task list.
4. Identify dependencies and risks.
5. Obtain approval when appropriate.
6. Execute sequentially.

Do not begin implementation before planning is complete.

---

# FAILURE PROTOCOL

On failure:
1. diagnose
2. isolate
3. repair minimally
4. verify
5. retry

Avoid rewrites unless necessary.

---

# CONTEXT LOADING PROTOCOL
Always load context strictly depending on the current task:

## For Feature Implementation & Code Maintenance:
- Load CORE.md
- Load relevant requirements
- Load relevant architecture documents
- Load active tasks

---

# FILE NAMING RULES

Use deterministic naming for applicable documents.

---

# DOCUMENTATION RULES

Documentation must be:
- concise
- implementation-ready
- AI-readable
- human-readable
- deterministic

Avoid:
- vague language
- unnecessary theory
- duplicated explanations

---

# CODE STANDARDS

Required:
- type safety
- input validation
- predictable error handling (prefer explicit error returns/results over throwing generic exceptions)
- Prefer native features
- explicit edge-case logging

Avoid:
- tightly coupled systems
- hidden side effects
- duplicated business logic
- magic values
- inconsistent naming
  
---

# TESTING STRATEGY

For backend and business logic:

1. Review existing tests first.
2. Prefer test-first development.
3. Add or modify tests before implementation.
4. Follow established testing patterns.

Avoid excessive test generation.

Testing effort should match implementation risk.

---

# DESIGN CONSISTENCY

UI systems must:
- follow shared design tokens
- preserve spacing consistency
- preserve typography consistency
- preserve interaction consistency
- support accessibility

---

# REFACTORING RULES

Prefer:
- incremental refactors
- isolated changes
- backward compatibility

Avoid:
- large rewrites
- unnecessary migrations
- architecture churn

---

# CHECKPOINT RULE

After completing any phase, task, or significant work unit:

1. Summarize completed work.
2. List generated or modified files.
3. List key decisions made.
4. Identify outstanding assumptions or risks.
5. Request explicit approval.
6. STOP immediately.

If the user provides feedback instead of "YES",
iterate on the current work unit and generate
a new checkpoint.

Forbidden:
- continuing to the next task automatically
- performing work outside the approved scope
- generating future-phase documents
- asking next-step questions

The response must terminate immediately after
the approval request.

Required approval format:

"Do you approve this? Reply YES to continue."

--- 

# TASK MANAGEMENT

Purpose:
Track active and planned work.

Tasks must contain:
- objective
- status
- dependencies
- acceptance criteria

Statuses:
- TODO
- IN_PROGRESS
- BLOCKED
- DONE

---

# MEMORY

Purpose:
Store persistent project knowledge that may be
useful across tasks and sessions.

Contains:
- project facts
- domain knowledge
- assumptions
- discovered constraints
- terminology
- external system knowledge

Must NOT contain:
- active tasks
- roadmap items
- architecture definitions
- implementation plans
- temporary discussions

Authority:
CORE.md defines architecture.
TASKS.md defines active work.
ROADMAP.md defines future work.

MEMORY.md stores knowledge only.

---

# CONTINUOUS LEARNING

When discovering:

- undocumented behavior
- architectural decisions
- project constraints
- conflicting documentation
- recurring implementation patterns

Propose updates to project documentation.

Never modify governance documents without approval.

Knowledge gained during execution should be preserved.

---

# PROJECT DOCUMENT MAINTENANCE

Project governance documents must remain current.

Documentation updates are part of completing work,
not a separate optional activity.

TASKS.md
- update when tasks are created, started, blocked, completed, or modified

MEMORY.md
- update when persistent project knowledge is discovered
- update when assumptions become established facts
- update when architectural decisions are finalized

ROADMAP.md
- update when milestones, releases, or long-term goals change

Before generating a checkpoint:

1. Update all affected governance documents.
2. Verify document consistency.
3. Generate the checkpoint.

Avoid stale documentation.

Governance documents must reflect the current
project state before any checkpoint is generated.

