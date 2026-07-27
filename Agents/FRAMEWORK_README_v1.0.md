# Decision-Driven BI Framework

Version: 1.0

Status: Approved

Framework Status: Production Ready

---

# Purpose

The Decision-Driven BI Framework provides a governed, repeatable methodology for transforming business requirements into decision-focused business intelligence solutions.

The framework ensures solutions begin with:

- Business Problems
- Business Decisions
- Business Questions
- Business Actions

before considering:

- Reports
- Dashboards
- Pages
- Visuals
- Technology

The goal is to create:

**Decision Products**

rather than:

**Reporting Products**

---

# Why Decision-Driven BI?

Traditional BI often follows:

```text
Data
↓
Chart
↓
Dashboard
↓
User Figures It Out
```

Decision-Driven BI follows:

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
```

The purpose of reporting is:

**Business Action**

not information consumption.

---

# Framework Mission

The framework exists to answer:

- What business problem requires attention?
- What decisions should be supported?
- What information is required?
- What evidence should support decisions?
- What actions should occur?
- What story should be communicated?

before asking:

```text
What should the report look like?
```

---

# Core Philosophy

The framework provides:

- Governance
- Structure
- Coverage
- Traceability
- Validation

Templates provide:

- Guardrails
- Structure
- Required Deliverables
- Traceability Requirements

The LLM provides:

- Discovery
- Reasoning
- Inference
- Question Generation
- Signal Design
- Story Design
- Business Insight

The framework constrains:

- Coverage
- Governance
- Structure
- Traceability

The framework does not constrain:

- Discovery
- Analysis
- Reasoning
- Narrative Creation

---

# Framework Architecture

The framework follows a governed lifecycle:

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

The complete architecture is documented in:

```text
Decision-Driven BI Architecture v3.0
```

This document serves as the authoritative framework constitution.

---

# Framework Layers

## Layer 1 — Inputs

Purpose:

Provide the business contract.

Answers:

```text
What information is required?
```

Artifacts:

- BRD Templates
- Business Inputs
- Discovery Contracts

---

## Layer 2 — Standards

Purpose:

Define quality expectations.

Answers:

```text
What good looks like?
```

Artifacts:

- Design Standards
- Validation Standards
- Governance Standards

---

## Layer 3 — Guidelines

Purpose:

Define execution methodology.

Answers:

```text
How should standards be applied?
```

Artifacts:

- Discovery Methodology
- Design Guidance
- Validation Guidance

---

## Layer 4 — Templates

Purpose:

Define required deliverables.

Answers:

```text
What should be produced?
```

Artifacts:

- REPORT_STORY_MATRIX Templates
- REPORT_STORY Templates

---

## Layer 5 — Agents

Purpose:

Execute framework methodology.

Answers:

```text
How should the framework operate?
```

Artifacts:

- Decision Story Agent
- Mockup Agent
- TRD Agent
- Semantic Design Agent
- Semantic Build Agent
- Report Build Agent

---

## Layer 6 — Governance

Purpose:

Evaluate outputs.

Answers:

```text
How are outputs approved?
```

Artifacts:

- Approval Gates
- Acceptance Criteria
- Validation Criteria
- Promotion Criteria

---

# Agent Ecosystem

The framework currently contains the following agents:

## Agent 01 — Decision Story Agent

Purpose:

Convert business requirements into:

- REPORT_STORY_MATRIX
- REPORT_STORY (DSC)

Answers:

```text
What decisions should the report support?

What story should the report tell?
```

---

## Agent 02 — Mockup Agent

Purpose:

Convert approved business designs into visual prototypes.

Answers:

```text
What should users see?

How should users experience information?
```

---

## Agent 03 — TRD Agent

Purpose:

Convert business designs into technical implementation contracts.

Answers:

```text
How should the solution be implemented?
```

---

## Agent 04 — Semantic Design Agent

Purpose:

Convert business and technical requirements into semantic architecture.

Answers:

```text
What semantic model should exist?
```

---

## Agent 05 — Semantic Build Agent

Purpose:

Convert semantic designs into implementation specifications.

Answers:

```text
How should the semantic model be built?
```

---

## Agent 06 — Report Build Agent

Purpose:

Convert approved business and semantic designs into a completed BI solution.

Answers:

```text
How should the approved solution be built?
```

---

# Framework Governance Model

Framework governance follows:

```text
Standards
↓
Guidelines
↓
Templates
↓
Examples
↓
Agent Logic
```

Rule:

```text
Standards Win
```

Principles:

- Standards Define Rules
- Guidelines Direct Execution
- Templates Define Structure
- Examples Demonstrate Usage
- Agents Execute Framework Logic

---

# Framework Read Order

Before execution all agents should review:

```text
1. Framework README

2. Inputs README

3. Standards README

4. Guidelines README

5. Templates README
```

Only after framework understanding has been established should artifact execution begin.

---

# Artifact Resolution Philosophy

The framework supports dynamic artifact resolution.

Do not rely on hardcoded versions.

Preferred selection order:

```text
Approved
↓
Production Ready
↓
Frozen
↓
Highest Approved Version
```

Artifacts should be validated for:

- Purpose
- Status
- Compatibility
- Version

before use.

---

# Framework Execution Model

All framework agents follow:

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

This execution model applies to current and future agents.

---

# Matrix vs DSC

## REPORT_STORY_MATRIX

Purpose:

Decision Validation Contract

Answers:

```text
What?
```

Validates:

- Decisions
- Questions
- Signals
- Thresholds
- Actions
- Risks
- Stories
- Traceability

The Matrix exists to validate decision thinking before business design begins.

---

## REPORT_STORY (DSC)

Purpose:

Decision Story Contract

Answers:

```text
Why?

How?

Success Criteria?
```

Defines:

- Decision Logic
- Business Logic
- Narratives
- Visual Strategy
- Semantic Expectations
- Implementation Expectations

The DSC exists to eliminate business rediscovery during implementation.

---

# Promotion Workflow

```text
INPUT_BRD Approved
↓
REPORT_STORY_MATRIX Approved
↓
REPORT_STORY Approved
↓
Mockup Approved
↓
TRD Approved
↓
Semantic Design Approved
↓
Semantic Build Approved
↓
Report Build Approved
↓
Production Solution
```

---

# Traceability Standard

All framework activities must preserve:

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
```

traceability.

No orphan elements are permitted.

---

# Where To Start

## New Developers

Read:

```text
Framework README
↓
Decision-Driven BI Architecture v3.0
```

---

## Decision Story Work

Start in:

```text
decision-story-agent/
```

Read:

```text
README.md
↓
inputs/
↓
standards/
↓
guidelines/
↓
templates/
```

---

# Framework Success Statement

The Decision-Driven BI Framework succeeds when business requirements are transformed into governed decision-focused artifacts that support:

- Better Decisions
- Better Questions
- Better Signals
- Better Stories
- Better Outcomes

while remaining:

- Consistent
- Governed
- Traceable
- Repeatable
- Action-Oriented
- AI-Ready
- Decision-Driven

across all future implementations.

The result is:

**Decision Products**

not

**Reporting Products**.