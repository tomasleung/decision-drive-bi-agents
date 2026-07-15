# REPORT_STORY_v7.0.md
## Animal Flow — Live Capacity Reporting
### Decision Story Contract (DSC) — v3 output

---

# Document Metadata

Document Type: Decision Story Contract

Version: 7.0

Skill Variant: skill_v2.2.md

Capability Name: Animal Flow — Live Capacity Reporting

Owner: Animal Flow

Purpose: Convert the Decision Story Matrix (v3) into a full Decision Story Contract that is developer- and design-ready.

Related Documents:

- INPUT_BRD_AnimalFlow_LiveCapacity_v2.0
- REPORT_STORY_MATRIX_v7.0

---

# SECTION 01 — DECISION MODEL

## Primary Decision

Which centres currently have sufficient capacity to support incoming animals?

## Secondary Decisions

- Which centres should be prioritized for intake?
- Which centres should be excluded from intake?
- Which centres require operational or data-quality intervention?
- Which regions are experiencing capacity pressure?

---

# SECTION 02 — BUSINESS QUESTION MATRIX

- Which centres currently have available DOG capacity?
- Which centres currently have available CAT capacity?
- Which centres are approaching critical utilization?
- Which centres have emergency closures?
- Which centres have stale or missing capacity confirmations?
- Which centres have missing kennel assignments?
- Which regions have the highest utilization pressure?

---

# SECTION 03 — BUSINESS LOGIC MODEL

Capacity availability is determined by combining open spaces and utilization; final placement decisions apply exclusion rules (emergency closure, critical utilization, critical data issues) before routing.

Example pseudocode:

```
if Emergency_Closure_Flag then Exclude
else if DOG_Utilization_Pct >= 100% then Exclude
else if Missing_Kennel_Assignments > 3 then Flag_Data_Cleanup_and_Block
else Consider Candidate Centres ordered by Open_Spaces and travel_time
```

---

# SECTION 04 — SIGNAL MATRIX

(See REPORT_STORY_MATRIX_v7.0 for full signal definitions and calculations.)

---

# SECTION 05 — THRESHOLD MATRIX

- DOG Utilization %: <80% Candidate; 80–99% Monitor; >=100% Exclude
- CAT Utilization %: <80% Candidate; 80–99% Monitor; >=100% Exclude
- Missing Kennel Assignments: 0 Healthy; 1–3 Warning; >3 Critical
- Capacity Confirmation Age: <12h Current; 12–24h Aging; >24h Stale

---

# SECTION 06 — ACTION MATRIX

- Route intake to Candidate Centres
- Review Monitor band before routing
- Exclude centres with emergency closure or critical utilization
- Escalate stale confirmations to operations
- Trigger data cleanup for critical missing assignments

---

# SECTION 07 — NARRATIVE STORY (EXPANDED)

Use the Story blocks below directly in design and mockups. Each Story contains Question → Output → Audience → Action → Supporting Signals.

## Story 0 — Provincial Snapshot

- Question: What is happening across the province today?
- Output: Provincial Capacity Snapshot
- Audience: Animal Flow, Leadership
- Action: Understand operating conditions and prioritise resources
- Supporting Signals: DOG_Utilization_Pct, CAT_Utilization_Pct, Regional_Open_Capacity

## Story 1 — Action Required

- Question: What requires immediate attention?
- Output: Action Required
- Audience: Animal Flow
- Action: Assign operational tasks and escalate critical centres
- Supporting Signals: Emergency_Closure_Flag, Missing_Kennel_Assignments, DOG_Utilization_Pct

## Story 2 — Intake Readiness

- Question: Which centres can safely receive incoming animals?
- Output: Intake Readiness
- Audience: Animal Flow
- Action: Route intake to Candidate Centres
- Supporting Signals: DOG_Open_Spaces, CAT_Open_Spaces, Capacity_Confirmation_Age_Hours

## Story 3 — Placement Prioritization

- Question: Which centres should be prioritized for intake?
- Output: Placement Decision Board
- Audience: Animal Flow
- Action: Rank centres by readiness and logistics
- Supporting Signals: DOG_Open_Spaces, Regional_Travel_Time, DOG_Utilization_Pct

## Story 4 — Capacity Analysis

- Question: Why can or cannot centres receive additional animals?
- Output: Capacity Analysis
- Audience: Animal Flow
- Action: Provide root-cause analysis and mitigation suggestions
- Supporting Signals: DOG_Utilization_Pct, CAT_Utilization_Pct, Emergency_Closure_Flag

## Story 5 — Data Trust

- Question: Can the information be trusted?
- Output: Data Trust Summary
- Audience: Animal Flow
- Action: Initiate data reconciliation and prevent automated routing if critical
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
- Supporting Signals: Actionable queue from prior stories

---

# SECTION 08 — PAGE ARCHETYPE & LAYOUT BLUEPRINT

- Summary Page: Provincial KPIs and regional heatmap
- Centre Diagnostic Page: per-centre metrics and action buttons
- Operations Tasking Page: actionable queue and owner assignment

Wireframe guidance: keep top-level actions immediately actionable (one-click route, one-click escalate), surface data trust alongside each centre card.

---

# SECTION 09 — VISUAL RECOMMENDATIONS

- KPI Cards for capacity metrics (provincial and regional)
- Heatmap for regional pressure
- Priority Table for candidate centres with status badges
- Exception Cards for data-quality issues

Include short reason and data-source lines for each visual in implementation notes.

---

# SECTION 10 — IMPLEMENTATION NOTES

- Data latency: capacity signals expected <= 2h; emergency closures <= 15m
- Aggregation windows: 1-minute for closures; 5-minute rollups for utilization
- Suggested indexes: centre_id, timestamp on capacity and kennel tables
- Sample SQL snippets: include in downstream TRD and semantic model work

---

# SECTION 11 — VALIDATION CHECKLIST

- Primary Decision Defined — PASS
- Business Questions Defined — PASS
- Signals Defined — PASS
- Thresholds Defined — PASS
- Decision Traceability — PASS
- Story Blocks Completed — PASS
- Page Wireframe Provided — PASS
- Visual Recommendations Provided — PASS

Standards applied: REPORT_DESIGN_STANDARDS_v1.1, DECISION_STORY_GUIDELINES_v1.0

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
