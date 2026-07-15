# REPORT_STORY_MATRIX_v8.0.md
## Animal Flow — Live Capacity Reporting
### Decision Story Matrix

---

# Document Metadata

Document Type

Decision Story Matrix

Version

8.0

Capability

Animal Flow — Live Capacity Reporting

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

- INPUT_BRD_AnimalFlow_LiveCapacity_v2.0
- REPORT_DESIGN_STANDARDS_v1.1
- DECISION_STORY_GUIDELINES_v1.0

---

# Writer guidance

This artifact follows the v5 template guidance. All placeholders are filled. Signal definitions include business calculation references and validation rules. Threshold tables include business meaning. Visual recommendations include data source and interaction notes.

---

# STEP 01 — DECISION MODEL

## Primary Decision

Which centres currently have sufficient capacity to support incoming animals?

---

## Secondary Decisions

- Which centres should be prioritized for intake?
- Which centres should be excluded from intake?
- Which centres require operational or data-quality intervention?
- Which regions are experiencing capacity pressure?
- Which centres need a trusted confirmation before placement?

---

## Decision Owner

Animal Flow Team

---

## Decision Frequency

Multiple times daily

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

Capacity
+
Eligibility
+
Data Trust
=
Placement Readiness

---

## Key Discovery

A centre can appear available but still be unsuitable due to utilization, emergency closure, or data trust issues.

---

## Decision Success Criteria

Users must be able to answer:

```text
Which centres can safely receive incoming animals?
```

within:

```text
30 Seconds
```

---

# STEP 02 — BUSINESS QUESTION MATRIX

| Business Question | Decision Category | Priority |
|----------|----------|----------|
| Which centres currently have available DOG capacity? | Placement | Critical |
| Which centres currently have available CAT capacity? | Placement | Critical |
| Which centres should be prioritized for intake? | Placement | Critical |
| Which centres should be avoided for intake? | Placement | High |
| Which centres have emergency closures? | Eligibility | High |
| Which centres have missing kennel assignments? | Data Quality | High |
| Which regions are experiencing utilization pressure? | Regional Monitoring | Medium |

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

- DOG_Open_Spaces
- CAT_Open_Spaces
- DOG_Utilization_Pct
- CAT_Utilization_Pct

Supported Decision

