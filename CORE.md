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

# CORE RULES

## Architecture
- Never violate layer boundaries
- Never place business logic in UI
- Reuse before creating new systems
- Prefer extension over rewrites
- Avoid duplicate implementations
- Preserve composability

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
2. Load relevant MEMORY.md
3. Identify impacted systems
4. Preserve architecture
5. Implement minimally
6. Verify behavior
7. Update documentation

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
- error handling
- avoid magic values

Avoid:
- tightly coupled systems
- hidden side effects
- duplicated business logic
- magic values
- inconsistent naming

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

# TASK MANAGEMENT

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
