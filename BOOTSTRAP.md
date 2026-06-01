# FRAME BOOTSTRAP

This document defines project  initialization procedures only.
It MUST NOT be used during runtime decision-making.

BOOTSTRAP is executed exactly once at project initialization.
After completion, it becomes immutable documentation and has no runtime authority. 


---

# SETUP

Create directory structure and files:
/
   CORE.md
   TASKS.md
   MEMORY.md
   ROADMAP.md
   SPECS/
   src/

---

# WORKFLOW

V - Project VISION
S - Project STACK
A - Project ARCHITECTURE
D - Project DATA
D - Project DESIGN 


Rules:
- complete one phase at a time
- never skip architecture
- never implement before requirements exist
- stop after every phase

---

# CHECKPOINT RULE

After completing ANY phase or sub-phase:

1. summarize outputs
2. list generated files
3. request explicit approval
4. STOP immediately

Forbidden:
- continuing automatically
- generating future-phase documents
- implementing features
- asking next-phase questions

Required approval format:
"Do you approve this phase? Reply YES to continue."

---

# QUALIFIED QUESTIONS RULE

Never ask vague or open-ended questions.

Always:
- provide recommendations
- explain tradeoffs
- propose sensible defaults
- guide decision-making

Preferred structure:
1. recommendation
2. reasoning
3. alternatives
4. confirmation request

---


Existing architecture has priority over theoretical improvements.

---

# PHASE OUTPUTS

## Vision
- project summary
- MVP definition
- scope boundaries
- success criteria

## Stack
- selected technologies
- tradeoff analysis
- dependency rationale

## Architecture
- architecture summary
- folder structure
- data flow overview
- service boundaries

## Data
- core entities
- relationships
- persistence strategy

## Design
- design direction
- UI principles
- interaction priorities

---

# RESPONSE STYLE

Be:
- concise
- technical
- strategic
- implementation-oriented

Avoid:
- fluff
- speculative architecture
- premature coding
- unnecessary verbosity

---

# WORKSPACE ANALYSIS

Before asking questions:

Inspect:
- repository structure
- frameworks
- configs
- package managers
- deployment configs
- architecture patterns

Examples:
- package.json
- Cargo.toml
- docker-compose.yml
- next.config.js
- ios/
- android/

---

# COMPLETION

Upon completion:
- CORE.md becomes runtime authority
- TASKS.md tracks execution
- MEMORY.md stores project knowledge
- ROADMAP.md tracks milestones
