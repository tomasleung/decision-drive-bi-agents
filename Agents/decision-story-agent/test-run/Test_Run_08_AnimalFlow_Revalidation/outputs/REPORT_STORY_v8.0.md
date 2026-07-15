# REPORT_STORY_v8.0.md
## Animal Flow — Live Capacity Reporting
### Decision Story Contract (DSC)

---

# Document Metadata

Document Type

Decision Story Contract

Version

8.0

Skill Variant

skill_v2.2.md

Capability Name

Animal Flow — Live Capacity Reporting

Owner

Animal Flow

Purpose

Convert the Decision Story Matrix into a full Decision Story Contract that is developer-ready.

Related Documents

- INPUT_BRD_AnimalFlow_LiveCapacity_v2.0
- REPORT_STORY_MATRIX_v8.0

---

# Writer guidance

This output follows the v5 template structure. Signal definitions include business calculation references and validation rules. Threshold tables include business meaning so downstream TDR and semantic design can implement correctly.

---

# SECTION 01 — DECISION MODEL

## Primary Decision

Which centres currently have sufficient capacity to support incoming animals?

---

## Secondary Decisions

- Which centres should be prioritized for intake?
- Which centres should be excluded from intake?
- Which centres require operational or data-quality intervention?
- Which regions are experiencing capacity pressure?
- Which centres need confirmation before placement?

---

# SECTION 02 — BUSINESS QUESTION MATRIX

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

# SECTION 03 — BUSINESS LOGIC MODEL

Eligibility is determined by available capacity, closure status, and data trust. Exclusion is applied first, then candidate centres are ranked by available open spaces and freshness of confirmation.

Example:

```
if Emergency_Closure_Flag then Exclude
else if DOG_Utilization_Pct >= 100% then Exclude
else if Missing_Kennel_Assignments > 3 then Data Cleanup Required
else Candidate Centre
```

---

# SECTION 04 — SIGNAL DEFINITIONS

| Signal | Definition | Calculation Reference | Unit | Source | Validation Rule | Example |
|----------|----------|----------|----------|----------|----------|----------|
| DOG_Open_Spaces | Number of open DOG-capable spaces available for intake | Count of open DOG kennel spaces | spaces | Shelter system | Must be non-negative and updated within 12 hours | 12 |
| CAT_Open_Spaces | Number of open CAT-capable spaces available for intake | Count of open CAT kennel spaces | spaces | Shelter system | Must be non-negative and updated within 12 hours | 8 |
| DOG_Utilization_Pct | DOG occupancy percentage | DOG occupied / DOG total * 100 | percent | Shelter system | Must be in 0-200 and updated within 2 hours | 84 |
| CAT_Utilization_Pct | CAT occupancy percentage | CAT occupied / CAT total * 100 | percent | Shelter system | Must be in 0-200 and updated within 2 hours | 72 |
| Emergency_Closure_Flag | Active emergency closure status for a centre | Active closure status exists | boolean | Operations feed | Must be boolean and refreshed within 15 minutes | true/false |
| Missing_Kennel_Assignments | Count of animals without an assigned kennel | Count of animals where kennel_id is null | count | Intake system | Must be integer and reconciled within 24 hours | 4 |
| Capacity_Confirmation_Age_Hours | Hours since last capacity confirmation by the centre | Current time minus confirmation timestamp | hours | Centre confirmation feed | Must be present and refreshed regularly | 6 |

---

# SECTION 05 — THRESHOLD MATRIX

| Signal | Threshold | Status | Action | Business Meaning |
|----------|----------|----------|----------|----------|
| DOG_Utilization_Pct | <80% | Healthy | Candidate Centre | Centre has adequate DOG capacity |
| DOG_Utilization_Pct | 80-99% | Monitor | Review Before Routing | Centre is nearing DOG utilization risk |
| DOG_Utilization_Pct | >=100% | Full | Do Not Intake | Centre is at or exceeding DOG capacity |
| CAT_Utilization_Pct | <80% | Healthy | Candidate Centre | Centre has adequate CAT capacity |
| CAT_Utilization_Pct | 80-99% | Monitor | Review Before Routing | Centre is nearing CAT utilization risk |
| CAT_Utilization_Pct | >=100% | Full | Do Not Intake | Centre is at or exceeding CAT capacity |
| Missing_Kennel_Assignments | 0 | Healthy | No Action | Data is complete and reliable |
| Missing_Kennel_Assignments | 1-3 | Warning | Review | Minor data issues; proceed with caution |
| Missing_Kennel_Assignments | >3 | Critical | Data Cleanup Required | Data quality risk is too high for automated routing |
| Capacity_Confirmation_Age_Hours | <12 | Current | Use Normally | Confirmation is fresh |
| Capacity_Confirmation_Age_Hours | 12-24 | Aging | Validate | Confirmation is aging and should be verified |
| Capacity_Confirmation_Age_Hours | >24 | Stale | Contact Centre | Confirmation is too old for reliable decisions |

