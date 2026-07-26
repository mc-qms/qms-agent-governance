# Semantic Primitives
**The primitive behavioral vocabulary for QMS AI Agents.**

This document provides the primitive behavioral vocabulary for designing AI agent instructions in a Quality Management System (QMS).

These concepts are intentionally presented as **semantic primitives** rather than complete instructions. Each concept functions as a high-information token that leverages an LLM's existing semantic understanding of logic, compliance, and systems design. Their purpose is to provide high-level behavioral anchors that can be expanded with an LLM into organization-specific instruction sets, workflows, and implementation patterns.

> **Implementation Note:** Applying these primitives in tandem with the specific operational needs of your intended agent is required to achieve successful governance. The brief annotations provided below are not definitions—they are **disambiguations** designed to steer the LLM toward a specific operational behavior.

---

## 1. Identity & Scope
These primitives establish the foundational boundaries of what the agent is, what authority it possesses, and how it presents itself.

* **Persona (Purpose & Scope)**
* **Modal Context Gating**
* **Tone**
* **Tense**

---

## 2. Knowledge & Boundaries
These primitives govern where the agent sources its information and what external context it is permitted to use or ignore.

* **Knowledge Sources (RAG)**
* **Source of Truth Boundaries**
* **Closed Context**
* **Read Documents First**
* **Use Templates Over Defaults**

---

## 3. Reasoning & Logic & Integrity
These primitives dictate how the agent processes information, handles gaps in data, and strictly applies compliance constraints.

* **Zero Inference**
* **Negative Constraints**
* **ALCOA+**
* **Error-Triggered Pushback**

---

## 4. Workflow Execution
Depending on the risk level and phase of the workflow, these primitives govern pacing, task management, and halting conditions.

* **Mandatory Context Halt**
    * Pause execution and require human intervention if fundamental prerequisite data or core regulatory context is entirely missing.
* **Don't Halt, Flag Gaps**
    * Continue processing available data while explicitly tagging minor missing or non-compliant information for human review.
* **Queue Tracker**
    * Maintain a rolling state of unresolved agenda items across multiple turns until the human operator explicitly clears them.

---

## 5. Documentation & Compliance
Because LLMs naturally tend to embellish and reformat text, these primitives ensure historical accuracy and proportionate output.

* **Proportionate Writing with Omissions**
    * Treat the template as a ceiling; right-size the document to the actual risk and leave non-applicable sections entirely blank.
* **Material-Bound History Conservation**
    * Rules, limits, and cumulative stress histories attach to the physical material itself and transfer with it, independent of container or document changes.

  ---

### These primitives are not intended to be universally applied. Selection and expansion should be based on the intended workflow, risk profile, and organizational requirements of the target agent.
