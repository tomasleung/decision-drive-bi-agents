# REPORT_STORY_MATRIX_TEMPLATE_v5.0
## Decision Story Matrix
### Decision-Driven BI Framework

---

# Document Metadata

Document Type

Decision Story Matrix

Version

5.0

Capability

[Capability Name]

Purpose

Provide a fast-review decision framework before generating the full Decision Story Contract (DSC).

Audience

- Product Owner
- Business Owner
- Report Designer
- BI Developer

Approval Gate

This artifact must be approved before creating the full DSC.

Resolved Templates

- 01_REPORT_STORY_MATRIX_TEMPLATE_v5.0.md

Reference Files

- [INPUT_BRD_...]
- [REPORT_DESIGN_STANDARDS_...]
- [DECISION_STORY_GUIDELINES_...]

---

# Writer guidance

This template is a business-level artifact. Fill every placeholder. Ensure the output includes the exact section headings shown here. Use the `Signal Contract` section to describe the business logic of each signal, not production SQL. The TDR/Semantic Design agent will convert business calculations into implementation logic.

The matrix must include:

- explicit decision traceability from questions → signals → thresholds → actions
- signal definitions with calculation reference, validation rule, and example
- threshold tables with business meaning
- story summary blocks with one-line purpose and supporting signals
- visual recommendations with data source and interaction guidance

---

# STEP 01 — DECISION MODEL

## Primary Decision

[Primary Decision]

---

## Secondary Decisions

- [Secondary Decision 01]
- [Secondary Decision 02]
- [Secondary Decision 03]
- [Secondary Decision 04]
- [Secondary Decision 05]

---

## Decision Owner

[Decision Owner]

---

## Decision Frequency

[Decision Frequency]

Examples

```text
Real Time
Hourly
Daily
Weekly
Monthly
Quarterly
```

---

## Governing Business Rule

[Business Rule]

Example

```text
Capacity
+
Eligibility
+
Data Trust
=
Placement Readiness
```

---

## Key Discovery

[Key Discovery]

---

## Decision Success Criteria

Users must be able to answer:

```text
[Decision Outcome]
```

within:

```text
[Time Requirement]
```

Example:

```text
30 Seconds
```

---

# STEP 02 — BUSINESS QUESTION MATRIX

| Business Question | Decision Category | Priority |
|----------|----------|----------|
| [Question] | [Category] | [Priority] |
| [Question] | [Category] | [Priority] |
| [Question] | [Category] | [Priority] |
| [Question] | [Category] | [Priority] |

---

## Decision Categories

```text
Placement
Operations
Capacity
Risk
Monitoring
Regional Monitoring
Data Quality
Executive Oversight
Compliance
Finance
Customer
```

---

## Priority Levels

```text
Critical
High
Medium
Low
```

---

# STEP 03 — SIGNAL MATRIX

## Signal Group

Signals

- [Signal]
- [Signal]
- [Signal]
- [Signal]

Supported Decision

```text
[Decision]
```

---

## Signal Validation

Every Signal Must:

```text
Support A Question

Support A Decision

Be Measurable

Be Explainable

Be Actionable
```

---

# STEP 04 — SIGNAL CONTRACTS

| Signal | Business Purpose | Business Definition | Calculation Reference | Unit | Source | Question Supported | Decision Supported | Validation Rule | Example |
|----------|----------|----------|----------|----------|----------|----------|----------|----------|----------|
| [Signal] | [Purpose] | [Definition] | [Business formula or reference] | [Unit] | [Source] | [Question] | [Decision] | [Validation rule] | [Example] |

---

## Signal Contract Validation

Every Signal Contract must define:

```text
Business Purpose

Business Definition

Question Supported

Decision Supported

Validation Rule
```

---

# STEP 05 — THRESHOLD MATRIX

## Signal Name

| Threshold | Status | Action | Business Meaning |
|----------|----------|----------|----------|
| [Threshold] | [Status] | [Action] | [Meaning] |
| [Threshold] | [Status] | [Action] | [Meaning] |
| [Threshold] | [Status] | [Action] | [Meaning] |

Supported Decision

```text
[Decision]
```

---

## Threshold Validation

Every Threshold Must Define:

```text
Status

Action

Business Meaning
```

---

# STEP 06 — DECISION TRACEABILITY

