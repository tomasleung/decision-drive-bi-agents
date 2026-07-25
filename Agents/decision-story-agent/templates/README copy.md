# Templates
## Decision Story Agent

---

# Purpose

This folder contains the official output templates used by the Decision Story Agent.

Templates define:

```text
Document Structure

Required Sections

Required Metadata

Review Requirements

Approval Requirements
```

Templates ensure generated artifacts remain:

```text
Consistent

Repeatable

Governed

Auditable

Reusable
```

across all Decision-Driven BI projects.

---

# Why Templates Exist

The Decision Story Agent transforms:

```text
Business Requirements

↓

Decision Design

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
```

Templates provide a predictable structure for both humans and AI agents.

---

# Current Templates

## 01_REPORT_STORY_MATRIX_TEMPLATE_v1.0.md

Generates:

```text
REPORT_STORY_MATRIX_vX.X.md
```

Purpose:

```text
Validate the Decision Framework
before creating the full
Decision Story Contract.
```

Used For:

```text
Decision Validation

Business Question Validation

Signal Validation

Threshold Validation

Action Validation

Story Validation
```

Answers:

```text
What decisions should the report support?

What questions must be answered?

What signals matter?

What actions should occur?
```

Role:

```text
Business Validation Artifact
```

---

## 02_REPORT_STORY_TEMPLATE_v1.0.md

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
Decision Modeling

Business Logic

Narrative Design

Story Design

Layout Design

Visual Recommendations

Business Journey Design
```

Answers:

```text
What story should the report tell?

How should users consume information?

What actions should the report support?
```

Role:

```text
Decision Design Contract
```

---

# Template Sequence

Templates must always be executed in the following order:

```text
REPORT_STORY_MATRIX

↓

REPORT_STORY
```

Never skip a template.

The second template depends upon validation completed in the first template.

---

# Template Relationships

```text
REPORT_STORY_MATRIX

Validates Decision Design

↓

REPORT_STORY

Defines Story Design
```

---

# Relationship To Standards

Standards define:

```text
Methodology

Rules

Governance

Validation Requirements
```

Templates define:

```text
Structure

Sections

Formatting

Output Layout
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

# Template Usage Rules

Templates must:

```text
Remain Approved

Remain Version Controlled

Remain Reusable

Remain Backward Traceable
```

Templates should not:

```text
Contain Business Logic

Contain Project-Specific Content

Contain Customer-Specific Decisions
```

Those are provided during execution.

---

# Agent Rules

Agents may:

```text
Populate Content

Populate Metadata

Populate Validation Sections

Populate Approval Sections
```

Agents may not:

```text
Remove Sections

Rename Sections

Reorder Sections

Skip Mandatory Sections

Modify Governance Sections
```

without template revision approval.

---

# Governance

Templates provide:

```text
Output Consistency

Deterministic Structure

Stakeholder Expectations

Review Consistency

Approval Consistency

Auditability
```

Every generated artifact must map back to an approved template.

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
```

---

# Folder Structure

```text
templates/

README.md

01_REPORT_STORY_MATRIX_TEMPLATE_v1.0.md

02_REPORT_STORY_TEMPLATE_v1.0.md
```

---

# Success Statement

The Templates folder succeeds when:

```text
Every Decision Story Artifact

uses the same structure,

supports the same review process,

and delivers the same governance experience
```

across all Decision-Driven BI projects.

The result is:

```text
Consistent

Governed

Predictable

Decision-Driven Documentation
```