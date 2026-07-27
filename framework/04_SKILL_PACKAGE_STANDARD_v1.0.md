# 04_SKILL_PACKAGE_STANDARD_v1.0

## Decision-Driven BI Agent Platform

Version: 1.0

Status: Approved

Maturity: Platform Foundation

Purpose:
Define the standard structure, responsibilities, governance model, and operating conventions for all skill packages within the Decision-Driven BI Agent Platform.

---

# PURPOSE

The Skill Package Standard ensures all platform agents:

- Follow a consistent skill structure
- Follow a consistent execution model
- Follow a consistent governance model
- Follow a consistent documentation model
- Follow a consistent AI operating model
- Remain portable across AI platforms

The standard exists to eliminate:

- Skill Drift
- Prompt Drift
- Documentation Drift
- Behavior Drift
- Repository Inconsistency

across the platform.

---

# CORE PHILOSOPHY

The platform does not treat a skill as:

Prompt
+
LLM

A platform skill consists of:

Framework
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
+
Runtime Instructions

The skill contains the knowledge.

The AI performs the reasoning.

---

# SKILL PACKAGE OBJECTIVE

Every skill package should allow:

Developers

AI Engineers

GitHub Copilot

Claude

ChatGPT

Gemini

Microsoft Fabric Agents

Future AI Platforms

to consistently understand:

- Agent Purpose
- Agent Responsibilities
- Execution Lifecycle
- Inputs
- Outputs
- Governance
- Validation
- Handoff Contracts

without direct support from the skill creator.

---

# SKILL PACKAGE DEFINITION

A Skill Package represents the complete knowledge and execution model required for a single agent.

The package must contain:

- Business Knowledge
- Execution Knowledge
- Governance Rules
- Templates
- Contracts
- Runtime Instructions

required for agent execution.

---

# STANDARD SKILL PACKAGE STRUCTURE

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

# SKILL PACKAGE LAYERS

Every skill package should be organized into:

Knowledge Layer

Execution Layer

Governance Layer

Runtime Layer

---

# KNOWLEDGE LAYER

Purpose:

Provide agent knowledge.

Components:

inputs/

standards/

guidelines/

templates/

contracts/

examples/

The Knowledge Layer teaches the agent:

What exists

What matters

What must be produced

---

# EXECUTION LAYER

Purpose:

Define how the agent operates.

Primary Artifact:

SKILL_BLUEPRINT.md

The Execution Layer defines:

- Lifecycle
- Discovery Flow
- Validation Flow
- Output Generation
- Approval Process

---

# GOVERNANCE LAYER

Purpose:

Control quality.

Primary Components:

standards/

governance/

contracts/

The Governance Layer defines:

- Rules
- Validation
- Approval Gates
- Promotion Criteria
- Traceability

---

# RUNTIME LAYER

Purpose:

Provide AI execution instructions.

Primary Artifact:

skill.md

The Runtime Layer defines:

What the AI should do during execution.

---

# ROOT FILE RESPONSIBILITIES

## README.md

Purpose:

Repository Navigation Guide

Answers:

- What is this repository?
- What problem does it solve?
- What folders exist?
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

- Why does this repository exist?
- What problem does it solve?
- Mission
- Goals
- Success Criteria
- Non-Goals

Audience:

- Architects
- AI Agents

---

## AGENT_README.md

Purpose:

Agent Repository Guide

Answers:

- Agent Purpose
- Responsibilities
- Inputs
- Outputs
- Dependencies
- Relationships

Audience:

- Developers
- Reviewers
- AI Agents

---

## SKILL_BLUEPRINT.md

Purpose:

Agent Operating Specification

Answers:

- How does the agent work?
- What lifecycle exists?
- What validations exist?
- What stop conditions exist?
- How does governance work?

Audience:

- AI Engineers
- Skill Authors
- Architects

---

## skill.md

Purpose:

Runtime Instructions

Answers:

- What should the AI do right now?
- What should it read?
- What should it generate?

Audience:

- Runtime AI Platforms

Examples:

- GitHub Copilot
- Claude
- ChatGPT
- Gemini
- Fabric Agents

---

## CHANGELOG.md

Purpose:

Track repository evolution.

Tracks:

- Version History
- Enhancements
- Breaking Changes
- Governance Changes

---

