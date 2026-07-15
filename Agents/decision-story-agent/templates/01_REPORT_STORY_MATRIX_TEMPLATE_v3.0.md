# REPORT_STORY_MATRIX_TEMPLATE_v3.0
## Decision Story Matrix — Prescriptive v3

---

# Metadata

Document Type: Decision Story Matrix

Version: 3.0

Capability: <Capability Name>

Purpose: Provide a compact, machine-friendly decision matrix to drive the Decision Story Contract (DSC).

Owner: <Business Owner>

Resolved Templates: 01_REPORT_STORY_MATRIX_TEMPLATE_v3.0.md

Reference Files: <list reference docs, e.g. INPUT_BRD_...>

---

# Writer guidance

Writer guidance: Produce a clear Decision Story Matrix. For each Story below, expand to include one-line Purpose and Supporting Signals. For every signal include a `Signal Definition` entry (name, calculation, unit, source) and ensure at least one corresponding threshold table exists. Keep language concise, use tables where possible, and ensure traceability from signals → questions → decisions → actions.

LLM note: output must include the exact section headings in this template and fill skeleton tables.

---

# STEP 01 — DECISION MODEL

## Primary Decision

<Primary decision statement>

---

## Secondary Decisions

- <Secondary decision 1>
- <Secondary decision 2>

---

## Decision Owner

<Team>

---

## Decision Frequency

<e.g. Multiple times daily>

---

# STEP 02 — BUSINESS QUESTION MATRIX

| Business Question | Decision Category | Priority |
|---|---|---|
| <Question 1> | <Category> | <Critical/High/Medium/Low> |

---

# STEP 03 — SIGNAL MATRIX (REQUIRED)

For each signal used in the matrix, provide a `Signal Definition` row using the table below. Include measurement, calculation, example value, and a validation rule.

| Signal | Definition | Calculation | Unit | Source | Validation Rule | Example |
|---|---|---:|---|---|---|---|
| <Signal name> | <Short definition> | <SQL / formula> | <unit> | <source system> | <validation check> | <example value> |

Repeat the table for each signal.

---

# STEP 04 — THRESHOLD MATRICES (REQUIRED PER SIGNAL)

For every critical signal include a Threshold Matrix with rationale.

### <Signal name> — Threshold Matrix

| Threshold | Status | Action | Rationale |
|---|---|---|---|
| <e.g. <80%> | Healthy | Candidate Centre | <1-line rationale> |

---

# STEP 05 — DECISION TRACEABILITY (REQUIRED)

Map signals to questions, decisions and actions to preserve traceability.

| Signal | Business Question | Decision | Resulting Action |
|---|---|---|---|
| <Signal name> | <Question text> | <Decision name> | <Action> |

---

# STEP 06 — STORY SUMMARY (REQUIRED)

Provide a compact set of stories (minimum required list). For each Story include a one-line Purpose and Supporting Signals.

- Summary / Provincial Snapshot — Purpose: <one-line>. Supporting Signals: <list>
- Action Required — Purpose: <one-line>. Supporting Signals: <list>
- Intake Readiness — Purpose: <one-line>. Supporting Signals: <list>
- Prioritization / Placement Board — Purpose: <one-line>. Supporting Signals: <list>
- Data Trust — Purpose: <one-line>. Supporting Signals: <list>
- Regional Pressure — Purpose: <one-line>. Supporting Signals: <list>
- Next Steps / Operational Briefing — Purpose: <one-line>. Supporting Signals: <list>

---

# STEP 07 — ACTION MATRIX (REQUIRED)

Provide condition→action mappings derived from threshold tables. Use machine-friendly table format.

| Condition | Recommended Action | Responsible Role |
|---|---|---|
| <Condition expression> | <Action> | <Role> |

---

# STEP 08 — PAGE ARCHETYPE & LAYOUT BLUEPRINT (REQUIRED)

Primary Archetype: <e.g. Operational Command Centre>

Secondary Archetype: <e.g. Capacity Intelligence>

Layout (reading order):

- Summary / Provincial Snapshot
- Action Required
- Intake Readiness
- Placement Decision Board
- Capacity Analysis
- Data Trust
- Regional Health
- Operational Briefing

Provide a small Markdown wireframe under this heading describing the main sections and recommended components.

---

# STEP 09 — VISUAL RECOMMENDATIONS (REQUIRED)

For each major Story/Section provide a short table: Visual | Reason | Data Source | Interaction

| Section | Visual | Reason | Data Source | Interaction |
|---|---|---|---|---|
| <Section> | <Visual type> | <Why> | <Signals> | <Interaction notes> |

---

# STEP 10 — VALIDATION CHECKLIST (REQUIRED)

Confirm the matrix includes the following (mark PASS/FAIL during validation):

- Primary Decision Defined — PASS/FAIL
- Business Questions Defined — PASS/FAIL
- Signals Defined (with calculations) — PASS/FAIL
- Thresholds Defined (per critical signal) — PASS/FAIL
- Decision Traceability Provided — PASS/FAIL
- Story Summary Completed — PASS/FAIL
- Page Archetype & Wireframe Provided — PASS/FAIL
- Visual Recommendations Provided — PASS/FAIL

---

# STANDARDS & REFERENCES

List standards applied and reference files (document IDs, versions).

---

# APPROVAL

Decision Model ☐ Approved
Questions ☐ Approved
Signals ☐ Approved
Thresholds ☐ Approved
Actions ☐ Approved
