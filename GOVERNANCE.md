# FRAME GOVERNANCE

Repository standards and consistency rules.

## Rule Supremacy In case of any ambiguity or conflict between these standards and FRAME+CORE, the PRIORITY ORDER and rules defined in FRAME+CORE strictly override this document. 

---

# FILE NAMING RULES

Use deterministic naming for applicable documents.

---

# KNOWLEDGE SEPARATION

Architecture belongs in CORE.md
Project knowledge belongs in MEMORY.md
Active work belongs in TASKS.md
Future work belongs in ROADMAP.md

Do not duplicate information across files.

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

After completing ANY phase or sub-phase:

1. summarize outputs
2. list generated files
3. request explicit approval
4. STOP immediately
5. If user provides feedback instead of "YES", iterate on the current step and generate a new checkpoint.

Forbidden:
- continuing automatically
- generating future-phase documents
- implementing features
- asking next-phase questions

Required approval format:
"Do you approve this? Reply YES to continue."

--- 

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
