# REPORT_STORY_MATRIX_v6.0.md
## Animal Flow — Live Capacity Reporting
### Decision Story Matrix

---

# Document Metadata

Document Type

Decision Story Matrix

Version

4.0

Capability

Animal Flow — Live Capacity Reporting

Purpose

Provide a fast-review decision framework before generating the full Decision Story Contract (DSC).

Skill Variant

skill copy.md

Resolved Templates

- 01_REPORT_STORY_MATRIX_TEMPLATE_v2.0.md
- 02_REPORT_STORY_TEMPLATE_v2.0.md

Reference Files

- REPORT_DESIGN_STANDARDS_v1.0.md
- DECISION_STORY_GUIDELINES_v1.0.md
- INPUT_BRD_AnimalFlow_LiveCapacity_v2.0.md

---

# STEP 01 — DECISION MODEL

## Primary Decision

Which centres currently have sufficient capacity to support incoming animals?

---

## Secondary Decisions

- Which centres require operational intervention?
- Which centres should be prioritized for intake?
- Which centres should be excluded from intake?
- Which regions are experiencing capacity pressure?
- Which centres need data-quality remediation?

---

## Decision Owner

Animal Flow Team

---

## Decision Frequency

Multiple Times Daily

---

## Key Discovery

A centre can show available space yet be unsuitable for intake due to emergency closure, stale confirmation, or data trust issues.

---

# STEP 02 — BUSINESS QUESTION MATRIX

## Placement Questions

| Question | Priority |
|----------|----------|
| Which centres currently have available DOG capacity? | Critical |
| Which centres currently have available CAT capacity? | Critical |
| Which centres should be prioritized for intake? | Critical |
| Which centres should be avoided for intake? | High |

---

## Capacity Questions

| Question | Priority |
|----------|----------|
| Which centres are approaching critical utilization? | High |
| Which centres have no available capacity? | High |
| Which centres have emergency closures? | High |

---

## Data Quality Questions

| Question | Priority |
|----------|----------|
| Which centres have missing kennel assignments? | High |
| Which centres have stale capacity confirmations? | High |
| Which centres require data quality review? | High |

---

## Regional Questions

| Question | Priority |
|----------|----------|
| Which regions have the highest utilization? | Medium |
| Which regions are experiencing capacity pressure? | Medium |

---

# STEP 03 — SIGNAL MATRIX

## Placement Signals

Signals

- Total DOG Spaces
- Open DOG Spaces
- Total CAT Spaces
- Open CAT Spaces

Supported Decision

```text
Which centres can safely receive incoming animals?
```

---

## Data Trust Signals

Signals

- Missing Kennel Assignments
- Assignment Accuracy %
- Capacity Confirmation Status
- Last Capacity Update

Supported Decision

```text
Can the information be trusted for placement decisions?
```

---

## Operational Signals

Signals

- DOG Utilization %
- CAT Utilization %
- Emergency Closure Status
- Capacity Confirmation Age

Supported Decision

```text
Which centres require intervention?
```

---

## Regional Signals

Signals

- Regional DOG Utilization %
- Regional CAT Utilization %
- Regional Open Capacity %
- Regional Capacity Availability

Supported Decision

```text
Which regions are experiencing pressure?
```

---

## Signal Validation

Every signal must:

```text
Support A Business Question

Support A Decision

Be Measurable

Be Actionable
```

---

# STEP 04 — ACTION MATRIX

## DOG Utilization %

| Threshold | Status | Action |
|------------|------------|------------|
| <80% | Healthy | Candidate Centre |
| 80%-99% | Monitor | Review Before Routing |
| >=100% | Full | Do Not Intake |

Supported Decision

```text
Can this centre receive additional DOG intake?
```

---

## CAT Utilization %

| Threshold | Status | Action |
|------------|------------|------------|
| <80% | Healthy | Candidate Centre |
| 80%-99% | Monitor | Review Before Routing |
| >=100% | Full | Do Not Intake |

Supported Decision

```text
Can this centre receive additional CAT intake?
```

---

## Missing Kennel Assignments

| Threshold | Status | Action |
|------------|------------|------------|
| 0 | Healthy | No Action |
| 1-3 | Warning | Review |
| >3 | Critical | Data Cleanup Required |

Supported Decision

```text
Can capacity information be trusted?
```

---

## Capacity Confirmation Age

| Threshold | Status | Action |
|------------|------------|------------|
| <12 Hours | Current | Use Normally |
| 12-24 Hours | Aging | Validate |
| >24 Hours | Stale | Contact Centre |

Supported Decision

```text
Should this centre be reviewed before placement?
```

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