```text
Which centres can safely receive incoming animals?
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
| DOG_Open_Spaces | Determine available DOG capacity | Count of open DOG-capable spaces ready for intake | count open DOG kennel spaces | spaces | Shelter system | Which centres currently have available DOG capacity? | Placement eligibility | Must be non-negative and updated within 12 hours | 12 |
| CAT_Open_Spaces | Determine available CAT capacity | Count of open CAT-capable spaces ready for intake | spaces | Shelter system | Which centres currently have available CAT capacity? | Placement eligibility | Must be non-negative and updated within 12 hours | 8 |
| DOG_Utilization_Pct | Measure DOG occupancy rate | DOG occupied / DOG total * 100 | percent | Shelter system | Which centres are approaching critical utilization? | Eligibility / prioritization | Must be between 0 and 200 and updated within 2 hours | 84 |
| CAT_Utilization_Pct | Measure CAT occupancy rate | CAT occupied / CAT total * 100 | percent | Shelter system | Which centres are approaching critical utilization? | Eligibility / prioritization | Must be between 0 and 200 and updated within 2 hours | 72 |
| Emergency_Closure_Flag | Identify active closures | Active emergency closure status exists | boolean | Operations feed | Should the centre be excluded from intake? | Exclusion decision | Must be boolean and refreshed within 15 minutes | true/false |
| Missing_Kennel_Assignments | Identify missing kennel records | Count of animals without assigned kennel | count | Intake system | Can the information be trusted? | Data trust | Must be integer and reconcile within 24 hours | 4 |
| Capacity_Confirmation_Age_Hours | Measure confirmation freshness | Hours since last confirmed capacity status | hours | Centre confirmation feed | Can the information be trusted? | Data trust | Must be present and updated with each confirmation | 6 |

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

## DOG_Utilization_Pct

| Threshold | Status | Action | Business Meaning |
|----------|----------|----------|----------|
| <80% | Healthy | Candidate Centre | Centre has available headroom for DOG intake |
| 80%–99% | Monitor | Review Before Routing | Centre is approaching utilization risk |
| >=100% | Full | Do Not Intake | Centre should be excluded for DOG intake |

Supported Decision

```text
Which centres are approaching critical utilization?
```

---

## CAT_Utilization_Pct

| Threshold | Status | Action | Business Meaning |
|----------|----------|----------|----------|
| <80% | Healthy | Candidate Centre | Centre has available headroom for CAT intake |
| 80%–99% | Monitor | Review Before Routing | Centre is approaching utilization risk |
| >=100% | Full | Do Not Intake | Centre should be excluded for CAT intake |

Supported Decision

```text
Which centres are approaching critical utilization?
```

---

## Missing_Kennel_Assignments

| Threshold | Status | Action | Business Meaning |
|----------|----------|----------|----------|
| 0 | Healthy | No Action | Data is complete and trusted |
| 1–3 | Warning | Review | Minor data quality issues require scrutiny |
| >3 | Critical | Data Cleanup Required | Data quality risk is too high for routing |

Supported Decision

```text
Can the information be trusted?
```

---

## Capacity_Confirmation_Age_Hours

| Threshold | Status | Action | Business Meaning |
|----------|----------|----------|----------|
| <12 | Current | Use Normally | Confirmation is fresh enough for routing |
| 12–24 | Aging | Validate | Information is aging and needs verification |
| >24 | Stale | Contact Centre | Data is stale and requires reconfirmation |

Supported Decision

```text
Can the information be trusted?
```

---

# STEP 06 — DECISION TRACEABILITY

| Business Question | Signal | Threshold | Action |
|----------|----------|----------|----------|
| Which centres currently have available DOG capacity? | DOG_Open_Spaces | <any> | Candidate Centre |
| Which centres currently have available CAT capacity? | CAT_Open_Spaces | <any> | Candidate Centre |
| Which centres should be excluded from intake? | Emergency_Closure_Flag | Active | Exclude Centre |
| Can the information be trusted? | Missing_Kennel_Assignments | >3 | Data Cleanup Required |
| Can the information be trusted? | Capacity_Confirmation_Age_Hours | >24 | Contact Centre |

---

# STEP 07 — ACTION MATRIX

| Condition | Recommended Action | Responsible Role |
|----------|----------|----------|
| Emergency_Closure_Flag = true | Exclude centre from intake | Animal Flow Ops |
| DOG_Utilization_Pct >= 100% | Do not intake DOGs | Animal Flow Ops |
| Missing_Kennel_Assignments > 3 | Block automated intake and assign data cleanup | Data Team |
| Capacity_Confirmation_Age_Hours > 24 | Contact centre to refresh confirmation | Animal Flow Ops |

---

# STEP 08 — STORY SUMMARY

## Story 0

Question

```text
What is happening across the province today?
```

Output

```text
Provincial Capacity Snapshot
```

Audience

```text
Animal Flow
Leadership
```

Action

```text
Understand overall operating conditions and prioritise regions
```

Supporting Signals

```text
DOG_Utilization_Pct, CAT_Utilization_Pct, Regional_Open_Capacity
```

Decision Supported

```text
Placement eligibility and regional monitoring
```

Purpose

```text
Provide situational awareness for province-wide capacity.
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
Operational Command Centre
```

---

## Secondary Archetype

```text
Capacity Intelligence
```

---

## Supporting Archetype

```text
Exception Management
```

---

# STEP 10 — LAYOUT BLUEPRINT

```text
Summary

↓

Action Required

↓

Intake Readiness

↓

Placement Decision Board

↓

Capacity Analysis

↓

Data Trust

↓

Regional Health

↓

Operational Briefing
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
| Summary | What is happening across the province today? | KPI Cards | Provide quick situational awareness | DOG_Open_Spaces, DOG_Utilization_Pct | Click to drill into region |
| Action Required | What requires immediate attention? | Exception KPI Cards | Surface urgent issues | Emergency_Closure_Flag, Missing_Kennel_Assignments | Link to task workflow |
| Intake Readiness | Which centres can safely receive intake? | Status Cards | Identify candidate centres quickly | DOG_Open_Spaces, Capacity_Confirmation_Age_Hours | Open centre details |

---

# STEP 12 — MARKDOWN WIREFRAME

```text
Summary

Action Required

Intake Readiness

Placement Decision Board

Capacity Analysis

Data Trust

Regional Health

Operational Briefing
```

---

## Wireframe Purpose

Provide approved reading order before mockup generation.

---

# STEP 13 — SUCCESS CRITERIA

✅ Understand The Situation

✅ Identify Risks

✅ Understand Constraints

✅ Trust The Information

✅ Make A Decision

✅ Take Action

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
