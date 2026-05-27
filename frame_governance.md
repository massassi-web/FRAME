# FRAME GOVERNANCE

Repository standards and consistency rules.

## Rule Supremacy In case of any ambiguity or conflict between these standards and FRAME+CORE, the PRIORITY ORDER and rules defined in FRAME+CORE strictly override this document. 

---

# DIRECTORY STRUCTURE

```text
/core
/bootstrap
/governance

/docs
  /foundation
  /requirements
  /architecture
  /mood-design
  /execution-infrastructure
  /decisions

/modules
/src
```

---

# FILE NAMING RULES

Use deterministic naming.

Required:
- 01_FOUNDATIONS.md
- 02_USER_FLOWS.md
- 03_REQUIREMENTS.md
- 04_ARCHITECTURE.md
- 05_DATABASE_SCHEMA.md
- 06_DESIGN_SYSTEM.md
- 07_INFRASTRUCTURE.md
- 08_ROADMAP.md

Never invent alternative names.

Forbidden:
- foundation-doc.md
- architecture_v2.md
- misc-notes.md

---

# ADR RULES

All major decisions require ADRs.

Required for:
- authentication
- database strategy
- rendering strategy
- state management
- infrastructure changes
- external integrations

---

# ADR FORMAT

```text
ADR-001-title.md
```

Required sections:
- Status
- Context
- Decision
- Consequences
- Alternatives

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

