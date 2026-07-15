# REPORT_STORY_v5.0.md
## Animal Flow — Live Capacity Reporting
### Decision Story Contract (DSC)

---

# Document Metadata

Document Type

Decision Story Contract

Version

3.0

Skill Variant

skill_v2.2.md

Capability Name

Animal Flow — Live Capacity Reporting

Owner

Animal Flow

Purpose

Convert the approved BRD into a decision-driven report contract that validates decisions, questions, signals, thresholds, actions, and story flow before technical design begins.

Related Documents

- INPUT_BRD_AnimalFlow_LiveCapacity_v2.0
- REPORT_STORY_MATRIX_v5.0

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

# SECTION 03 — SIGNALS & THRESHOLDS

- Open DOG Spaces — Candidate if available and all quality checks pass
- Open CAT Spaces — Candidate if available and all quality checks pass
- DOG Utilization % — <80% candidate, 80-99% monitor, >=100% exclude
- CAT Utilization % — <80% candidate, 80-99% monitor, >=100% exclude
- Missing Kennel Assignments — 0 healthy, 1-3 warning, >3 critical
- Capacity Confirmation Status — current, aging, stale
- Emergency Closure Status — active exclude, inactive normal

---

# SECTION 04 — ACTION MATRIX

- Route intake to centres classified as candidate centres.
- Review centres in the monitor band before routing.
- Exclude centres with critical utilization or emergency closure.
- Escalate centres with stale capacity confirmations to operations.
- Trigger data cleanup for centres with critical missing assignments.

---

# SECTION 05 — STORY FLOW

1. Provincial Snapshot: describe capacity availability and regional pressure.
2. Intake Readiness: identify candidate centres and exclusions.
3. Operational Actions: define review, exclusion, and escalation tasks.
4. Data Trust: surface quality issues and remediation requirements.

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
