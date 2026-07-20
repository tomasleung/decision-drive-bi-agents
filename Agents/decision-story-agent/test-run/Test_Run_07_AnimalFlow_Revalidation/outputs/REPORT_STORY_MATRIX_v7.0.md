# REPORT_STORY_MATRIX_v7.0.md
## Animal Flow — Live Capacity Reporting
### Decision Story Matrix (v3 output)

---

# Document Metadata

Document Type: Decision Story Matrix

Version: 7.0

Capability: Animal Flow — Live Capacity Reporting

Purpose: Provide a compact, machine-friendly decision matrix to drive the Decision Story Contract (DSC) with developer-ready signal definitions, thresholds, and traceability.

Skill Variant: skill_v2.2.md

Resolved Templates:

- 01_REPORT_STORY_MATRIX_TEMPLATE_v3.0.md
- 02_REPORT_STORY_TEMPLATE_v3.0.md

Reference Files:

- REPORT_DESIGN_STANDARDS_v1.1.md
- DECISION_STORY_GUIDELINES_v1.0.md
- INPUT_BRD_AnimalFlow_LiveCapacity_v2.0.md

---

# Writer guidance (applied)

This artifact follows the v3 template guidance: each Story includes Purpose and Supporting Signals; every signal includes a Signal Definition and a Threshold Matrix; decision traceability is provided.

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

---

## Decision Owner

Animal Flow Team

---

## Decision Frequency

Multiple times daily

---

# STEP 02 — BUSINESS QUESTION MATRIX

| Business Question | Decision Category | Priority |
|---|---:|---|
| Which centres currently have available DOG capacity? | Placement | Critical |
| Which centres currently have available CAT capacity? | Placement | Critical |
| Which centres should be prioritized for intake? | Placement | Critical |
| Which centres should be avoided for intake? | Placement | High |
| Which centres have emergency closures? | Eligibility | High |
| Which centres have missing kennel assignments? | Data Trust | High |
| Which regions have the highest utilization? | Regional Monitoring | Medium |

---

# STEP 03 — SIGNAL MATRIX (DETAILED DEFINITIONS)

| Signal | Definition | Calculation | Unit | Source | Validation Rule | Example |
|---|---|---:|---|---|---|---|
| DOG_Open_Spaces | Number of open DOG-capable spaces available for intake | `COUNT(kennels) WHERE species='DOG' AND status='OPEN'` | spaces | Shelter system | Non-negative integer; last update <= 12h | 12 |
| CAT_Open_Spaces | Number of open CAT-capable spaces available for intake | `COUNT(kennels) WHERE species='CAT' AND status='OPEN'` | spaces | Shelter system | Non-negative integer; last update <= 12h | 8 |
| DOG_Utilization_Pct | Share of DOG capacity currently occupied | `DOG_Occupied / DOG_Total * 100` | percent | Shelter system | 0-200%; last update <= 2h | 84 |
| CAT_Utilization_Pct | Share of CAT capacity currently occupied | `CAT_Occupied / CAT_Total * 100` | percent | Shelter system | 0-200%; last update <= 2h | 72 |
| Emergency_Closure_Flag | Boolean indicator if centre has an active emergency closure | `exists(closure WHERE status='ACTIVE')` | boolean | Operations feed | boolean; update propagation <= 15m | true/false |
| Missing_Kennel_Assignments | Count of animals without assigned kennel records | `COUNT(animals WHERE kennel_id IS NULL)` | count | Intake system | integer; reconcile within 24h | 4 |
| Capacity_Confirmation_Age_Hours | Hours since last capacity confirmation by centre | `current_timestamp - last_confirmation_ts` | hours | Centre confirmation feed | numeric; must be present | 6 |

Repeat as needed for derived/regional signals.

---

# STEP 04 — THRESHOLD MATRICES (PER CRITICAL SIGNAL)

### DOG_Utilization_Pct — Threshold Matrix

| Threshold | Status | Action | Rationale |
|---:|---|---|---|
| <80% | Healthy | Candidate Centre | Normal operating headroom available |
| 80%–99% | Monitor | Review Before Routing | Nearing operational risk; verify other signals |
| >=100% | Full | Do Not Intake | No capacity; enforce exclusion |

### CAT_Utilization_Pct — Threshold Matrix

| Threshold | Status | Action | Rationale |
|---:|---|---|---|
| <80% | Healthy | Candidate Centre | Normal headroom |
| 80%–99% | Monitor | Review Before Routing | Verify before routing |
| >=100% | Full | Do Not Intake | Exclude centre |

### Missing_Kennel_Assignments — Threshold Matrix

| Threshold | Status | Action | Rationale |
|---:|---|---|---|
| 0 | Healthy | No Action | Data is complete |
| 1–3 | Warning | Review | Minor quality issues; manual check |
| >3 | Critical | Data Cleanup Required | High data risk; block automated routing |

### Capacity_Confirmation_Age_Hours — Threshold Matrix

| Threshold | Status | Action | Rationale |
|---:|---|---|---|
| <12 | Current | Use Normally | Fresh confirmation |
| 12–24 | Aging | Validate | Confirm with centre |
| >24 | Stale | Contact Centre | Do not trust for automated routing |

---

# STEP 05 — DECISION TRACEABILITY (REQUIRED)

| Signal | Business Question | Decision | Resulting Action |
|---|---|---|---|
| DOG_Open_Spaces, DOG_Utilization_Pct | Which centres can receive DOG intake? | Placement Eligibility | Route to Candidate Centres or Block if Full |
| CAT_Open_Spaces, CAT_Utilization_Pct | Which centres can receive CAT intake? | Placement Eligibility | Route to Candidate Centres or Block if Full |
| Emergency_Closure_Flag | Should the centre be excluded? | Exclusion Decision | Exclude Centre Immediately |
| Missing_Kennel_Assignments, Capacity_Confirmation_Age_Hours | Can the information be trusted? | Trust Decision | Escalate to Data Team, Block Routing for Critical Issues |

