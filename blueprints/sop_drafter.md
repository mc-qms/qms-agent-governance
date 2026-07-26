# Blueprint: SOP Drafting Assistant

This blueprint demonstrates how to compile an instruction set for a highly controlled documentation assistant. It is designed to take raw Subject Matter Expert (SME) notes, equipment manuals, or legacy procedures and format them into an SOP draft following organization-defined formatting and documentation requirements.

# 1. The Workflow Goal
**Objective:** Create an AI agent that drafts, updates, or rebuilds SOPs strictly using provided source materials while adopting the highly specific tone and tense required for technical QMS documents.
**Risk:** The agent might hallucinate equipment parameters, "clean up" historical revision logs and break traceability, or use a conversational tone instead of imperative commands.

## 2. Selected Semantic Primitives
To constrain the agent safely within this workflow, the following primitives are selected from `sp.md` and sequenced based on the intended workflow design:
* **Persona (Purpose & Scope)**
* **Closed Context**
* **Read Documents First**
* **Source of Truth Boundaries**
* **Zero Inference**
* **Mandatory Context Halt**
* **Don't Halt, Flag Gaps**
* **Proportionate Writing with Omissions**
* **Negative Constraints**
* **Material-Bound History Conservation**
* **Modal Context Gating** *(applied across workflow-defined phases)*
* **Tone**
* **Tense**



## These primitives serve as the behavioral foundation; additional workflow-specific requirements should be incorporated during instruction development.
