# FRAME: AI-Assisted Engineering Framework

FRAME is a minimalist, deterministic governance framework designed for "vibe coding" and autonomous AI development workflows. Its primary objective is to preserve absolute architectural integrity, systematically mitigate LLM hallucinations, and enforce a strict, phase-gated lifecycle across long-term project lifespans.

---

## 🏗️ System Architecture

The repository's structural governance is partitioned into four core operational files, each maintaining clear boundaries of context and authority:

| File | Execution Lifecycle | Operational Authority & Core Purpose |
| :--- | :--- | :--- |
| `BOOTSTRAP.md` | Initialization Only | Governs the one-time project initialization phases (V-S-A-D-D). Retains zero runtime authority upon completion and becomes immutable historical documentation. |
| `CORE.md` | Runtime Context | The central architectural law. Encapsulates immutable invariant rules, multi-layer ANT constraints, standards, and the checkpoint protocol. |
| `TASKS.md` | Active Context | Tracks the precise status, objectives, explicit dependencies, and strict acceptance criteria for active and planned engineering sprints. |
| `MEMORY.md` | Persistent Knowledge | A purely factual data sink. Aggregates discovered domain knowledge, physical constraints, terminology, and external integrations. Holds zero execution or planning authority. |

---

## 🚦 Initialization Lifecycle & Workflow (V-S-A-D-D)

Initial project bootstrapping must process linearly through five non-skippable developmental gates. No implementation or forward phase progression may occur until the active phase output criteria are finalized:

[V] Vision ➔
[S] Stack ➔
[A] Architecture ➔
[D] Data ➔
[D] Design

[CHECKPOINT RULE] ➔ Halt & Require Explicit "YES"

* **V - Project Vision:** High-level project intent, clear MVP parameter boundaries, scope isolation, and explicit criteria for success.
* **S - Project Stack:** Definitive technology selections, rigorous trade-off analyses, and structural dependency rationale.
* **A - Project Architecture:** Formal structural baseline, complete directory hierarchy mapping, system data-flows, and interface boundaries.
* **D - Project Data:** Mapping of core data entities, structural relational topologies, and concrete persistence mechanics.
* **D - Project Design:** Core visual direction guidelines, underlying UI tokens, interaction mechanics, and constrained MVP screen scope.

---

## 🚦 The Invariant Rules of AI Engagement

Autonomous agents operating within a FRAME repository must comply with three mechanical integration laws at all times:

### 1. The Checkpoint Protocol
Immediately upon finishing any phase, sub-phase, or task block, the agent must completely halt all processing. It is explicitly forbidden to execute speculative optimizations, generate next-phase documentation, or touch code assets. The agent must return a highly structured output and ask: 
`"Do you approve this? Reply YES to continue."`

### 2. Qualified Questions Protocol
Vague, open-ended, or ambiguous diagnostic inquiries are entirely prohibited. When prompting for human intervention, the agent must formulate a decisive direction using a strict conversational blueprint:
1. **Recommendation:** Present a definitive, singular default technical action block.
2. **Reasoning:** Provide structured technical justification and target architectural impact.
3. **Alternatives:** Detail alternative architectural tradeoffs, performance differentials, or stack costs.
4. **Confirmation Request:** Issue a binary gate block requiring explicit user authorization.

### 3. Scope Expansion Rules
Agents are strictly locked out from incorporating unrequested external systems, new design libraries, secondary abstractions, or forward-looking optimizations. Engineering execution must optimize solely for the minimal viable path required to satisfy the immediate acceptance criteria defined in `TASKS.md`.

---

## 📐 Architectural Paradigm: The ANT Layer Model

By default, unless overwritten by an explicit system design layout inside the architectural specs, all functional logic adheres to a decoupled three-tier hierarchy called the **ANT Layer Model**:

### 1. Intent Layer
* **Allowed:** Presentational state rendering, primitive user input handling, and initial intent capture components.
* **Forbidden:** Embedding domain business rules, direct persistence interaction, or multi-service orchestration.

### 2. Orchestration Layer
* **Allowed:** Domain business workflows, programmatic state transitions, and coordination across execution boundaries.
* **Forbidden:** Direct UI asset rendering, low-level database operations, or explicit infrastructure I/O side effects.

### 3. Execution Layer
* **Allowed:** Atomic database queries, low-level network API clients, filesystem read/writes, message queues, and peripheral hardware integrations.
* **Forbidden:** Presentational visual layers, active session orchestration, or application workflow configuration context.

---

## 🚀 Bootstrapping a New Repository

To initialize an empty repository under FRAME governance, mount the four root framework files into the project root and feed the following instruction to the incoming LLM context windows:

> "Inspect workspace infrastructure files if any exist. Read and process `BOOTSTRAP.md` to initialize the project strictly following the 'V - Project VISION' specifications. Generate all phase outputs, structure the system boundary definition, and HALT immediately at the checkpoint gate. Do not step forward without explicit verification."