# FOLDER RESPONSIBILITIES

## inputs/

Purpose:

Input Contracts

Defines:

Required business information before execution begins.

Examples:

- BRD Templates
- Discovery Templates
- Business Contracts

---

## standards/

Purpose:

Governance Rules

Defines:

What good looks like.

Examples:

- Modeling Standards
- Design Standards
- Validation Standards
- Traceability Standards

Highest Priority Artifact Layer.

---

## guidelines/

Purpose:

Execution Guidance

Defines:

How standards should be applied.

Examples:

- Discovery Guidance
- Design Guidance
- Review Guidance

---

## templates/

Purpose:

Artifact Structure

Defines:

Required output structures.

Examples:

- REPORT_STORY Template
- TRD Template
- Semantic Model Template

---

## contracts/

Purpose:

Agent Handoffs

Defines:

Required information passed between agents.

Examples:

- DSC Contract
- Mockup Contract
- TRD Contract
- Semantic Contract

---

## governance/

Purpose:

Quality Governance

Defines:

- Approval Rules
- Promotion Rules
- Validation Rules
- Review Criteria

---

## examples/

Purpose:

Reference Implementations

Used For:

- Learning
- Validation
- Regression Testing

---

## outputs/

Purpose:

Generated Deliverables

Examples:

- REPORT_STORY
- MOCKUP
- TRD
- SEMANTIC_MODEL_SPEC

---

## test-run/

Purpose:

Execution Validation

Used For:

- Agent Testing
- Regression Testing
- Quality Verification

---

# REQUIRED READ ORDER

Before execution an AI agent should establish skill understanding.

Recommended Read Order:

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
standards/
↓
guidelines/
↓
templates/
↓
contracts/
↓
examples/
↓
SKILL_BLUEPRINT.md
↓
skill.md

Execution should not begin until understanding has been established.

---

# EXECUTION MODEL

All platform skills follow:

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

This lifecycle applies to all platform agents.

---

# SKILL GOVERNANCE HIERARCHY

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
Blueprint
↓
Runtime Instructions
↓
AI Reasoning

Rule:

Standards Always Win.

---

# BLUEPRINT RESPONSIBILITIES

The Blueprint defines:

- Agent Lifecycle
- Discovery Process
- Validation Process
- Output Process
- Governance Process
- Approval Process

The Blueprint should never contain:

- Prompt Instructions
- Runtime Commands

These belong in:

skill.md

---

# RUNTIME RESPONSIBILITIES

skill.md defines:

- Runtime Behavior
- Execution Instructions
- Artifact Resolution
- Output Generation

skill.md implements the Blueprint.

skill.md does not redefine the Blueprint.

---

# EXAMPLE RESPONSIBILITIES

Examples exist to:

- Demonstrate Expected Quality
- Demonstrate Artifact Structure
- Demonstrate Traceability
- Demonstrate Governance

Examples do not replace standards.

Examples are subordinate to standards.

---

# REQUIRED GOVERNANCE COMPONENTS

Every skill package must define:

Purpose

Mission

Inputs

Outputs

Dependencies

Validation Rules

Stop Conditions

Approval Gates

Success Criteria

Promotion Status

A skill missing these components is incomplete.

---

# REQUIRED TRACEABILITY

Platform traceability model:

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

Whenever applicable:

No orphan elements permitted.

---

# SKILL PORTABILITY REQUIREMENT

Every skill package should support:

- GitHub Copilot
- Claude
- ChatGPT
- Gemini
- Microsoft Fabric Skills
- Future AI Platforms

Skill knowledge should remain independent from any single LLM.

The skill package is the product.

The AI is the execution engine.

---

# SUCCESS CRITERIA

The standard succeeds when every skill package:

- Uses the same structure
- Uses the same lifecycle
- Uses the same governance model
- Uses the same validation process
- Uses the same traceability model

regardless of implementation platform.

---

# SUCCESS STATEMENT

The Skill Package Standard succeeds when a developer or AI agent can:

1. Open a skill repository

2. Understand the repository purpose

3. Understand the execution model

4. Understand governance

5. Execute the skill safely

6. Produce governed outputs

without requiring direct guidance from the skill author.

The result is:

Portable

Governed

Reusable

AI-Native

Enterprise-Ready

skill packages.

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

README.md (Platform Landing Page)