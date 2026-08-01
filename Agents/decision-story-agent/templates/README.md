# Templates

## Decision Story Agent

Version: 1.1

Status: Approved

Purpose:

The Templates folder contains the official output templates used by the Decision Story Agent.

Templates define:

```text
Document Structure

Required Sections

Required Metadata

Validation Requirements

Approval Requirements

Promotion Requirements
```

Templates ensure generated artifacts remain:

```text
Consistent

Repeatable

Governed

Auditable

Traceable

Reusable
```

across all Decision-Driven BI projects.

---

# Purpose Of The Templates Layer

The Templates layer provides the approved structure used to convert validated decision thinking into governed artifacts.

Templates exist after:

```text
Thinking
↓
Governance
↓
Validation
↓
Design
```

and before:

```text
Implementation
```

Templates do not replace:

- Discovery
- Analysis
- Decision Design
- Business Reasoning

Templates provide structure for approved thinking.

---

# Why Templates Exist

The Decision Story Agent transforms:

```text
Business Requirements
↓
Decision Discovery
↓
Question Discovery
↓
Signal Discovery
↓
Action Discovery
↓
Story Design
↓
Decision Story Artifacts
```

Without templates:

```text
Outputs become inconsistent

Reviews become subjective

Governance becomes difficult

Traceability becomes unreliable

Quality becomes inconsistent
```

Templates provide a predictable structure for:

- Humans
- AI Agents
- Reviewers
- Governance Teams
- Future Platform Extensions

---

# Decision-First Alignment

The Decision Story Agent operates within the Decision-Driven BI Framework.

Framework Rule:

```text
No Decision
↓
No Artifact
```

Templates exist to document:

```text
Decisions

Questions

Signals

Thresholds

Actions

Stories
```

Templates should never encourage:

```text
Report First Thinking

Dashboard First Thinking

Visual First Thinking
```

Every artifact should begin with a decision.

---

# Current Templates

---

## REPORT_STORY_MATRIX_TEMPLATE_v7.0

Generates:

```text
REPORT_STORY_MATRIX_vX.X.md
```

Purpose:

```text
Validate Decision Thinking

before creation of the
Decision Story Contract.
```

Used For:

```text
Decision Validation

Business Question Validation

Signal Validation

Threshold Validation

Action Validation

Traceability Validation

Story Validation
```

Answers:

```text
What decisions should be supported?

What questions must be answered?

What signals matter?

What actions should occur?

Are we ready to proceed?
```

Role:

```text
Decision Validation Contract
```

---

## REPORT_STORY_TEMPLATE_v7.0

Generates:

```text
REPORT_STORY_vX.X.md
```

Purpose:

```text
Create the official
Decision Story Contract (DSC).
```

Used For:

```text
Business Design

Decision Modeling

Business Logic Design

Story Design

Narrative Design

Layout Design

Visual Recommendations

Implementation Readiness
```

Answers:

```text
What story should the solution tell?

How should users consume information?

What actions should occur?

What should downstream agents build?
```

Role:

```text
Decision Story Contract
```

---

# Template Execution Sequence

Templates must always be executed in the following order:

```text
REPORT_STORY_MATRIX
↓
REPORT_STORY
```

Never skip a template.

The Decision Story Contract depends upon validation completed within the Decision Story Matrix.

---

# Template Lifecycle

Templates participate in the platform lifecycle.

```text
Standards
↓
Guidelines
↓
Templates
↓
Contracts
↓
Generated Artifacts
```

Responsibilities:

```text
Standards
=
Rules

Guidelines
=
Recommended Practices

Templates
=
Structure

Contracts
=
Governed Handoffs

Artifacts
=
Generated Outputs
```

---

# Template Relationships

```text
REPORT_STORY_MATRIX

Validates Decision Design

↓

REPORT_STORY

Defines Business Design

↓

DSC Contract

Supports Downstream Agents
```

Each template builds upon previous validation work.

---

# Relationship To Standards

Standards define:

```text
Methodology

Rules

Governance

Validation Requirements

Quality Expectations
```

Templates define:

```text
Structure

Sections

Formatting

Output Layout

Documentation Patterns
```

Relationship:

```text
Standards
↓
Templates
↓
Artifacts
```

Standards tell us:

```text
What good looks like
```

Templates tell us:

```text
How to document it
```

---

# Relationship To Contracts

Templates create artifacts.

Contracts govern artifacts.

Relationship:

```text
Templates
↓
Artifacts
↓
Contracts
↓
Downstream Consumption
```

Example:

```text
REPORT_STORY_TEMPLATE
↓
REPORT_STORY
↓
DECISION_STORY_HANDOFF_CONTRACT
↓
Mockup Agent
```

---

# Template Traceability Rule

All generated artifacts should preserve:

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

Templates must support this traceability chain.

Templates should never introduce orphan elements.

Every section within a template should contribute to traceability.

---

# Template Usage Rules

Templates must:

```text
Remain Approved

Remain Version Controlled

Remain Reusable

Remain Traceable

Remain Governed

Remain Backward Compatible
```

Templates should not:

```text
Contain Project-Specific Logic

Contain Customer-Specific Decisions

Contain Temporary Workarounds

Contain Business Conclusions
```

Those are supplied during execution.

---

# Agent Rules

Agents may:

```text
Populate Content

Populate Metadata

Populate Validation Sections

Populate Approval Sections

Populate Traceability Sections
```

Agents may not:

```text
Remove Sections

Rename Sections

Reorder Sections

Skip Mandatory Sections

Modify Governance Sections

Modify Approval Sections
```

without approved template revision.

---

# Human Authority Principle

Templates support governance.

Templates do not provide governance authority.

AI may:

```text
Generate Content

Populate Sections

Recommend Improvements

Perform Validation
```

AI may not:

```text
Approve Governance

Approve Promotion

Approve Decisions

Approve Business Outcomes
```

Human approval remains mandatory.

---

# Governance

Templates provide:

```text
Output Consistency

Deterministic Structure

Stakeholder Expectations

Review Consistency

Approval Consistency

Promotion Consistency

Auditability

Traceability
```

Every generated artifact should map back to an approved template.

---

# Validation

Before approving a generated artifact verify:

```text
□ Correct Template Used

□ Metadata Complete

□ Required Sections Present

□ Validation Sections Completed

□ Approval Sections Present

□ Traceability Preserved

□ Governance Sections Complete

□ Promotion Requirements Satisfied
```

---

# Template Evolution Rules

Templates may evolve.

Template evolution should follow:

```text
Current State
↓
Gap Analysis
↓
Preservation Analysis
↓
Regression Analysis
↓
Refactor
↓
Validation Review
↓
Approval
↓
Promotion
```

Refactoring should preserve:

```text
Governance

Traceability

Validation Logic

Approval Logic

Promotion Logic
```

Valid existing capabilities should never be removed unintentionally.

---

# Folder Structure

```text
templates/

README.md

REPORT_STORY_MATRIX_TEMPLATE_v7.0.md

REPORT_STORY_TEMPLATE_v7.0.md
```

---

# Success Statement

The Templates folder succeeds when:

```text
Every Decision Story Artifact

uses the same structure,

supports the same review process,

supports the same validation process,

supports the same promotion process,

and delivers the same governance experience
```

across all Decision-Driven BI projects.

The result is:

```text
Consistent

Governed

Traceable

Repeatable

Auditable

Decision-Driven Documentation
```

throughout the Decision-Driven BI Agent Platform.