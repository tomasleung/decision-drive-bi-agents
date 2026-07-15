# REPORT_STORY_v3.0.md
## Animal Flow — Live Capacity Reporting
### Decision Story Contract (DSC)

---

# Document Metadata

Document Type

Decision Story Contract

Version

2.0

Capability Name

Animal Flow — Live Capacity Reporting

Artifact Type

DSC

Owner

Animal Flow

Status

Approved

Purpose

Convert approved business requirements into a decision-driven report narrative, page structure, layout blueprint, and visual design contract before technical design begins.

Related Documents

```text
INPUT_BRD_AnimalFlow_LiveCapacity_v2.0

REPORT_STORY_MATRIX_v2.0
```

---

# SECTION 01 — DECISION MODEL

## Primary Decision

Which centres currently have sufficient capacity to support incoming animals?

---

## Secondary Decisions

- Which centres require operational intervention?
- Which centres should be prioritized for intake?
- Which centres should be avoided for intake?
- Which centres have data quality concerns?
- Which regions are experiencing capacity pressure?

---

## Decision Owner

Animal Flow Team

---

## Decision Frequency

Multiple Times Daily

---

## Governing Business Rule

Animal placement decisions must not rely solely on available space.

The governing placement decision is:

```text
DOG Capacity
+
CAT Capacity
+
DOG Utilization
+
CAT Utilization
+
Emergency Closure Status
+
Data Quality
+
Capacity Confirmation Status
=
Placement Readiness
```

---

## Key Discovery

A centre may have:

```text
Available Physical Space
```

and still be:

```text
Unable To Receive Additional Animals
```

because:

```text
Capacity Threshold Has Been Reached

OR

Emergency Closure Is Active

OR

Data Cannot Be Trusted
```

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

# SECTION 02 — BUSINESS QUESTION MATRIX

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
| Which centres have stale updates? | High |
| Which centres have not confirmed capacity status? | High |
| Which centres require data quality review? | High |

---

## Regional Questions

| Question | Priority |
|----------|----------|
| Which regions have the highest utilization? | Medium |
| Which regions are experiencing capacity pressure? | Medium |

---

# SECTION 03 — BUSINESS LOGIC MODEL

## Capacity Availability

Capacity availability is determined through:

```text
Available DOG Spaces

Available CAT Spaces

DOG Utilization %

CAT Utilization %
```

---

## Placement Eligibility

A centre is eligible when:

```text
Capacity Available

AND

Emergency Closure Inactive

AND

Capacity Information Current

AND

Data Quality Acceptable
```

---

## Data Trust

Data confidence is determined through:

```text
Missing Kennel Assignments

Assignment Accuracy %

Capacity Confirmation Status

Last Capacity Update

ShelterBuddy Synchronization Status
```

---

## Regional Monitoring

Regional pressure is evaluated using:

```text
Regional Utilization %

Regional Capacity %

Regional Open Capacity %
```

---

# SECTION 04 — SIGNAL MATRIX

## Provincial Snapshot Signals

```text
Total DOG Spaces

Open DOG Spaces

Total CAT Spaces

Open CAT Spaces

DOG Utilization %

CAT Utilization %
```

---

## Intake Readiness Signals

```text
Open DOG Spaces

Open CAT Spaces

DOG Utilization %

CAT Utilization %

Emergency Closure Status
```

---

## Data Trust Signals

```text
Missing Kennel Assignments

Assignment Accuracy %

Capacity Confirmation Status

Last Capacity Update

ShelterBuddy Last Sync
```

---

## Operational Risk Signals

```text
DOG Utilization %

CAT Utilization %

Emergency Closure Status

Capacity Confirmation Status
```

---

## Regional Signals

```text
Regional DOG Utilization %

Regional CAT Utilization %

Regional Capacity %

Regional Open Capacity %
```

---

# SECTION 05 — THRESHOLD MATRIX

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

## Emergency Closure

| Status | Action |
|------------|------------|
| Active | Exclude Centre |
| Inactive | Normal Operations |

---

# SECTION 06 — ACTION MATRIX

| Condition | Recommended Action |
|------------|------------|
