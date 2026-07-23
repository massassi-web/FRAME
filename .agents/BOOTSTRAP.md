# FRAME BOOTSTRAP

This document defines project  initialization procedures only.
It MUST NOT be used during runtime decision-making.

BOOTSTRAP is executed exactly once at project initialization.
After completion, it becomes immutable documentation and has no runtime authority. 


---

# SETUP

Create directory structure and files:
/
   .agents/
      AGENTS.md
      TASKS.md
      MEMORY.md
      ROADMAP.md
      skills/
   SPECS/            # Functional requirements, API contracts, design docs
   src/

---

# WORKFLOW

V - VISION
S - STACK
A - ARCHITECTURE
D - DATA
D - DESIGN 


Rules:
- complete one phase at a time
- never skip architecture
- never implement before requirements exist
- stop after every phase

---

# PHASE GUIDANCE RULE

When entering a phase:

1. Announce the current phase.
2. Explain the purpose of the phase.
3. Explain why the phase matters.
4. Describe the expected output.
5. Describe the key decisions that must be made.
6. Provide recommendations where appropriate.
7. Provide examples when useful.
8. Ask targeted questions.

The objective is to help the user make informed decisions and establish clear project requirements.

---

# PHASE REVIEW RULE

After receiving user input for a phase:

1. Summarize the user's decisions.
2. Identify assumptions.
3. Highlight potential risks or gaps.
4. Suggest improvements or alternatives.
5. Recommend a preferred approach.
6. Produce the phase output.

After the phase output is complete,
execute the Checkpoint Rule.

---

# CHECKPOINT RULE

Project initialization follows the
checkpoint process defined by AGENTS.md.

---

# QUALIFIED QUESTIONS RULE

Never ask vague or open-ended questions.

When multiple valid approaches exist:

1. Recommend a default solution.
2. Explain why it is recommended.
3. Present alternatives and tradeoffs.
4. Allow the user to override the recommendation.
5. Request confirmation.

Never force the user to choose from a blank slate.

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
- MVP visual scope

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

Before asking project questions:

1. Inspect the workspace.
2. Identify existing technologies.
3. Identify existing architecture patterns.
4. Reuse discovered context where possible.

Avoid asking questions that can be answered
through repository inspection.

Rules:
- existing architecture has priority over theoretical improvements
- prefer understanding before proposing changes
- preserve established patterns unless explicitly replaced

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
- .agents/AGENTS.md becomes runtime authority
- .agents/TASKS.md tracks execution
- .agents/MEMORY.md stores project knowledge
- .agents/ROADMAP.md tracks milestones
