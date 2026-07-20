# Governance Layer

## Purpose

The Governance layer defines how Decision Story outputs are evaluated, approved, and improved.

These artifacts provide a consistent framework for:

```text
Decision Story Agent

Decision Story Review Agent

Template Evolution Agent

Future Human Reviews

Future LLM Reviews
```

The Governance layer ensures that output quality is measured against defined standards rather than individual opinions.

---

# Governance Hierarchy

The governance process follows:

```text
Gold Output Specification

↓

Review Criteria

↓

Scoring Model

↓

Review Results

↓

Template Improvements
```

---

# Governance Artifacts

## 1. DECISION_STORY_GOLD_OUTPUT_SPEC_v1.0.md

Purpose:

```text
Defines what a successful Decision Story output must contain.
```

This document establishes the official definition of:

```text
What Good Looks Like
```

Examples:

```text
Minimum Story Count

Minimum Question Coverage

Signal Contract Requirements

Traceability Requirements

Visual Coverage Requirements
```

This is the governing standard for all future Decision Story outputs.

---

## 2. DECISION_STORY_REVIEW_CRITERIA_v1.0.md

Purpose:

```text
Defines what reviewers check.
```

The Review Criteria converts the Gold Output Specification into reviewable checkpoints.

Examples:

```text
Are 8 Stories Present?

Are Signal Contracts Complete?

Is Decision Traceability Present?

Are Visual Recommendations Complete?
```

This document defines:

```text
What To Review
```

---

## 3. DECISION_STORY_SCORING_MODEL_v1.0.md

Purpose:

```text
Defines how outputs are scored.
```

The Scoring Model assigns weights and promotion thresholds.

Examples:

```text
Question Coverage

Signal Design

Story Quality

Visual Recommendations

Traceability
```

This document defines:

```text
How To Score
```

---

# Relationship Between Governance Files

```text
DECISION_STORY_GOLD_OUTPUT_SPEC_v1.0

Defines:

"What Good Looks Like"

↓

DECISION_STORY_REVIEW_CRITERIA_v1.0

Defines:

"What To Check"

↓

DECISION_STORY_SCORING_MODEL_v1.0

Defines:

"How To Score"
```

---

# Relationship To Templates

Templates define:

```text
How Output Is Generated
```

Governance defines:

```text
How Output Is Evaluated
```

Example:

```text
Template

↓

Generated Output

↓

Review Criteria

↓

Scoring Model

↓

Promotion Decision
```

---

# Relationship To Example Artifacts

Example artifacts provide reference implementations.

Location:

```text
examples/

ANIMALFLOW_REPORT_STORY_MATRIX_GOLD_v1.0.md

ANIMALFLOW_REPORT_STORY_GOLD_v1.0.md
```

Purpose:

```text
Show What Good Looks Like
```

The Gold examples are the practical implementation of the Governance standards.

---

# Promotion Workflow

```text
BRD

↓

Decision Story Agent

↓

REPORT_STORY_MATRIX

↓

REPORT_STORY

↓

Review Agent

↓

Review Criteria

↓

Scoring Model

↓

Promotion Decision
```

---

# Template Evolution Workflow

```text
Generated Output

↓

Review Findings

↓

Root Cause Analysis

↓

Template Improvement

↓

Retest

↓

Promotion
```

---

# Guiding Principle

The Decision-Driven BI Framework does not evaluate outputs based on:

```text
Personal Preference

Writing Style

Model Choice
```

Outputs are evaluated based on:

```text
Decision Support

Business Coverage

Traceability

Actionability

Governance Compliance
```

---

# Success Statement

The Governance layer succeeds when:

```text
Every Review

Is Consistent

Every Score

Is Repeatable

Every Output

Can Be Evaluated Objectively

Every Template

Can Be Improved Using Evidence
```

rather than opinion.