| Business Question | Signal | Threshold | Action |
|----------|----------|----------|----------|
| [Question] | [Signal] | [Threshold] | [Action] |

---

## Traceability Goal

Every Business Question must trace to:

```text
Signal

↓

Threshold

↓

Action
```

---

# STEP 07 — ACTION MATRIX

| Condition | Recommended Action | Responsible Role |
|----------|----------|----------|
| [Condition] | [Action] | [Role] |

---

## Action Validation

Every Action Must Support:

```text
Human Decision

Business Outcome

Operational Response
```

---

# STEP 08 — STORY SUMMARY

## Story 0

Question

```text
[Business Question]
```

Output

```text
[Output Section]
```

Audience

```text
[Audience]
```

Action

```text
[Intended Action]
```

Supporting Signals

```text
[Signals]
```

Decision Supported

```text
[Decision]
```

Purpose

```text
[Business Purpose]
```

---

Repeat for all Story Sections

---

## Story Validation

Story Flow Must Follow:

```text
Context

↓

Attention Required

↓

Decision Support

↓

Explanation

↓

Trust

↓

Action
```

---

# STEP 09 — PAGE ARCHETYPE

## Primary Archetype

```text
[Primary Archetype]
```

---

## Secondary Archetype

```text
[Secondary Archetype]
```

---

## Supporting Archetype

```text
[Supporting Archetype]
```

---

## Approved Archetypes

```text
Operational Command Centre

Capacity Intelligence

Executive Monitoring

Exception Management

Regional Monitoring

Performance Monitoring

Data Quality Investigation
```

---

# STEP 10 — LAYOUT BLUEPRINT

```text
[Section 01]

↓

[Section 02]

↓

[Section 03]

↓

[Section 04]

↓

[Section 05]

↓

[Section 06]

↓

[Section 07]

↓

[Section 08]
```

---

## Layout Validation

Layout Must Support:

```text
Context

↓

Analysis

↓

Decision

↓

Action
```

---

# STEP 11 — VISUAL RECOMMENDATIONS

| Section | Question Supported | Visual | Reason | Data Source | Interaction |
|----------|----------|----------|----------|----------|----------|
| [Section] | [Question] | [Visual] | [Reason] | [Signals] | [Interaction] |

---

## Visual Validation

Every Visual Must Support:

```text
Question

Signal

Decision

Action
```

---

# STEP 12 — MARKDOWN WIREFRAME

```text
[Section 01]

[Section 02]

[Section 03]

[Section 04]

[Section 05]

[Section 06]

[Section 07]

[Section 08]
```

---

## Wireframe Purpose

Provide approved reading order before mockup generation.

---

# STEP 13 — SUCCESS CRITERIA

✅ [Success Criterion]

✅ [Success Criterion]

✅ [Success Criterion]

✅ [Success Criterion]

✅ [Success Criterion]

✅ [Success Criterion]

---

## Report Validation

Users should be able to:

```text
Understand The Situation

Identify Risks

Understand Constraints

Trust The Information

Make A Decision

Take Action
```

within the defined success criteria.

---

# STEP 14 — VALIDATION CHECKLIST

- Primary Decision Defined — PASS/FAIL
- Business Questions Defined — PASS/FAIL
- Signals Defined — PASS/FAIL
- Signal Contracts Defined — PASS/FAIL
- Thresholds Defined — PASS/FAIL
- Decision Traceability Provided — PASS/FAIL
- Story Summary Completed — PASS/FAIL
- Layout Blueprint Defined — PASS/FAIL
- Visual Recommendations Defined — PASS/FAIL

---

# APPROVAL CHECKPOINT

Decision Model

☐ Approved

Business Questions

☐ Approved

Signals

☐ Approved

Signal Contracts

☐ Approved

Thresholds

☐ Approved

Decision Traceability

☐ Approved

Actions

☐ Approved

Story Summary

☐ Approved

Layout Blueprint

☐ Approved

Visual Recommendations

☐ Approved

---

# MATRIX SUCCESS STATEMENT

A Decision Story Matrix succeeds when:

```text
Every Question
supports a Decision

Every Signal
supports a Question

Every Threshold
supports an Action

Every Action
supports a Decision

Every Story Section
supports User Action
```

and stakeholders agree the decision logic is complete before generating the Decision Story Contract.

---

## Next Step

```text
Generate:

REPORT_STORY_v5.0.md

(Decision Story Contract)
```
