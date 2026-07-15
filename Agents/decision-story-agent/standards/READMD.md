# Standards
## Decision Story Agent

---

# Purpose

This folder contains the governing standards used by the Decision Story Agent.

Standards define:

```text
What Good Looks Like

Required Design Rules

Required Validation Rules

Required Governance Rules
```

The standards ensure all Decision Story artifacts are:

```text
Consistent

Deterministic

Governed

Repeatable

Decision Driven
```

across all projects.

---

# Why Standards Exist

The Decision Story Agent transforms:

```text
Business Requirements

↓

Decision Design

↓

Story Design
```

Without standards, reports become:

```text
Visual Driven

Dashboard Driven

Technology Driven
```

instead of:

```text
Decision Driven

Question Driven

Action Driven
```

---

# Current Standards

## REPORT_DESIGN_STANDARDS_v1.0

Purpose:

```text
Provide the official Decision-Driven BI
report design methodology.
```

This standard defines:

```text
Decision Design

Business Question Design

Signal Design

Threshold Design

Action Design

Story Design

Page Archetypes

Layout Standards

Visual Standards

Decision Story Contract Standards
```

---

# Standards Coverage

## Decision Design

Defines:

```text
Decision Ownership

Decision Frequency

Primary Decisions

Secondary Decisions

Decision Success Criteria
```

Answers:

```text
What decision requires support?
```

---

## Business Question Design

Defines:

```text
Question Structure

Question Prioritization

Question Validation
```

Answers:

```text
What must users know
before making a decision?
```

---

## Signal Design

Defines:

```text
Signal Identification

Signal Qualification

Signal Alignment
```

Answers:

```text
What should users monitor?
```

---

## Threshold Design

Defines:

```text
Healthy States

Warning States

Critical States

Action Triggers
```

Answers:

```text
When should users react?
```

---

## Action Design

Defines:

```text
Business Actions

Recommended Actions

Governance Actions
```

Answers:

```text
What should users do next?
```

---

## Story Design

Defines:

```text
Narrative Flow

Story Structure

Decision Flow

Audience Alignment
```

Answers:

```text
What story should the report tell?
```

---

## Layout Standards

Defines:

```text
Information Hierarchy

Page Archetypes

Section Ordering

Reading Flow
```

Answers:

```text
How should users consume information?
```

---

## Visual Standards

Defines:

```text
Visual Selection

Visual Purpose

Visual Governance

Visual Consistency
```

Answers:

```text
How should information be presented?
```

---

# Usage

The Decision Story Agent must apply:

```text
REPORT_DESIGN_STANDARDS_v1.0
```

before generating:

```text
REPORT_STORY_MATRIX

REPORT_STORY
```

The standards must be applied before templates are populated.

---

# Relationship To Templates

Standards define:

```text
Behavior

Logic

Governance

Validation Rules
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

---

# Design Chain

All report design activities must follow:

```text
Decision

↓

Business Question

↓

Signal

↓

Threshold

↓

Action

↓

Story

↓

Layout

↓

Visual
```

This sequence may not be reversed.

Never start with:

```text
Visual

↓

Layout

↓

Story

↓

Decision
```

---

# Rule

The Standards folder is the:

```text
Source Of Truth
```

for Decision Story design.

Agent logic must never override standards.

Templates must never override standards.

Examples must never override standards.

When conflicts exist:

```text
Standards Win
```

---

# Validation

Before approving Decision Story outputs verify:

```text
□ Decisions Identified

□ Questions Identified

□ Signals Identified

□ Thresholds Identified

□ Actions Identified

□ Story Flow Validated

□ Visual Recommendations Validated

□ Decision Traceability Preserved
```

---

# Success Statement

The Standards folder succeeds when:

```text
Every Decision Story

follows the same rules,

uses the same methodology,

and preserves the same
decision-driven philosophy.
```

The result is:

```text
Consistent

Governed

Repeatable

Decision-Driven Report Design
```