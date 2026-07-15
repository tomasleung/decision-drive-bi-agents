# REPORT_STORY_v6.0.md
## Animal Flow — Live Capacity Reporting
### Decision Story Contract (DSC)

---

# Document Metadata

Document Type

Decision Story Contract

Version

4.0

Skill Variant

skill copy.md

Capability Name

Animal Flow — Live Capacity Reporting

Owner

Animal Flow

Purpose

Convert the approved BRD into a decision-driven report contract that validates decisions, questions, signals, thresholds, actions, and story flow before technical design begins.

Related Documents

- INPUT_BRD_AnimalFlow_LiveCapacity_v2.0
- REPORT_STORY_MATRIX_v6.0

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

## Capacity Availability

Capacity availability is determined by:

- Available DOG Spaces
- Available CAT Spaces
- DOG Utilization %
- CAT Utilization %

---

## Placement Eligibility

A centre is eligible when:

- Capacity Available
- Emergency Closure Inactive
- Capacity Information Current
- Data Quality Acceptable

---

# SECTION 04 — SIGNAL MATRIX

(See REPORT_STORY_MATRIX_v6.0 for full signal groupings and definitions)

---

# SECTION 05 — THRESHOLD MATRIX

- DOG Utilization %: <80% Candidate; 80-99% Monitor; >=100% Exclude
- CAT Utilization %: <80% Candidate; 80-99% Monitor; >=100% Exclude
- Missing Kennel Assignments: 0 Healthy; 1-3 Warning; >3 Critical
- Capacity Confirmation Age: <12h Current; 12-24h Aging; >24h Stale

---

# SECTION 06 — ACTION MATRIX

- Route intake to Candidate Centres
- Review Monitor band before routing
- Exclude centres with emergency closure or critical utilization
- Escalate stale confirmations to operations
- Trigger data cleanup for critical missing assignments

---

# SECTION 07 — NARRATIVE STORY

1. Provincial Snapshot: show capacity and regional pressure.
2. Intake Readiness: list candidate centres and exclusions.
3. Operational Actions: list review/escalation tasks.
4. Data Trust: surface data issues and remediation steps.

---

# SECTION 08 — PAGE ARCHETYPE

- Summary Page: provincial KPIs and regional heatmap
- Centre Diagnostic Page: per-centre metrics and action buttons
- Operations Tasking Page: queue of centres needing review

---

# SECTION 09 — LAYOUT BLUEPRINT

Primary reading order: Summary → Diagnostics → Action → Trust

---

# SECTION 10 — VISUAL RECOMMENDATIONS

- KPI Cards for capacity metrics
- Heatmap for regional pressure
- Priority Table for candidate centres
- Exception Cards for data-quality issues

---

# VALIDATION CHECKLIST

- Primary Decision Defined — PASS
- Questions Defined — PASS
- Signals Defined — PASS
- Thresholds Defined — PASS
- Actions Defined — PASS
- Story Flow Defined — PASS
- Standards Applied — PASS
- Guidelines Applied — PASS

***
