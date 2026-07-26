# Contributing to the QMS Agent Governance Framework

Thank you for your interest in contributing! This framework relies on community expertise to build a robust, standardized vocabulary for AI governance in regulated environments.

To ensure the framework remains lean and effective, please adhere to the following guidelines when submitting new Pull Requests (PRs).

## Submitting New Semantic Primitives (`sp.md`)
We welcome new semantic primitives that define operational boundaries for AI agents. When proposing a new primitive, ensure it meets the following criteria:

* **It is an Anchor, Not a Prompt:** A primitive should be a high-density behavioral concept (e.g., `Zero Inference`), not a lengthy, wordy paragraph of system instructions. It relies on the LLM's latent understanding to expand it.
* **It is Workflow-Agnostic:** The primitive should be applicable across various QMS workflows (e.g., auditing, drafting, intake), not hyper-specific to one machine or single use-case.
* **It Defines a Boundary:** A valid primitive dictates what an agent *must do*, *must not do*, or *when it must stop*. 
* **Formatting:** Please match the existing structure in `sp.md`—a bolded title followed by (if necessary) an indented sub-bullet containing a concise, 1-2 sentence disambiguation.

## Submitting New Blueprints (`blueprints/`)
If you'd like to share how you compile primitives into functional instructions: 
* Keep is simple! These are frames for instructions, not instructions themselves.
* Remove any proprietary company information, specific product names, or sensitive data.
