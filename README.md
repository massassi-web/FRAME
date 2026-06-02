# FRAME

**FRAME** is a lightweight governance framework for AI-assisted software development.

It helps AI coding agents maintain architectural consistency, reduce scope creep, avoid unnecessary complexity, and preserve project knowledge across long-running projects.

FRAME separates **project initialization** from **project execution** through two core documents:

* **BOOTSTRAP.md** — initializes the project
* **CORE.md** — governs engineering decisions after initialization

The framework is intentionally small and tool-agnostic. It can be used with any AI coding assistant, regardless of model or platform.

---

## Project Structure

```text
/
├─ BOOTSTRAP.md
├─ CORE.md
├─ TASKS.md
├─ MEMORY.md
├─ ROADMAP.md
├─ SPECS/
└─ src/
```

| File           | Purpose                                                           |
| -------------- | ----------------------------------------------------------------- |
| `BOOTSTRAP.md` | Defines the project initialization workflow.                      |
| `CORE.md`      | Defines architectural principles, standards, and execution rules. |
| `TASKS.md`     | Tracks active and planned work.                                   |
| `MEMORY.md`    | Stores persistent project knowledge and decisions.                |
| `ROADMAP.md`   | Tracks long-term goals and milestones.                            |

---

## Why FRAME?

AI coding agents often struggle with:

* architectural drift
* duplicate implementations
* unnecessary abstractions
* uncontrolled scope expansion
* inconsistent decisions across sessions

FRAME introduces a small set of rules that help maintain consistency throughout the lifecycle of a project.

---

## Initialization Workflow

Projects are initialized through five sequential phases:

```text
Vision → Stack → Architecture → Data → Design
```

Each phase must be approved before the next phase begins.

This ensures that implementation never starts before requirements, architecture, and data models are properly defined.

---

## Core Principles

Priority order:

1. Architectural Integrity
2. Simplicity
3. Reusability
4. Maintainability
5. Performance
6. Developer Convenience

Higher-priority principles always override lower-priority principles.

---

## The ANT Layer Model

FRAME uses a simple three-layer architecture by default.

### Intent Layer

Responsible for:

* rendering
* input handling
* intent capture

### Orchestration Layer

Responsible for:

* workflows
* business coordination
* state transitions

### Execution Layer

Responsible for:

* databases
* APIs
* filesystem access
* external effects

Unless a project defines a different architecture, the ANT model is the default structure.

---

## Starting a New Project

To initialize a FRAME project:

Create the FRAME directory structure.
Add the governance files to the project root.
Load BOOTSTRAP.md into the AI assistant.
Begin with the Vision phase.
Progress sequentially through the initialization workflow.
Obtain approval at every checkpoint.

Example initialization prompt:

```text
Read BOOTSTRAP.md and initialize the project.

Inspect the workspace for existing files and architecture.

Begin with the Vision phase and follow the initialization workflow exactly.

Stop at the first checkpoint and wait for approval before continuing.
```

---

## Design Philosophy

FRAME is built around a small set of engineering principles:

* Preserve architectural integrity
* Prefer simplicity over complexity
* Reuse before creating new systems
* Extend before rewriting
* Minimize unnecessary abstractions
* Maintain long-term consistency

The framework intentionally remains lightweight and tool-agnostic, allowing it to be used with any AI coding assistant or development environment.

---

## License

MIT License