---

# STEP 06 — STORY SUMMARY (EXPANDED)

Each Story below includes Question → Output → Audience → Action → Supporting Signals.

## Story 0 — Provincial Snapshot

- Question: What is happening across the province today?
- Output: Provincial Capacity Snapshot
- Audience: Animal Flow, Leadership
- Action: Understand overall operating conditions and prioritise regions
- Supporting Signals: DOG_Utilization_Pct, CAT_Utilization_Pct, Regional_Open_Capacity

## Story 1 — Action Required

- Question: What requires immediate attention?
- Output: Action Required
- Audience: Animal Flow
- Action: Identify urgent risks and assign operational tasks
- Supporting Signals: Emergency_Closure_Flag, Missing_Kennel_Assignments, DOG_Utilization_Pct

## Story 2 — Intake Readiness

- Question: Which centres can safely receive incoming animals?
- Output: Intake Readiness
- Audience: Animal Flow
- Action: Route intake to Candidate Centres
- Supporting Signals: DOG_Open_Spaces, CAT_Open_Spaces, DOG_Utilization_Pct, Capacity_Confirmation_Age_Hours

## Story 3 — Placement Prioritization

- Question: Which centres should be prioritized for intake?
- Output: Placement Decision Board
- Audience: Animal Flow
- Action: Rank centres by readiness and logistical constraints
- Supporting Signals: DOG_Open_Spaces, CAT_Open_Spaces, Regional_Travel_Time, DOG_Utilization_Pct

## Story 4 — Capacity Analysis

- Question: Why can or cannot centres receive additional animals?
- Output: Capacity Analysis
- Audience: Animal Flow
- Action: Present root cause and suggest mitigations
- Supporting Signals: DOG_Utilization_Pct, CAT_Utilization_Pct, Emergency_Closure_Flag

## Story 5 — Data Trust

- Question: Can the information be trusted?
- Output: Data Trust Summary
- Audience: Animal Flow
- Action: Escalate or clean data before automated actions
- Supporting Signals: Missing_Kennel_Assignments, Capacity_Confirmation_Age_Hours

## Story 6 — Regional Health

- Question: Where is capacity pressure building?
- Output: Regional Health
- Audience: Animal Flow, Leadership
- Action: Monitor and reallocate resources
- Supporting Signals: Regional_DOG_Utilization_Pct, Regional_Open_Capacity

## Story 7 — Operational Briefing

- Question: What should we do next?
- Output: Operational Briefing
- Audience: Animal Flow, Operations
- Action: Execute recommended actions and assign responsibilities
- Supporting Signals: Actionable queue from previous stories

---

# STEP 07 — ACTION MATRIX

| Condition | Recommended Action | Responsible Role |
|---|---|---|
| DOG_Utilization_Pct >= 100% | Do Not Intake | Animal Flow Ops |
| 80% <= DOG_Utilization_Pct < 100% AND Missing_Kennel_Assignments <= 3 | Review Before Routing | Animal Flow Ops |
| Missing_Kennel_Assignments > 3 | Block Automated Routing; Assign Data Cleanup Task | Data Team |
| Capacity_Confirmation_Age_Hours > 24 | Contact Centre for Confirmation | Animal Flow Ops |

---

# STEP 08 — PAGE ARCHETYPE & LAYOUT

Primary Archetype: Operational Command Centre

Secondary Archetype: Capacity Intelligence

Layout (reading order): Summary → Action Required → Intake Readiness → Placement Board → Capacity Analysis → Data Trust → Regional Health → Operational Briefing

Markdown Wireframe (page-level):

- Summary KPIs (Province-wide) — KPI cards: DOG Utilization, CAT Utilization, Regional Pressure
- Action Required — Exception list with quick actions
- Intake Readiness — Table of candidate centres with status badges
- Placement Decision Board — Ranked table with filters
- Capacity Analysis — Per-centre drilldown cards
- Data Trust — Exception matrix and reconciliation tasks
- Regional Health — Heatmap + trend charts
- Operational Briefing — Task list and owner assignment

---

# STEP 09 — VISUAL RECOMMENDATIONS

| Section | Visual | Reason | Data Source | Interaction |
|---|---|---|---|---|
| Summary | KPI Cards | Provide quick situational awareness | DOG_Open_Spaces, DOG_Utilization_Pct | Click to drill into region |
| Action Required | Exception KPI Cards | Surface urgent items | Emergency_Closure_Flag, Missing_Kennel_Assignments | Link to tasking workflow |
| Intake Readiness | Status Cards | Quickly identify eligible centres | DOG_Open_Spaces, Capacity_Confirmation_Age_Hours | Open centre details |

---

# STEP 10 — VALIDATION CHECKLIST

- Primary Decision Defined — PASS
- Business Questions Defined — PASS
- Signals Defined (with calculations) — PASS
- Thresholds Defined (per critical signal) — PASS
- Decision Traceability Provided — PASS
- Story Summary Completed — PASS
- Page Archetype & Wireframe Provided — PASS
- Visual Recommendations Provided — PASS

Standards applied: REPORT_DESIGN_STANDARDS_v1.1, DECISION_STORY_GUIDELINES_v1.0

---

# APPROVAL

Decision Model ☐ Approved
Questions ☐ Approved
Signals ☐ Approved
Thresholds ☐ Approved
Actions ☐ Approved