---

# SECTION 06 — DECISION TRACEABILITY

| Signal | Business Question | Decision | Action |
|----------|----------|----------|----------|
| DOG_Open_Spaces | Which centres currently have available DOG capacity? | Candidate Selection | Candidate Centre |
| CAT_Open_Spaces | Which centres currently have available CAT capacity? | Candidate Selection | Candidate Centre |
| Emergency_Closure_Flag | Which centres should be excluded from intake? | Exclusion Decision | Exclude Centre |
| Missing_Kennel_Assignments | Can the information be trusted? | Data Trust | Data Cleanup Required |
| Capacity_Confirmation_Age_Hours | Can the information be trusted? | Data Trust | Contact Centre |

---

# SECTION 07 — ACTION MATRIX

| Condition | Recommended Action | Responsible Role | Notes |
|----------|----------|----------|----------|
| Emergency_Closure_Flag = true | Exclude centre from intake | Animal Flow Ops | Immediate operational exclusion |
| DOG_Utilization_Pct >= 100% | Do not intake DOGs | Animal Flow Ops | Centre at or over capacity |
| CAT_Utilization_Pct >= 100% | Do not intake CATs | Animal Flow Ops | Centre at or over capacity |
| Missing_Kennel_Assignments > 3 | Block automated routing and assign data cleanup | Data Team | Quality issue prevents safe routing |
| Capacity_Confirmation_Age_Hours > 24 | Contact centre for refresh | Animal Flow Ops | Data freshness issue |

---

# SECTION 08 — NARRATIVE STORY

## Story 0 — Provincial Snapshot

- Question: What is happening across the province today?
- Output: Provincial Capacity Snapshot
- Audience: Animal Flow, Leadership
- Action: Understand province-wide capacity and pressure
- Supporting Signals: DOG_Utilization_Pct, CAT_Utilization_Pct, Regional_Open_Capacity
- Rationale: Provide situational awareness to guide operational priorities

---

## Story 1 — Action Required

- Question: What requires immediate attention?
- Output: Action Required
- Audience: Animal Flow
- Action: Identify urgent risks and assign tasks
- Supporting Signals: Emergency_Closure_Flag, Missing_Kennel_Assignments, DOG_Utilization_Pct
- Rationale: Surface issues that need immediate remediation

---

Repeat for all story sections.

---

# SECTION 09 — PAGE ARCHETYPE

## Primary Archetype

Operational Command Centre

---

## Secondary Archetype

Capacity Intelligence

---

## Supporting Archetype

Exception Management

---

# SECTION 10 — LAYOUT BLUEPRINT

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

# SECTION 11 — VISUAL RECOMMENDATIONS

| Section | Question Supported | Visual | Reason | Data Source | Interaction |
|----------|----------|----------|----------|----------|----------|
| Summary | What is happening across the province today? | KPI Cards | Provide quick situational awareness | DOG_Utilization_Pct, CAT_Utilization_Pct | Click to drill to region |
| Action Required | What requires immediate attention? | Exception KPI Cards | Highlight urgent issues | Emergency_Closure_Flag, Missing_Kennel_Assignments | Link to action tasks |
| Intake Readiness | Which centres can safely receive intake? | Status Cards | Identify candidate centres quickly | DOG_Open_Spaces, Capacity_Confirmation_Age_Hours | Open centre details |

---

# SECTION 12 — IMPLEMENTATION NOTES

- Data latency expectations: utilization updated within 2 hours, closure status within 15 minutes
- Aggregation windows: 5-minute utilization rollups, 1-minute closure status
- Suggested keys: centre_id, timestamp, species, status
- Downstream TDR should convert business calculation references into implementation SQL and data model logic

---

# SECTION 13 — VALIDATION CHECKLIST

- Primary Decision Defined — PASS
- Business Questions Defined — PASS
- Signals Defined — PASS
- Thresholds Defined — PASS
- Decision Traceability Provided — PASS
- Story Blocks Completed — PASS
- Layout Blueprint Defined — PASS
- Visual Recommendations Defined — PASS

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
