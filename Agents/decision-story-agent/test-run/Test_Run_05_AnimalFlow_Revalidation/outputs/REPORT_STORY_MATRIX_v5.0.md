# REPORT_STORY_MATRIX_v5.0.md
## Animal Flow — Live Capacity Reporting
### Decision Story Matrix

---

# Document Metadata

Document Type

Decision Story Matrix

Version

3.0

Capability

Animal Flow — Live Capacity Reporting

Purpose

Provide a fast-review decision framework before generating the full Decision Story Contract (DSC).

Skill Variant

skill_v2.2.md

Reference Files

- REPORT_DESIGN_STANDARDS_v1.0.md
- DECISION_STORY_GUIDELINES_v1.0.md
- 01_REPORT_STORY_MATRIX_TEMPLATE_v1.0.md
- INPUT_BRD_AnimalFlow_LiveCapacity_v2.0.md

---

# STEP 01 — DECISION MODEL

## Primary Decision

Which centres currently have sufficient capacity to support incoming animals?

---

## Secondary Decisions

- Which centres require intervention due to capacity or data issues?
- Which centres should be prioritized for intake?
- Which centres should be excluded from intake?
- Which regions are under the highest operational pressure?
- Which centres need data quality remediation?

---

## Decision Owner

Animal Flow Team

---

## Decision Frequency

Multiple Times Daily

---

## Key Discovery

A centre may have available physical space while still being unsuitable for intake when capacity confirmation, emergency closure, or data quality are compromised.

---

# STEP 02 — BUSINESS QUESTION MATRIX

| Business Question | Decision Category | Priority |
|-------------------|------------------|----------|
| Which centres currently have available DOG capacity? | Placement | Critical |
| Which centres currently have available CAT capacity? | Placement | Critical |
| Which centres are approaching critical utilization? | Capacity Risk | High |
| Which centres have emergency closures? | Eligibility | High |
| Which centres have stale or missing capacity confirmations? | Governance | High |
| Which centres have data-quality issues affecting placements? | Data Trust | High |
| Which regions are under capacity pressure? | Regional Monitoring | Medium |

---

# STEP 03 — SIGNAL MATRIX

## Placement Signals

Signals

- Total DOG Spaces
- Open DOG Spaces
- Total CAT Spaces
- Open CAT Spaces
- DOG Utilization %
- CAT Utilization %
- Emergency Closure Status

Supported Decision

```text
Which centres can safely receive incoming animals?
```

---

## Data Trust Signals

Signals

- Missing Kennel Assignments
- Capacity Confirmation Status
- Last Capacity Update
- ShelterBuddy Last Sync
- Assignment Accuracy %

Supported Decision

```text
Can the information be trusted for placement decisions?
```

---

# STEP 04 — ACTION MATRIX

## DOG Utilization %

| Threshold | Status | Action |
|------------|------------|------------|
| <80% | Healthy | Candidate Centre |
| 80%-99% | Monitor | Review Before Routing |
| >=100% | Full | Do Not Intake |

---

## CAT Utilization %

| Threshold | Status | Action |
|------------|------------|------------|
| <80% | Healthy | Candidate Centre |
| 80%-99% | Monitor | Review Before Routing |
| >=100% | Full | Do Not Intake |

---

## Missing Kennel Assignments

| Threshold | Status | Action |
|------------|------------|------------|
| 0 | Healthy | No Action |
| 1-3 | Warning | Review |
| >3 | Critical | Data Cleanup Required |

---

## Capacity Confirmation Age

| Threshold | Status | Action |
|------------|------------|------------|
| <12 Hours | Current | Use Normally |
| 12-24 Hours | Aging | Validate |
| >24 Hours | Stale | Contact Centre |

---

## Emergency Closure Status

| Status | Action |
|------------|------------|
| Active | Exclude Centre |
| Inactive | Normal Operations |

---

# STEP 05 — VALIDATION CHECKLIST

- Primary Decision Defined
- Questions Defined
- Signals Defined
- Thresholds Defined
- Actions Defined
- Story Flow Defined
- Standards Applied
- Guidelines Applied
- Decision Traceability Preserved

***
