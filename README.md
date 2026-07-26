# QMS Agent Governance Framework
**A Behavioral Specification for AI Agents in Regulated Environments**

In high-consequence regulated industries, errors, unverified assumptions, or data alterations can directly impact safety, compliance, and product integrity.

Large Language Models (LLMs) are probabilistic systems that can generate plausible but unsupported outputs, make assumptions from incomplete context, and prioritize conversational helpfulness in ways that conflict with controlled Quality Management System (QMS) environments. This open-source framework defines behavioral concepts, workflow patterns, and semantic guardrails intended to constrain general-purpose AI agents toward controlled, source-driven operation.

Rather than just focusing on the final output, this framework defines the behavioral boundaries of the agent: what evidence it is permitted to use, when it must halt operations, and what actions are prohibited.

> Core Philosophy: This framework assumes the AI agent serves as a workflow assistant, not a decision-maker. It is intended to constrain the agent to administrative and knowledge-support activities while preserving human accountability for quality decisions and controlled records.

This framework is not intended to define:
* Autonomous quality decisions
* Batch disposition
* Laboratory result interpretation
* Release authorization
* Replacement of Quality Unit responsibilities
* Validated AI system requirements

---

## The Core Problem: Context Limits and Fatigue
Some no-code AI agent builders impose character limits on system instructions—often around 8,000. Even when instruction limits are not explicitly imposed, longer instruction sets can reduce reliability as models must balance competing instructions within their available context. When building a QMS agent, the instruction length is a critical concern.

---

## Design Philosophy: Workflow-Centric Architecture
When building agents for regulated environments, the intention is not to design prompts around abstract "AI Personas" acting autonomously. AI should not independently make quality decisions unless specifically validated, controlled, and approved for that intended use. Instead, designs follow Human Workflows. The concepts and blueprints in this repository treat the AI agent as a collaborator that assists the user but is not responsible for quality decisions.

---

## How to Use This Framework

### 1. [Concepts (`concepts.md`)](./concepts.md)
This file contains the core operational guidelines used to govern agent behavior. They are structured across five domains:
* Identity & Scope
* Knowledge & Boundaries
* Reasoning & Logic
* Workflow Execution
* Documentation & Compliance
#### The concepts in this repository are intentionally abstract. They are designed to serve as building blocks that can be expanded into organization-specific agent instructions, workflows, and implementation patterns.


### 2. [Blueprints (`blueprints/`)](./blueprints/)
The example blueprints demonstrate how an instruction set could be framed using the concepts. Actual details and instruction generation would be made by the user and their choice of LLM.

---

## Disclaimer & Liability Notice
Not Validated Software | Not Regulatory Advice

This repository provides an experimental framework and conceptual architectural patterns for educational and developmental purposes only.
* No Warranty: The concepts and blueprints provided herein are offered "AS IS" without warranty of any kind, express or implied.
* Not Validated: This framework does not constitute validated software under requirements associated with 21 CFR Part 11, EU Annex 11, GAMP 5, or any other global regulatory standard.
* User Responsibility: The creators of this repository accept no responsibility for implementations, deployments, or outcomes resulting from the use of these concepts. It is the strict and sole responsibility of the implementing organization and its Quality Unit to independently verify, validate, and ensure that any AI system deployed in a regulated environment complies with all applicable internal procedures and international regulatory requirements.

---

## License
This framework is licensed under a [Creative Commons Attribution 4.0 International License](https://creativecommons.org/licenses/by/4.0/). You are free to share and adapt this material for any purpose, even commercially, provided you give appropriate credit to the original author. Attribution should reference this repository as the original source of the framework.
