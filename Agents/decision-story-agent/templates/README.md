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
