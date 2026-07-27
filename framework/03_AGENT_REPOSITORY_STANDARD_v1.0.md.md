# AGENT_REPOSITORY_STANDARD_v1.0

## Decision-Driven BI Agent Platform

Version: 1.0

Status: Approved

Maturity: Platform Foundation

Purpose:
Define the standard structure, governance model, required artifacts, folder organization, and operating conventions for all agent repositories within the Decision-Driven BI Agent Platform.

---

# PURPOSE

The Agent Repository Standard ensures all current and future agents:

- Follow a consistent structure
- Follow a consistent governance model
- Follow a consistent read order
- Follow a consistent artifact lifecycle
- Can be understood by humans and AI
- Can operate across multiple LLM platforms
- Support long-term maintainability

The repository standard exists to eliminate:

- Repository Drift
- Documentation Drift
- Agent Drift
- Skill Drift
- Governance Drift

across the Decision-Driven BI Agent Platform.

---

# REPOSITORY PHILOSOPHY

An Agent Repository is not simply:

Prompt
+
LLM

An Agent Repository is:

Framework
+
Knowledge
+
Governance
+
Standards
+
Guidelines
+
Templates
+
Contracts
+
Examples
+
Agent Logic

The repository contains the knowledge.

The AI provides reasoning.

---

# REPOSITORY OBJECTIVES

Every repository should allow:

Developers

AI Engineers

GitHub Copilot

Claude

ChatGPT

Gemini

Microsoft Fabric Agents

Future AI Platforms

to understand:

- Why the agent exists
- What the agent does
- What it consumes
- What it produces
- How it operates
- How it is governed

without direct guidance from the repository creator.

---

# AGENT REPOSITORY DEFINITION

An Agent Repository represents:

A Single Agent

With:

- Defined Purpose
- Defined Responsibilities
- Defined Inputs
- Defined Outputs
- Defined Governance
- Defined Approval Gates
- Defined Handoff Contracts

within the larger Decision-Driven BI Agent Ecosystem.

---

# STANDARD REPOSITORY STRUCTURE

```text
agent-name/

├── inputs/
│
├── standards/
│
├── guidelines/
│
├── templates/
│
├── contracts/
│
├── governance/
│
├── examples/
│
├── outputs/
│
├── test-run/
│
├── README.md
│
├── PROJECT_INIT.md
│
├── AGENT_README.md
│
├── SKILL_BLUEPRINT.md
│
├── skill.md
│
└── CHANGELOG.md
```

---

# ROOT FILE RESPONSIBILITIES

## README.md

Purpose:

Repository Navigation Guide

Answers:

- What is this repository?
- What agent exists here?
- What folders exist?
- What files are important?
- What should be read first?

Audience:

- Developers
- AI Agents
- Contributors

---

## PROJECT_INIT.md

Purpose:

Repository Constitution

Answers:

- Why this repository exists
- What problem it solves
- Mission
- Scope
- Success Criteria
- Non-Goals

Audience:

- Architects
- AI Agents
- Repository Owners

---

## AGENT_README.md

Purpose:

Agent Repository Guide

Answers:

- Agent Mission
- Agent Position
- Inputs
- Outputs
- Dependencies
- Responsibilities
- Relationships

Audience:

- Developers
- AI Agents
- Reviewers

---

## SKILL_BLUEPRINT.md

Purpose:

Agent Operating Specification

Answers:

- How the agent works
- Discovery Flow
- Validation Flow
- Execution Lifecycle
- Governance Model
- Approval Model

Audience:

- Skill Authors
- AI Engineers
- Framework Architects

---

## skill.md

Purpose:

Runtime Instructions

Answers:

- What should the AI do?
- In what order?
- Using what artifacts?

Audience:

- Runtime AI Platforms

Examples:

- GitHub Copilot
- Claude
- ChatGPT
- Gemini

---

## CHANGELOG.md

Purpose:

Repository History

Tracks:

- Version Changes
- Improvements
- Breaking Changes
- Governance Updates

---

# FOLDER RESPONSIBILITIES

## inputs/

Purpose:

Input Contracts

Defines:

What information must exist before execution begins.

Examples:

- BRD Templates
- Input Contracts
- Input Examples

---

## standards/

Purpose:

Governance Rules

Defines:

What good looks like.

Examples:

- Design Standards
- Validation Standards
- Traceability Standards

Priority:

Highest

---

## guidelines/

Purpose:

Execution Guidance

