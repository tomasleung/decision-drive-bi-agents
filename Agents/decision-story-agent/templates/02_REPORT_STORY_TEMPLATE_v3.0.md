# REPORT_STORY_TEMPLATE_v3.0
## Decision Story Contract (DSC) — Prescriptive v3

---

# Metadata

Document Type: Decision Story Contract

Version: 3.0

Capability: <Capability Name>

Skill Variant: <skill file used>

Owner: <Business Owner>

Purpose: Convert the Decision Story Matrix into a full Decision Story Contract that is developer-ready and design-ready.

Resolved Templates: 02_REPORT_STORY_TEMPLATE_v3.0.md

Reference Files: <list reference docs>

---

# Writer guidance

Writer guidance: Expand the matrix into a comprehensive DSC. For each Story include: Question, Output, Audience, Action, Supporting Signals (with brief rationale). For each supporting signal include a Signal Definition row and Threshold Matrix. Include Decision Traceability and a short page-by-page wireframe. Add Visual Recommendations with short reasons and data sources. Finish with a Validation Checklist and Approval Gate.

LLM note: Keep prose concise; prefer tables and bullet lists. Provide explicit calculation examples for signals.

---

# SECTION 01 — DECISION MODEL (REQUIRED)

## Primary Decision

<Primary decision statement>

## Secondary Decisions

- <Secondary decision 1>

## Decision Owner

<Team>

## Decision Frequency

<e.g. Multiple times daily>

---

# SECTION 02 — BUSINESS QUESTION MATRIX (REQUIRED)

| Business Question | Decision Category | Priority |
|---|---|---|
| <Question 1> | <Category> | <Critical/High/Medium/Low> |

---

# SECTION 03 — BUSINESS LOGIC MODEL (REQUIRED)

Describe the business logic used to combine signals and determine placement eligibility. Provide pseudocode or a short formula where possible.

Example:

```
PlacementReadiness = DOG_Open_Spaces + CAT_Open_Spaces + (100 - DOG_Utilization) + (100 - CAT_Utilization) - EmergencyClosurePenalty
```

---

# SECTION 04 — SIGNAL DEFINITIONS (REQUIRED)

| Signal | Definition | Calculation | Unit | Source | Validation Rule | Example |
|---|---|---:|---|---|---|---|
| <Signal> | <Definition> | <SQL/formula> | <unit> | <source> | <validation> | <example> |

Repeat per signal.

---

# SECTION 05 — THRESHOLD MATRIX (REQUIRED PER SIGNAL)

| Signal | Threshold | Status | Action | Rationale |
|---|---|---|---|---|
| <Signal> | <value> | <status> | <action> | <rationale> |

---

# SECTION 06 — DECISION TRACEABILITY (REQUIRED)

| Signal | Business Question | Decision | Action |
|---|---|---|---|
| <Signal> | <Question> | <Decision> | <Action> |

---

# SECTION 07 — ACTION MATRIX (REQUIRED)

| Condition | Recommended Action | Responsible Role | Notes |
|---|---|---|---|
| <Condition> | <Action> | <Role> | <Notes> |

---

# SECTION 08 — NARRATIVE STORY (REQUIRED)

For each story produce an explicit block in this exact format. Repeat for Story 0..N.

## Story X — <Short title>

- Question: <Full question>
- Output: <Exact output label>
- Audience: <list>
- Action: <one-line recommended action>
- Supporting Signals: <comma-separated list>
- Rationale: <one-line rationale>

Example stories to include (minimum): Summary / Provincial Snapshot; Action Required; Intake Readiness; Placement Prioritization; Capacity Analysis; Data Trust; Regional Health; Operational Briefing.

---

# SECTION 09 — PAGE ARCHETYPE & LAYOUT BLUEPRINT (REQUIRED)

Describe the primary layout and provide a simple Markdown wireframe per page.

---

# SECTION 10 — VISUAL RECOMMENDATIONS (REQUIRED)

| Section | Visual | Reason | Data Source | Interaction |
|---|---|---|---|---|
| <Section> | <Visual> | <Why> | <Signals> | <Interaction> |

---

# SECTION 11 — IMPLEMENTATION NOTES (RECOMMENDED)

Include data latency expectations, aggregation windows, recommended indexing keys, sample SQL, and any dev notes.

---

# SECTION 12 — VALIDATION CHECKLIST & STANDARDS (REQUIRED)

- Primary Decision Defined — PASS/FAIL
- Business Questions Defined — PASS/FAIL
- Signals Defined (with calculations) — PASS/FAIL
- Thresholds Defined — PASS/FAIL
- Decision Traceability — PASS/FAIL
- Story Blocks Completed — PASS/FAIL
- Page Wireframe Provided — PASS/FAIL
- Visual Recommendations Provided — PASS/FAIL

Standards applied: <list>

---

# APPROVAL GATE

Decision Model ☐ Approved
Business Questions ☐ Approved
Business Logic ☐ Approved
Signals ☐ Approved
Thresholds ☐ Approved
Actions ☐ Approved
Story Narrative ☐ Approved
Page Archetype ☐ Approved
