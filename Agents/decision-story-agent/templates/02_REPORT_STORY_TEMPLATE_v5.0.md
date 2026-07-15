# REPORT_STORY_TEMPLATE_v5.0
## Decision Story Contract (DSC)
### Decision-Driven BI Framework

---

# Document Metadata

Document Type

Decision Story Contract

Version

5.0

Capability

[Capability Name]

Skill Variant

[skill file used]

Owner

[Business Owner]

Purpose

Convert the Decision Story Matrix into a full, developer-ready Decision Story Contract.

Resolved Templates

- 02_REPORT_STORY_TEMPLATE_v5.0.md

Reference Files

- [INPUT_BRD_...]
- [REPORT_DESIGN_STANDARDS_...]
- [DECISION_STORY_GUIDELINES_...]
- [REPORT_STORY_MATRIX_...]

---

# Writer guidance

This template is a business-level handoff artifact. Fill every placeholder and preserve the exact section headings. Use business calculation references in signal definitions. Do not require exact production SQL here. The downstream TDR/Semantic agent will use this contract to implement measures and data flows.

Required output structure:

- full signal definition detail with calculation reference, validation rule, example
- threshold tables with business meaning
- traceability between question, signal, and action
- story blocks with audience, output, action, and supporting signals
- page archetype, layout blueprint, visuals, and implementation notes

---

# SECTION 01 — DECISION MODEL

## Primary Decision

[Primary Decision]

## Secondary Decisions

- [Secondary Decision 01]
- [Secondary Decision 02]
- [Secondary Decision 03]
- [Secondary Decision 04]
- [Secondary Decision 05]

---

# SECTION 02 — BUSINESS QUESTION MATRIX

| Business Question | Decision Category | Priority |
|----------|----------|----------|
| [Question] | [Category] | [Priority] |
| [Question] | [Category] | [Priority] |
| [Question] | [Category] | [Priority] |

---

# SECTION 03 — BUSINESS LOGIC MODEL

Describe the business logic used to combine signals and determine placement, eligibility, or escalation. Use a short formula or pseudocode where helpful.

Example:

```
If Emergency_Closure_Flag then Exclude
Else If DOG_Utilization_Pct >= 100% then Exclude
Else If Missing_Kennel_Assignments > 3 then Flag_Data_Cleanup_Required
Else Candidate Centre
```

---

# SECTION 04 — SIGNAL DEFINITIONS

| Signal | Definition | Calculation Reference | Unit | Source | Validation Rule | Example |
|----------|----------|----------|----------|----------|----------|----------|
| [Signal] | [Definition] | [Business formula or reference] | [Unit] | [Source] | [Validation rule] | [Example] |

---

# SECTION 05 — THRESHOLD MATRIX

| Signal | Threshold | Status | Action | Business Meaning |
|----------|----------|----------|----------|----------|
| [Signal] | [Threshold] | [Status] | [Action] | [Meaning] |
| [Signal] | [Threshold] | [Status] | [Action] | [Meaning] |

---

# SECTION 06 — DECISION TRACEABILITY

| Signal | Business Question | Decision | Action |
|----------|----------|----------|----------|
| [Signal] | [Question] | [Decision] | [Action] |

---

# SECTION 07 — ACTION MATRIX

| Condition | Recommended Action | Responsible Role | Notes |
|----------|----------|----------|----------|
| [Condition] | [Action] | [Role] | [Notes] |

---

# SECTION 08 — NARRATIVE STORY

## Story 0 — [Title]

- Question: [Business Question]
- Output: [Output Section]
- Audience: [Audience]
- Action: [Intended Action]
- Supporting Signals: [Signals]
- Rationale: [Why this story matters]

---

Repeat for each story section.

---

# SECTION 09 — PAGE ARCHETYPE

## Primary Archetype

[Primary Archetype]

---

## Secondary Archetype

[Secondary Archetype]

---

## Supporting Archetype

[Supporting Archetype]

---

# SECTION 10 — LAYOUT BLUEPRINT

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

# SECTION 11 — VISUAL RECOMMENDATIONS

| Section | Question Supported | Visual | Reason | Data Source | Interaction |
|----------|----------|----------|----------|----------|----------|
| [Section] | [Question] | [Visual] | [Reason] | [Signals] | [Interaction] |

---

# SECTION 12 — IMPLEMENTATION NOTES

Include data latency expectations, aggregation windows, sample SQL references, data sources, and developer handoff notes.

---

# SECTION 13 — VALIDATION CHECKLIST

- Primary Decision Defined — PASS/FAIL
- Business Questions Defined — PASS/FAIL
- Signals Defined — PASS/FAIL
- Thresholds Defined — PASS/FAIL
- Decision Traceability Provided — PASS/FAIL
- Story Blocks Completed — PASS/FAIL
- Layout Blueprint Defined — PASS/FAIL
- Visual Recommendations Defined — PASS/FAIL

---

# SECTION 14 — APPROVAL GATE

Decision Model

☐ Approved

Business Questions

☐ Approved

Signals

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