Defines:

How standards should be applied.

Examples:

- Discovery Guidance
- Modeling Guidance
- Review Guidance

---

## templates/

Purpose:

Artifact Structures

Defines:

How outputs should be organized.

Examples:

- REPORT_STORY_TEMPLATE
- TRD_TEMPLATE
- SEMANTIC_TEMPLATE

---

## contracts/

Purpose:

Agent Handoff Contracts

Defines:

What downstream agents must receive.

Examples:

- DSC Contract
- Mockup Contract
- TRD Contract
- Semantic Contract

---

## governance/

Purpose:

Repository Governance

Defines:

- Approval Rules
- Promotion Rules
- Validation Rules
- Review Rules

---

## examples/

Purpose:

Reference Implementations

Used for:

- Training
- Quality Validation
- Regression Testing

---

## outputs/

Purpose:

Generated Artifacts

Contains:

Agent Deliverables

Examples:

- REPORT_STORY
- MOCKUP
- TRD

---

## test-run/

Purpose:

Repository Validation

Used for:

- End-to-End Testing
- Regression Testing
- Quality Verification

---

# PLATFORM READ ORDER

Before repository execution:

Read:

PROJECT_INIT.md
↓
FRAMEWORK_README
↓
ARCHITECTURE
↓
README.md
↓
AGENT_README.md
↓
Standards
↓
Guidelines
↓
Templates
↓
Contracts
↓
SKILL_BLUEPRINT.md
↓
skill.md

Execution should not begin until repository understanding is complete.

---

# GOVERNANCE HIERARCHY

When conflicts occur:

Standards
↓
Guidelines
↓
Templates
↓
Contracts
↓
Examples
↓
Agent Logic
↓
AI Reasoning

Rule:

Standards Always Win.

---

# ARTIFACT RESOLUTION MODEL

Do not hardcode versions.

Resolve artifacts dynamically.

Resolution Process:

Locate
↓
Purpose Validation
↓
Status Validation
↓
Compatibility Validation
↓
Version Selection
↓
Execution

---

# APPROVED ARTIFACT SELECTION

Preferred Selection Order:

Approved
↓
Production Ready
↓
Frozen
↓
Highest Compatible Version

Do not automatically select the highest version.

Compatibility must be validated.

---

# AGENT EXECUTION MODEL

Every repository follows:

Discover
↓
Validate
↓
Reason
↓
Generate
↓
Validate
↓
Promote

This lifecycle applies to all agents.

---

# REQUIRED GOVERNANCE COMPONENTS

Every repository must define:

Purpose

Mission

Inputs

Outputs

Dependencies

Validation Rules

Approval Gates

Success Criteria

Success Statement

Promotion Status

Repositories missing these components are considered incomplete.

---

# REQUIRED TRACEABILITY

The platform traceability model is:

Business Problem
↓
Decision
↓
Question
↓
Signal
↓
Threshold
↓
Action
↓
Story
↓
Visual
↓
Implementation

Agents should preserve traceability whenever applicable.

No orphan elements should exist.

---

# AGENT HANDOFF RULE

Every repository must declare:

Inputs Consumed

Outputs Produced

Downstream Consumers

Approval Requirements

Handoff Contracts

before execution logic is finalized.

---

# AI PORTABILITY REQUIREMENT

Repositories must remain compatible with:

- GitHub Copilot
- Claude
- ChatGPT
- Gemini
- Microsoft Fabric Skills
- Future AI Platforms

Repository knowledge should not depend on a specific LLM.

The repository is the product.

The AI is the execution engine.

---

# SUCCESS CRITERIA

The standard succeeds when:

Every agent repository:

- Looks consistent
- Reads consistently
- Executes consistently
- Scales consistently
- Preserves governance
- Preserves traceability

regardless of implementation technology.

---

# SUCCESS STATEMENT

The Agent Repository Standard succeeds when a developer or AI agent can:

1. Open a repository

2. Understand the repository purpose

3. Understand repository structure

4. Understand repository responsibilities

5. Execute the repository safely

6. Produce governed outputs

without requiring direct guidance from the repository creator.

The result is:

A portable,
governed,
AI-native,
platform-ready repository architecture.

---

# PROMOTION STATUS

Version:
1.0

Status:
APPROVED

Maturity:
Platform Standard

Promotion:
Approved For All Current And Future Agent Repositories

Next Artifact:

SKILL_PACKAGE_STANDARD_v1.0