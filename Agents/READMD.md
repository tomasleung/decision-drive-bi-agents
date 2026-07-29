# Agents README

## Decision-Driven BI Agent Platform

Version: 1.0

Status: Approved

Purpose:

Provide the navigation, catalog, and onboarding guide for the platform's agent ecosystem.

This README serves as the entry point into the agents folder and explains:

- What agents exist
- Why they exist
- How they work together
- How information moves through the platform
- Recommended agent read order
- How agents fit into the Decision-Driven BI lifecycle

---

# Purpose Of The Agents Folder

The agents folder contains the operational workforce of the Decision-Driven BI Agent Platform.

Agents exist to transform:

Business Requirements

into

Production-Ready Business Intelligence Assets

through governed handoffs and specialized responsibilities.

Agents are responsible for:

- Discovery
- Validation
- Design
- Modeling
- Specification
- Build Preparation

Each agent owns a specific part of the lifecycle.

---

# Agent Philosophy

Agents do not replace governance.

Agents do not replace ownership.

Agents do not replace business decisions.

Agents operate within:

- Platform Coach Standards
- Decision-First Principles
- RDLC Governance
- Platform Architecture
- Contracts
- Standards

The platform provides knowledge.

Agents provide reasoning.

AI provides execution.

---

# Agent Ecosystem Overview

The platform follows:

```text
Business Discovery
↓
Decision Validation
↓
Business Design
↓
Technical Design
↓
Semantic Design
↓
Semantic Build
↓
Report Build
↓
Business Action
```

Each phase is represented by a dedicated platform agent.

---

# Agent Catalog

The current platform defines six primary agents.

---

## Agent 01 — Decision Story Agent

Purpose:

Transform Business Requirements into approved decision design artifacts.

Consumes:

```text
INPUT_BRD
```

Produces:

```text
REPORT_STORY_MATRIX

REPORT_STORY
```

Answers:

```text
What decisions require support?

What business questions matter?

What signals matter?

What actions should occur?

What story should be communicated?
```

Lifecycle Ownership:

```text
Decision Validation

Business Design
```

---

## Agent 02 — Mockup Agent

Purpose:

Transform approved business design into user experience prototypes.

Consumes:

```text
REPORT_STORY
```

Produces:

```text
MOCKUP.md

MOCKUP.svg
```

Answers:

```text
What should users see?

How should the story be consumed?

What deserves attention?
```

Lifecycle Ownership:

```text
Business Design

Experience Design
```

---

## Agent 03 — TRD Agent

Purpose:

Transform approved business artifacts into a governed technical implementation contract.

Consumes:

```text
REPORT_STORY

MOCKUP
```

Produces:

```text
TRD
```

Answers:

```text
What data is required?

What systems provide data?

What technical objects are required?

How should the solution be implemented?
```

Lifecycle Ownership:

```text
Technical Design
```

---

## Agent 04 — Semantic Design Agent

Purpose:

Transform business and technical requirements into semantic architecture.

Consumes:

```text
REPORT_STORY

TRD
```

Produces:

```text
DATA_MODEL_MATRIX

SEMANTIC_MODEL_SPEC

MEASURE_CONTRACT
```

Answers:

```text
What facts exist?

What dimensions exist?

What measures exist?

How should semantic objects support decisions?
```

Lifecycle Ownership:

```text
Semantic Design
```

---

## Agent 05 — Semantic Build Agent

Purpose:

Transform semantic architecture into implementation-ready specifications.

Consumes:

```text
DATA_MODEL_MATRIX

SEMANTIC_MODEL_SPEC

MEASURE_CONTRACT
```

Produces:

```text
SEMANTIC_BUILD_SPEC

DAX_MEASURE_SPEC

TMDL_BUILD_SPEC

DEPLOYMENT_SPEC
```

Answers:

```text
How should the semantic model be built?

How should measures be implemented?

How should deployment occur?
```

Lifecycle Ownership:

```text
Semantic Build
```

---

## Agent 06 — Report Build Agent

Purpose:

Transform approved business and semantic assets into a completed BI solution.

Consumes:

```text
REPORT_STORY

MOCKUP

TRD

Fabric Semantic Model
```

Produces:

```text
REPORT_BUILD_SPEC

Completed BI Solution
```

Answers:

```text
What pages should exist?

What visuals should exist?

What interactions should exist?

How should users experience the solution?
```

Lifecycle Ownership:

```text
Report Build

Solution Delivery
```

---

# End-To-End Agent Flow

```text
INPUT_BRD
↓
Decision Story Agent
↓
REPORT_STORY_MATRIX
↓
REPORT_STORY
↓
Mockup Agent
↓
MOCKUP
↓
TRD Agent
↓
TRD
↓
Semantic Design Agent
↓
DATA_MODEL_MATRIX
↓
SEMANTIC_MODEL_SPEC
↓
MEASURE_CONTRACT
↓
Semantic Build Agent
↓
SEMANTIC_BUILD_SPEC
↓
Fabric Semantic Model
↓
Report Build Agent
↓
Production BI Solution
```

---

# Agent Handoff Model

The platform is built around governed handoffs.

Every agent:

```text
Consumes Approved Artifacts
↓
Performs Specialized Reasoning
↓
Produces Approved Artifacts
```

Agents should never:

```text
Re-discover Approved Business Knowledge
```

The contract layer exists to prevent:

```text
Business Rediscovery
```

throughout the lifecycle.

---

# Agent Design Principles

Every platform agent should define:

- Purpose
- Inputs
- Outputs
- Workflow
- Validation Rules
- Approval Rules
- Exit Criteria
- Handoff Contracts
- Examples
- Failure Modes

No agent should exist without a business question.

No agent should exist without a downstream consumer.

---

# Agent Governance Model

Every agent operates under:

```text
Platform Coach Standard
↓
Framework
↓
Architecture
↓
Repository Standard
↓
Skill Package Standard
↓
Skill Implementation Standard
↓
Agent Repository
↓
Runtime Execution
```

Governance always overrides execution.

---

# Agent Read Order

Before reviewing a specific repository:

Understand the platform first.

Recommended order:

```text
README.md
↓
framework/README.md
↓
framework/standards/README.md
↓
agents/README.md
```

Then choose an individual agent.

---

# Individual Agent Read Order

Example:

```text
agents/
└── decision-story-agent/
```

Read:

```text
PROJECT_INIT.md
↓
README.md
↓
AGENT_README.md
↓
SKILL_BLUEPRINT.md
↓
skill.md
```

Only after agent understanding is complete should execution begin.

---

# Agent Lifecycle Pattern

Every platform agent should follow:

```text
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
```

This pattern applies to:

- Human Work
- AI Work
- Agent Work
- Automation Work

---

# Agent Success Criteria

The agent ecosystem succeeds when:

Every agent:

- Answers a specific question
- Produces a specific artifact
- Supports a specific lifecycle phase
- Has a defined owner
- Has a defined contract
- Has a governed handoff

without requiring business rediscovery.

---

# Agent Ecosystem Success Statement

The agent ecosystem succeeds when Business Requirements can flow through a governed sequence of specialized agents that progressively transform:

```text
Business Intent
↓
Decision Design
↓
Business Design
↓
Technical Design
↓
Semantic Design
↓
Semantic Build
↓
Report Build
↓
Business Action
```

while preserving:

```text
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
```

traceability throughout the lifecycle.

---

# Next Location

To begin implementation, start with:

```text
agents/
└── decision-story-agent/
```

Read:

```text
PROJECT_INIT.md
```

first.