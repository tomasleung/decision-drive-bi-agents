# ANIMALFLOW_REPORT_STORY_MATRIX_GOLD_v1.0

## Animal Flow — Live Capacity Reporting

### Decision Story Matrix

---

# Document Metadata

Document Type

Decision Story Matrix

Version

1.0

Capability

Animal Flow — Live Capacity Reporting

Purpose

Provide the approved Gold Standard decision framework used to evaluate all future Decision Story Agent outputs.

Audience

- Product Owner
- Business Owner
- Report Designer
- BI Developer
- Solution Architect
- Data Architect

Approval Gate

This artifact serves as the official benchmark and review target for:

- Decision Story Agent
- Decision Story Review Agent
- Template Evolution Agent

Related Governance

```text
DECISION_STORY_GOLD_OUTPUT_SPEC_v1.0

DECISION_STORY_REVIEW_CRITERIA_v1.0

DECISION_STORY_SCORING_MODEL_v1.0
```

Source Artifacts

```text
INPUT_BRD_AnimalFlow_LiveCapacity_v2.0

REPORT_STORY_MATRIX_v1.0

REPORT_STORY_v1.0

REPORT_STORY_MATRIX_v8.0

REPORT_STORY_v8.0
```

Purpose Statement

```text
This document represents the approved
Gold Output for Animal Flow.

All future Decision Story outputs
should be reviewed against this artifact.
```
# STEP 01 — DECISION MODEL

## Primary Decision

Which centres currently have sufficient capacity to support incoming animals?

---

## Secondary Decisions

- Which centres should be prioritized for intake?
- Which centres should be excluded from intake?
- Which centres require operational intervention?
- Which centres require data quality intervention?
- Which centres should be reviewed before placement decisions?
- Which centres have capacity constraints that prevent intake?
- Which regions are experiencing capacity pressure?
- Which regions require proactive operational support?

---

## Decision Owner

Animal Flow Team

---

## Decision Frequency

Multiple Times Daily

Examples

```text
Morning Intake Planning

Transport Routing

Emergency Intake Requests

Same-Day Placement Decisions

Operational Escalation Review
```

---

## Governing Business Rule

Animal placement decisions must not rely solely on available physical space.

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

A centre may appear available because physical space exists.

However, physical space alone does not determine intake readiness.

A centre may still be unsuitable for intake when:

```text
Capacity Threshold Reached

OR

Emergency Closure Active

OR

Capacity Confirmation Stale

OR

Data Quality Risk Exists
```

The business currently evaluates:

```text
Open Spaces
```

The actual decision requires:

```text
Capacity

+

Eligibility

+

Data Trust

+

Operational Readiness
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

without reviewing raw operational records.

---

## Decision Outcomes

The report must support the following outcomes:

### Outcome 01

```text
Identify Candidate Intake Centres
```

---

### Outcome 02

```text
Identify Centres Requiring Review
```

---

### Outcome 03

```text
Identify Centres Requiring Exclusion
```

---

### Outcome 04

```text
Identify Data Trust Risks
```

---

### Outcome 05

```text
Prioritize Placement Decisions
```

---

### Outcome 06

```text
Monitor Regional Capacity Pressure
```

---

## Decision Validation

The Decision Model succeeds when:

```text
Every Decision

supports a Business Outcome

Every Business Outcome

supports a User Action

Every User Action

supports Animal Placement Decisions
```

and users can determine:

```text
Where To Place Animals

Where Not To Place Animals

What Risks Exist

What Actions Must Be Taken
```

without manually analyzing centre-level operational data.

# STEP 02 — BUSINESS QUESTION MATRIX

## Purpose

Define the complete set of business questions required to support the Primary Decision.

Every question must:

```text
Support A Decision

Support A User Action

Support A Report Story

Support At Least One Signal
```

---

## Placement Questions

| Business Question | Decision Category | Priority |
|----------|----------|----------|
| Which centres currently have available DOG capacity? | Placement | Critical |
| Which centres currently have available CAT capacity? | Placement | Critical |
| Which centres should be prioritized for intake? | Placement | Critical |
| Which centres should be avoided for intake? | Placement | High |
| Which centres can safely receive incoming animals right now? | Placement | Critical |

---

## Capacity Questions

| Business Question | Decision Category | Priority |
|----------|----------|----------|
| Which centres are approaching critical utilization? | Capacity | High |
| Which centres have reached maximum utilization? | Capacity | High |
| Which centres have the greatest remaining intake capacity? | Capacity | High |
| Which centres have limited operational headroom? | Capacity | High |

---

## Operations Questions

| Business Question | Decision Category | Priority |
|----------|----------|----------|
| Which centres require operational intervention? | Operations | High |
| Which centres require immediate follow-up? | Operations | High |
| Which centres require manual review before placement? | Operations | High |

---

## Eligibility Questions

| Business Question | Decision Category | Priority |
|----------|----------|----------|
| Which centres have emergency closures? | Eligibility | High |
| Which centres should be excluded from intake immediately? | Eligibility | High |
| Which centres currently fail intake eligibility rules? | Eligibility | High |

---

## Data Trust Questions

| Business Question | Decision Category | Priority |
|----------|----------|----------|
| Which centres have missing kennel assignments? | Data Quality | High |
| Which centres have stale capacity updates? | Data Quality | High |
| Which centres have not confirmed capacity status? | Governance | High |
| Which centres have unreliable operational data? | Data Quality | High |
| Can the information be trusted for automated placement decisions? | Data Trust | Critical |

---

## Governance Questions

| Business Question | Decision Category | Priority |
|----------|----------|----------|
| Which centres require confirmation before placement decisions? | Governance | High |
| Which centres have exceeded acceptable data freshness thresholds? | Governance | High |
| Which centres require escalation due to unresolved issues? | Governance | High |

---

## Regional Monitoring Questions

| Business Question | Decision Category | Priority |
|----------|----------|----------|
| Which regions are experiencing capacity pressure? | Regional Monitoring | Medium |
| Which regions have the highest utilization rates? | Regional Monitoring | Medium |
| Which regions have the greatest available intake capacity? | Regional Monitoring | Medium |
| Which regions should be monitored closely over the next operational period? | Regional Monitoring | Medium |

---

## Executive Oversight Questions

| Business Question | Decision Category | Priority |
|----------|----------|----------|
| What is happening across the province today? | Executive Oversight | Medium |
| Where are the largest operational risks? | Executive Oversight | Medium |
| What actions should be prioritized by leadership? | Executive Oversight | Medium |

---

## Question Coverage Summary

| Category | Question Count |
|----------|----------:|
| Placement | 5 |
| Capacity | 4 |
| Operations | 3 |
| Eligibility | 3 |
| Data Trust | 5 |
| Governance | 3 |
| Regional Monitoring | 4 |
| Executive Oversight | 3 |

Total Questions

```text
30
```

---

## Business Question Validation

Every question must satisfy the following:

### Decision Support

```text
Question

↓

Decision
```

---

### Signal Support

```text
Question

↓

Signal
```

---

### Action Support

```text
Question

↓

Action
```

---

### Story Support

```text
Question

↓

Story Section
```

---

## Gold Standard Validation

This section succeeds when:

```text
All Critical Decisions
are represented.

All Major Business Risks
are represented.

All Operational Actions
are represented.

All Report Stories
can be traced to at least one Business Question.
```
# STEP 03 — SIGNAL MATRIX

## Purpose

Define the signal groups required to support business questions, decisions, thresholds, actions, and report stories.

Signal Groups provide business organization.

Signal Contracts provide business definitions.

Both are required.

---

# Placement Signals

## Supported Decisions

```text
Placement Eligibility

Candidate Centre Selection

Placement Prioritization
```

### Signals

- Total_DOG_Spaces
- Open_DOG_Spaces
- Total_CAT_Spaces
- Open_CAT_Spaces
- DOG_Utilization_Pct
- CAT_Utilization_Pct
- Emergency_Closure_Flag

---

## Business Questions Supported

```text
Which centres currently have available DOG capacity?

Which centres currently have available CAT capacity?

Which centres can safely receive incoming animals?

Which centres should be prioritized for intake?

Which centres should be avoided for intake?
```

---

# Capacity Signals

## Supported Decisions

```text
Capacity Monitoring

Capacity Risk Assessment

Intake Readiness
```

### Signals

- DOG_Utilization_Pct
- CAT_Utilization_Pct
- Available_DOG_Capacity
- Available_CAT_Capacity
- Total_Open_Capacity
- Capacity_Pressure_Index

---

## Business Questions Supported

```text
Which centres are approaching critical utilization?

Which centres have reached maximum utilization?

Which centres have the greatest remaining intake capacity?

Which centres have limited operational headroom?
```

---

# Operational Signals

## Supported Decisions

```text
Operational Escalation

Operational Intervention

Intake Review
```

### Signals

- Emergency_Closure_Flag
- DOG_Utilization_Pct
- CAT_Utilization_Pct
- Capacity_Confirmation_Status
- Capacity_Confirmation_Age_Hours
- Operational_Review_Flag

---

## Business Questions Supported

```text
Which centres require intervention?

Which centres require immediate follow-up?

Which centres require manual review before intake?
```

---

# Eligibility Signals

## Supported Decisions

```text
Placement Eligibility

Centre Exclusion

Routing Decisions
```

### Signals

- Emergency_Closure_Flag
- DOG_Utilization_Pct
- CAT_Utilization_Pct
- Placement_Eligibility_Status
- Intake_Block_Flag

---

## Business Questions Supported

```text
Which centres have emergency closures?

Which centres should be excluded immediately?

Which centres fail intake eligibility rules?
```

---

# Data Trust Signals

## Supported Decisions

```text
Data Trust Assessment

Automated Routing Approval

Data Quality Escalation
```

### Signals

- Missing_Kennel_Assignments
- Assignment_Accuracy_Pct
- Capacity_Confirmation_Status
- Capacity_Confirmation_Age_Hours
- Last_Capacity_Update
- ShelterBuddy_Last_Sync
- Data_Trust_Status

---

## Business Questions Supported

```text
Which centres have missing kennel assignments?

Which centres have stale capacity updates?

Which centres have not confirmed capacity status?

Can this information be trusted?

Which centres require data quality review?
```

---

# Governance Signals

## Supported Decisions

```text
Governance Review

Placement Approval

Escalation Review
```

### Signals

- Capacity_Confirmation_Status
- Capacity_Confirmation_Age_Hours
- Data_Trust_Status
- Escalation_Status
- Data_Freshness_Status

---

## Business Questions Supported

```text
Which centres require confirmation before placement?

Which centres violate freshness requirements?

Which centres require escalation?
```

---

# Regional Signals

## Supported Decisions

```text
Regional Monitoring

Regional Capacity Planning

Resource Allocation
```

### Signals

- Regional_DOG_Utilization_Pct
- Regional_CAT_Utilization_Pct
- Regional_Open_Capacity
- Regional_Open_Capacity_Pct
- Regional_Pressure_Index
- Regional_Candidate_Centres

---

## Business Questions Supported

```text
Which regions are experiencing capacity pressure?

Which regions have the highest utilization?

Which regions have the greatest available capacity?

Which regions require proactive intervention?
```

---

# Executive Signals

## Supported Decisions

```text
Executive Monitoring

Leadership Prioritization

Provincial Oversight
```

### Signals

- Provincial_DOG_Utilization_Pct
- Provincial_CAT_Utilization_Pct
- Provincial_Open_Capacity
- Provincial_Pressure_Index
- High_Risk_Centre_Count
- Eligible_Centre_Count

---

## Business Questions Supported

```text
What is happening across the province today?

Where are the largest operational risks?

What actions should leadership prioritize?
```

---

# Signal Coverage Summary

| Signal Group | Signal Count |
|----------|----------:|
| Placement Signals | 7 |
| Capacity Signals | 6 |
| Operational Signals | 6 |
| Eligibility Signals | 5 |
| Data Trust Signals | 7 |
| Governance Signals | 5 |
| Regional Signals | 6 |
| Executive Signals | 6 |

Total Signals

```text
48
```

---

# Signal Validation Rules

Every Signal must:

```text
Support At Least One Business Question

Support At Least One Decision

Support At Least One Report Story

Be Measurable

Be Explainable

Be Actionable
```

---

# Signal Traceability Requirement

Every Signal must support:

```text
Question

↓

Decision

↓

Threshold

↓

Action

↓

Story

↓

Visual
```

---

# Gold Standard Validation

This section succeeds when:

```text
All Business Questions
have supporting signals.

All Major Decisions
have supporting signals.

All Stories
have supporting signals.

No Signal
exists without a business purpose.
```
# STEP 04 — SIGNAL CONTRACTS

## Purpose

Signal Contracts define the business meaning of every critical signal used in decision making.

Signal Contracts are the authoritative business definition for:

```text
Business Users

Report Designers

Mockup Agent

TRD Agent

Semantic Design Agent

Future Review Agents
```

They describe:

```text
Why The Signal Exists

What The Signal Means

What Decision The Signal Supports

How The Signal Should Be Interpreted
```

---

# Placement Signal Contracts

| Signal | Business Purpose | Business Definition | Unit | Source | Question Supported | Decision Supported | Validation Rule | Example |
|----------|----------|----------|----------|----------|----------|----------|----------|----------|
| Open_DOG_Spaces | Determine available DOG intake capacity | Number of DOG-capable spaces available for immediate intake | Spaces | Shelter System | Which centres currently have available DOG capacity? | Placement Eligibility | Must be non-negative | 12 |
| Open_CAT_Spaces | Determine available CAT intake capacity | Number of CAT-capable spaces available for immediate intake | Spaces | Shelter System | Which centres currently have available CAT capacity? | Placement Eligibility | Must be non-negative | 8 |
| DOG_Utilization_Pct | Measure DOG occupancy pressure | Percentage of DOG capacity currently occupied | Percent | Shelter System | Which centres are approaching critical utilization? | Capacity Monitoring | Must be between 0% and 200% | 84% |
| CAT_Utilization_Pct | Measure CAT occupancy pressure | Percentage of CAT capacity currently occupied | Percent | Shelter System | Which centres are approaching critical utilization? | Capacity Monitoring | Must be between 0% and 200% | 72% |
| Emergency_Closure_Flag | Determine intake eligibility | Indicates whether a centre has an active emergency closure | Boolean | Operations Feed | Which centres should be excluded? | Intake Eligibility | Must be TRUE/FALSE | TRUE |

---

# Capacity Signal Contracts

| Signal | Business Purpose | Business Definition | Unit | Source | Question Supported | Decision Supported | Validation Rule | Example |
|----------|----------|----------|----------|----------|----------|----------|----------|----------|
| Available_DOG_Capacity | Measure remaining DOG intake capability | Remaining available DOG intake capacity after occupancy | Spaces | Shelter System | Which centres have remaining DOG capacity? | Placement Prioritization | Must be non-negative | 16 |
| Available_CAT_Capacity | Measure remaining CAT intake capability | Remaining available CAT intake capacity after occupancy | Spaces | Shelter System | Which centres have remaining CAT capacity? | Placement Prioritization | Must be non-negative | 11 |
| Total_Open_Capacity | Measure overall intake readiness | Total number of available intake spaces | Spaces | Shelter System | Which centres have greatest capacity? | Candidate Selection | Must be non-negative | 27 |
| Capacity_Pressure_Index | Measure operational crowding | Business indicator summarizing utilization pressure across species | Index | Derived Business Logic | Which centres are under pressure? | Capacity Risk | Value must be defined | Moderate |

---

# Operational Signal Contracts

| Signal | Business Purpose | Business Definition | Unit | Source | Question Supported | Decision Supported | Validation Rule | Example |
|----------|----------|----------|----------|----------|----------|----------|----------|----------|
| Operational_Review_Flag | Identify centres requiring intervention | Indicates a centre requires operational review before placement | Boolean | Business Rules | Which centres require intervention? | Operational Escalation | Must be TRUE/FALSE | TRUE |
| Capacity_Confirmation_Status | Assess readiness confidence | Indicates whether capacity information has been confirmed | Status | Centre Confirmation Feed | Which centres require review? | Operational Readiness | Must have valid status | Confirmed |
| Capacity_Confirmation_Age_Hours | Measure confirmation freshness | Hours since last capacity confirmation | Hours | Centre Confirmation Feed | Which centres require confirmation? | Operational Review | Must be non-negative | 6 |

---

# Data Trust Signal Contracts

| Signal | Business Purpose | Business Definition | Unit | Source | Question Supported | Decision Supported | Validation Rule | Example |
|----------|----------|----------|----------|----------|----------|----------|----------|----------|
| Missing_Kennel_Assignments | Identify data quality risk | Number of animals without assigned kennel records | Count | Intake System | Which centres have data quality issues? | Data Trust | Must be non-negative integer | 4 |
| Assignment_Accuracy_Pct | Assess assignment integrity | Percentage of valid kennel assignments | Percent | Intake System | Can the information be trusted? | Data Trust | Must be between 0% and 100% | 98% |
| Data_Trust_Status | Overall trust indicator | Business assessment of whether data is suitable for decision making | Status | Derived Business Rules | Can this information be trusted? | Routing Approval | Must have valid status | Trusted |
| Last_Capacity_Update | Measure update freshness | Timestamp of latest capacity refresh | Timestamp | Shelter System | Which centres have stale updates? | Data Trust | Must exist | 2026-07-17 09:00 |
| ShelterBuddy_Last_Sync | Measure system synchronization | Timestamp of latest ShelterBuddy synchronization | Timestamp | ShelterBuddy | Can data be trusted? | Governance | Must exist | 2026-07-17 08:55 |

---

# Governance Signal Contracts

| Signal | Business Purpose | Business Definition | Unit | Source | Question Supported | Decision Supported | Validation Rule | Example |
|----------|----------|----------|----------|----------|----------|----------|----------|----------|
| Data_Freshness_Status | Determine decision readiness | Indicates whether data meets freshness requirements | Status | Business Rules | Which centres exceed freshness thresholds? | Governance Review | Must have valid status | Current |
| Escalation_Status | Track governance actions | Indicates whether unresolved issues require escalation | Status | Governance Process | Which centres require escalation? | Governance Review | Must have valid status | Escalated |

---

# Regional Signal Contracts

| Signal | Business Purpose | Business Definition | Unit | Source | Question Supported | Decision Supported | Validation Rule | Example |
|----------|----------|----------|----------|----------|----------|----------|----------|----------|
| Regional_DOG_Utilization_Pct | Measure regional DOG pressure | Aggregate DOG utilization across a region | Percent | Shelter System | Which regions have highest utilization? | Regional Monitoring | Must be between 0% and 200% | 86% |
| Regional_CAT_Utilization_Pct | Measure regional CAT pressure | Aggregate CAT utilization across a region | Percent | Shelter System | Which regions have highest utilization? | Regional Monitoring | Must be between 0% and 200% | 75% |
| Regional_Open_Capacity | Measure available regional intake space | Total available intake capacity in region | Spaces | Shelter System | Which regions have available capacity? | Regional Planning | Must be non-negative | 34 |
| Regional_Pressure_Index | Measure regional strain | Combined business indicator of regional pressure | Index | Derived Business Logic | Which regions need intervention? | Resource Allocation | Value must be defined | High |

---

# Executive Signal Contracts

| Signal | Business Purpose | Business Definition | Unit | Source | Question Supported | Decision Supported | Validation Rule | Example |
|----------|----------|----------|----------|----------|----------|----------|----------|----------|
| Provincial_Open_Capacity | Measure provincial intake readiness | Total available capacity across all centres | Spaces | Aggregated Shelter Data | What is happening across the province today? | Executive Monitoring | Must be non-negative | 122 |
| Provincial_Pressure_Index | Measure province-wide risk | Aggregate indicator of provincial capacity pressure | Index | Derived Business Logic | Where are the largest operational risks? | Executive Oversight | Value must be defined | Elevated |
| High_Risk_Centre_Count | Measure operational risk exposure | Number of centres currently classified as high risk | Count | Business Rules | What should leadership prioritize? | Executive Oversight | Must be non-negative | 5 |
| Eligible_Centre_Count | Measure placement opportunity | Number of centres currently eligible for intake | Count | Business Rules | What placement capacity exists today? | Executive Oversight | Must be non-negative | 19 |

---

# Signal Contract Validation

Every Signal Contract must define:

```text
Business Purpose

Business Definition

Unit

Source

Question Supported

Decision Supported

Validation Rule
```

---

# Signal Contract Success Statement

This section succeeds when:

```text
Every Signal

has a Business Purpose

Every Signal

supports a Business Question

Every Signal

supports a Decision

Every Signal

supports a Story

Every Signal

can be understood without technical documentation
```
# STEP 05 — THRESHOLD MATRIX

## Purpose

Thresholds convert signals into business decisions.

Every threshold must define:

```text
What Happened

↓

Why It Matters

↓

What Action Should Be Taken
```

Thresholds are used by:

```text
Animal Flow Team

Operations

Leadership

Decision Story Agent

Review Agent

Future Rule Engines
```

---

# DOG_Utilization_Pct

## Supported Decision

```text
Can this centre safely receive additional DOG intake?
```

| Threshold | Status | Action | Business Meaning |
|----------|----------|----------|----------|
| < 80% | Healthy | Candidate Centre | Centre has sufficient DOG capacity and can be considered for intake placement. |
| 80% – 99% | Monitor | Review Before Routing | Centre remains eligible but is approaching capacity pressure. |
| >= 100% | Full | Do Not Intake | Centre has reached or exceeded DOG capacity and must be excluded from intake. |

---

## Business Interpretation

```text
Healthy

↓

Preferred Intake Candidate

Monitor

↓

Operational Review Required

Full

↓

Exclude From Intake
```

---

# CAT_Utilization_Pct

## Supported Decision

```text
Can this centre safely receive additional CAT intake?
```

| Threshold | Status | Action | Business Meaning |
|----------|----------|----------|----------|
| < 80% | Healthy | Candidate Centre | Centre has sufficient CAT capacity available. |
| 80% – 99% | Monitor | Review Before Routing | Capacity pressure is increasing and requires validation before placement. |
| >= 100% | Full | Do Not Intake | Centre must be excluded from CAT intake activity. |

---

## Business Interpretation

```text
Healthy

↓

Preferred CAT Placement

Monitor

↓

Verify Capacity Before Placement

Full

↓

Exclude From Placement
```

---

# Total_Open_Capacity

## Supported Decision

```text
Which centres should be prioritized?
```

| Threshold | Status | Action | Business Meaning |
|----------|----------|----------|----------|
| > 20 Spaces | High Capacity | Prioritize | Centre has substantial intake capacity available. |
| 10 – 20 Spaces | Moderate Capacity | Consider | Centre remains a viable placement option. |
| < 10 Spaces | Low Capacity | Lower Priority | Capacity exists but should be used cautiously. |
| 0 Spaces | No Capacity | Exclude | No remaining intake space exists. |

---

# Capacity_Pressure_Index

## Supported Decision

```text
Which centres are under operational pressure?
```

| Threshold | Status | Action | Business Meaning |
|----------|----------|----------|----------|
| Low | Healthy | Continue Operations | Capacity pressure is not impacting operations. |
| Moderate | Monitor | Review Daily | Capacity pressure should be monitored. |
| High | Risk | Operational Review | Pressure is creating operational constraints. |
| Critical | Escalate | Immediate Intervention | Immediate action required to prevent intake disruption. |

---

# Emergency_Closure_Flag

## Supported Decision

```text
Is the centre eligible for intake?
```

| Threshold | Status | Action | Business Meaning |
|----------|----------|----------|----------|
| FALSE | Eligible | Continue Evaluation | Centre remains eligible for placement review. |
| TRUE | Excluded | Exclude Centre | Centre cannot participate in intake while closure is active. |

---

## Business Interpretation

```text
Emergency Closure

↓

Overrides All Other Placement Rules

↓

Immediate Exclusion
```

---

# Missing_Kennel_Assignments

## Supported Decision

```text
Can operational data be trusted?
```

| Threshold | Status | Action | Business Meaning |
|----------|----------|----------|----------|
| 0 | Healthy | No Action | Data is complete and trusted. |
| 1 – 3 | Warning | Review | Minor quality issues require validation. |
| > 3 | Critical | Data Cleanup Required | Data quality risk is too high for automated routing. |

---

## Business Interpretation

```text
Healthy

↓

Trusted

Warning

↓

Review Required

Critical

↓

Block Automation
```

---

# Assignment_Accuracy_Pct

## Supported Decision

```text
Can placement decisions rely on assignment data?
```

| Threshold | Status | Action | Business Meaning |
|----------|----------|----------|----------|
| >= 99% | Trusted | Use Normally | Assignment quality is highly reliable. |
| 95% – 98% | Review | Validate | Minor concerns exist. |
| < 95% | High Risk | Escalate | Assignment quality may affect placement decisions. |

---

# Capacity_Confirmation_Age_Hours

## Supported Decision

```text
Can capacity information be trusted?
```

| Threshold | Status | Action | Business Meaning |
|----------|----------|----------|----------|
| < 12 Hours | Current | Use Normally | Capacity confirmation is fresh and reliable. |
| 12 – 24 Hours | Aging | Validate | Confirmation is becoming stale and should be checked. |
| > 24 Hours | Stale | Contact Centre | Capacity information can no longer be trusted without reconfirmation. |

---

## Business Interpretation

```text
Current

↓

Trusted

Aging

↓

Validate

Stale

↓

Contact Centre
```

---

# Data_Trust_Status

## Supported Decision

```text
Should automated placement decisions proceed?
```

| Threshold | Status | Action | Business Meaning |
|----------|----------|----------|----------|
| Trusted | Proceed | Continue Routing | Data quality supports automated decision making. |
| Review Required | Validate | Manual Review | Additional confirmation is required. |
| Not Trusted | Block | Stop Automated Routing | Automated placement decisions should not proceed. |

---

# Regional_Pressure_Index

## Supported Decision

```text
Which regions require intervention?
```

| Threshold | Status | Action | Business Meaning |
|----------|----------|----------|----------|
| Low | Healthy | Monitor | Region operating normally. |
| Moderate | Watch | Monitor Closely | Capacity pressure beginning to emerge. |
| High | Risk | Allocate Resources | Operational support may be required. |
| Critical | Escalate | Leadership Intervention | Region requires immediate attention and planning. |

---

# Provincial_Pressure_Index

## Supported Decision

```text
What is the province-wide operating condition?
```

| Threshold | Status | Action | Business Meaning |
|----------|----------|----------|----------|
| Low | Healthy | Continue Operations | Provincial capacity remains stable. |
| Moderate | Monitor | Increase Observation | Conditions should be observed closely. |
| High | Alert | Prepare Response | System-wide pressure is creating risk. |
| Critical | Escalate | Provincial Action Plan | Immediate province-wide intervention required. |

---

# Threshold Validation

Every Threshold must define:

```text
Threshold

Status

Action

Business Meaning
```

---

# Threshold Traceability Requirement

Every Threshold must trace to:

```text
Signal

↓

Decision

↓

Action

↓

Story

↓

Visual
```

---

# Gold Standard Validation

This section succeeds when:

```text
Every Critical Signal
has thresholds

Every Threshold
produces an action

Every Action
supports a decision

Every Decision
supports the primary business outcome
```

and users can immediately determine:

```text
What Happened

Why It Matters

What To Do Next
```
# STEP 06 — DECISION TRACEABILITY

## Purpose

Decision Traceability ensures every business question can be traced through the entire decision chain.

The objective is to eliminate:

```text
Unnecessary Signals

Unused Metrics

Orphan Visuals

Non-Actionable Reporting
```

Every element in the report must support:

```text
Question

↓

Signal

↓

Threshold

↓

Decision

↓

Action

↓

Story

↓

Visual
```

---

# Placement Decision Traceability

| Business Question | Signal | Threshold | Decision | Resulting Action |
|----------|----------|----------|----------|----------|
| Which centres currently have available DOG capacity? | Open_DOG_Spaces | > 0 Spaces | DOG Placement Eligibility | Candidate Centre |
| Which centres currently have available CAT capacity? | Open_CAT_Spaces | > 0 Spaces | CAT Placement Eligibility | Candidate Centre |
| Which centres can safely receive incoming animals? | DOG_Utilization_Pct | < 80% | Intake Eligibility | Candidate Centre |
| Which centres can safely receive incoming animals? | CAT_Utilization_Pct | < 80% | Intake Eligibility | Candidate Centre |
| Which centres should be prioritized for intake? | Total_Open_Capacity | > 20 Spaces | Placement Prioritization | Prioritize Centre |
| Which centres should be avoided for intake? | DOG_Utilization_Pct | >= 100% | Placement Exclusion | Do Not Intake |
| Which centres should be avoided for intake? | CAT_Utilization_Pct | >= 100% | Placement Exclusion | Do Not Intake |

---

# Eligibility Decision Traceability

| Business Question | Signal | Threshold | Decision | Resulting Action |
|----------|----------|----------|----------|----------|
| Which centres have emergency closures? | Emergency_Closure_Flag | TRUE | Centre Eligibility | Exclude Centre |
| Which centres should be excluded immediately? | Emergency_Closure_Flag | TRUE | Intake Exclusion | Exclude Centre |
| Which centres fail intake eligibility rules? | Intake_Block_Flag | Active | Eligibility Review | Do Not Intake |

---

# Capacity Decision Traceability

| Business Question | Signal | Threshold | Decision | Resulting Action |
|----------|----------|----------|----------|----------|
| Which centres are approaching critical utilization? | DOG_Utilization_Pct | 80% - 99% | Capacity Risk Assessment | Review Before Routing |
| Which centres are approaching critical utilization? | CAT_Utilization_Pct | 80% - 99% | Capacity Risk Assessment | Review Before Routing |
| Which centres have reached maximum utilization? | DOG_Utilization_Pct | >=100% | Capacity Exceeded | Do Not Intake |
| Which centres have reached maximum utilization? | CAT_Utilization_Pct | >=100% | Capacity Exceeded | Do Not Intake |
| Which centres have limited operational headroom? | Capacity_Pressure_Index | High | Capacity Risk Assessment | Operational Review |

---

# Operational Decision Traceability

| Business Question | Signal | Threshold | Decision | Resulting Action |
|----------|----------|----------|----------|----------|
| Which centres require intervention? | Operational_Review_Flag | TRUE | Operational Escalation | Assign Review Task |
| Which centres require immediate follow-up? | Capacity_Pressure_Index | Critical | Operational Escalation | Immediate Intervention |
| Which centres require manual review before intake? | Capacity_Confirmation_Status | Review Required | Operational Readiness | Review Before Routing |

---

# Data Trust Decision Traceability

| Business Question | Signal | Threshold | Decision | Resulting Action |
|----------|----------|----------|----------|----------|
| Which centres have missing kennel assignments? | Missing_Kennel_Assignments | >3 | Data Trust Review | Data Cleanup Required |
| Which centres have stale capacity updates? | Capacity_Confirmation_Age_Hours | >24 Hours | Data Freshness Review | Contact Centre |
| Which centres have not confirmed capacity status? | Capacity_Confirmation_Status | Missing | Governance Review | Request Confirmation |
| Which centres have unreliable operational data? | Data_Trust_Status | Not Trusted | Data Trust Decision | Block Automated Routing |
| Can the information be trusted? | Assignment_Accuracy_Pct | <95% | Data Trust Decision | Escalate Review |

---

# Governance Decision Traceability

| Business Question | Signal | Threshold | Decision | Resulting Action |
|----------|----------|----------|----------|----------|
| Which centres require confirmation before placement decisions? | Capacity_Confirmation_Age_Hours | >24 Hours | Governance Review | Contact Centre |
| Which centres exceed freshness requirements? | Data_Freshness_Status | Stale | Governance Review | Escalate Issue |
| Which centres require escalation? | Escalation_Status | Escalated | Governance Review | Assign Escalation Owner |

---

# Regional Decision Traceability

| Business Question | Signal | Threshold | Decision | Resulting Action |
|----------|----------|----------|----------|----------|
| Which regions are experiencing capacity pressure? | Regional_Pressure_Index | High | Regional Capacity Review | Allocate Resources |
| Which regions have the highest utilization? | Regional_DOG_Utilization_Pct | >85% | Regional Monitoring | Monitor Region |
| Which regions have the highest utilization? | Regional_CAT_Utilization_Pct | >85% | Regional Monitoring | Monitor Region |
| Which regions require proactive intervention? | Regional_Pressure_Index | Critical | Regional Escalation | Leadership Review |

---

# Executive Decision Traceability

| Business Question | Signal | Threshold | Decision | Resulting Action |
|----------|----------|----------|----------|----------|
| What is happening across the province today? | Provincial_Pressure_Index | Any | Executive Monitoring | Situational Awareness |
| Where are the largest operational risks? | High_Risk_Centre_Count | >0 | Risk Assessment | Review Risk Centres |
| What actions should leadership prioritize? | Eligible_Centre_Count | Defined Daily | Executive Prioritization | Allocate Resources |

---

# Story Traceability

Every Story must be traceable to at least one Business Question.

| Story | Business Question Supported |
|----------|----------|
| Story 0 — Provincial Snapshot | What is happening across the province today? |
| Story 1 — Action Required | What requires immediate attention? |
| Story 2 — Intake Readiness | Which centres can safely receive incoming animals? |
| Story 3 — Placement Prioritization | Which centres should be prioritized for intake? |
| Story 4 — Capacity Analysis | Why can or cannot centres receive additional animals? |
| Story 5 — Data Trust | Can the information be trusted? |
| Story 6 — Regional Health | Which regions are experiencing capacity pressure? |
| Story 7 — Operational Briefing | What should we do next? |

---

# Visual Traceability

Every visual must support a Story.

| Story | Visual |
|----------|----------|
| Provincial Snapshot | KPI Cards |
| Action Required | Exception KPI Cards |
| Intake Readiness | Status Cards |
| Placement Prioritization | Priority Table |
| Capacity Analysis | Comparison Cards |
| Data Trust | Exception Matrix |
| Regional Health | Regional Capacity Chart |
| Operational Briefing | Recommendation Cards |

---

# Traceability Validation

This section succeeds when:

```text
Every Question

Supports A Decision

Every Decision

Supports An Action

Every Action

Supports A Story

Every Story

Supports A Visual
```

and no element exists without supporting:

```text
Business Purpose

Decision Logic

Operational Action
```

---

# Gold Standard Validation

The traceability model must allow a reviewer to start from:

```text
Visual

↓

Story

↓

Action

↓

Decision

↓

Threshold

↓

Signal

↓

Question
```

or

```text
Question

↓

Signal

↓

Threshold

↓

Decision

↓

Action

↓

Story

↓

Visual
```

with no breaks in the decision chain.
# STEP 07 — ACTION MATRIX

## Purpose

The Action Matrix converts decisions into operational actions.

The objective is to ensure:

```text
No Signal

↓

No Threshold

↓

No Decision

exists without a defined action.
```

Every action must identify:

```text
What To Do

Who Does It

Why It Matters
```

---

# Placement Actions

| Condition | Recommended Action | Responsible Role | Priority |
|----------|----------|----------|----------|
| Open_DOG_Spaces > 0 AND DOG_Utilization_Pct < 80% | Designate as Candidate Centre | Animal Flow Operations | High |
| Open_CAT_Spaces > 0 AND CAT_Utilization_Pct < 80% | Designate as Candidate Centre | Animal Flow Operations | High |
| Total_Open_Capacity > 20 | Prioritize Intake Routing | Animal Flow Operations | High |
| Total_Open_Capacity 10 - 20 | Consider For Placement | Animal Flow Operations | Medium |
| Total_Open_Capacity < 10 | Use With Caution | Animal Flow Operations | Medium |
| Total_Open_Capacity = 0 | Remove From Intake Options | Animal Flow Operations | Critical |

---

# Capacity Risk Actions

| Condition | Recommended Action | Responsible Role | Priority |
|----------|----------|----------|----------|
| DOG_Utilization_Pct 80% - 99% | Review Before Routing | Animal Flow Operations | High |
| DOG_Utilization_Pct >= 100% | Do Not Intake DOGs | Animal Flow Operations | Critical |
| CAT_Utilization_Pct 80% - 99% | Review Before Routing | Animal Flow Operations | High |
| CAT_Utilization_Pct >= 100% | Do Not Intake CATs | Animal Flow Operations | Critical |
| Capacity_Pressure_Index = High | Assign Operational Review | Animal Flow Operations | High |
| Capacity_Pressure_Index = Critical | Escalate Immediately | Animal Flow Leadership | Critical |

---

# Eligibility Actions

| Condition | Recommended Action | Responsible Role | Priority |
|----------|----------|----------|----------|
| Emergency_Closure_Flag = TRUE | Exclude Centre Immediately | Animal Flow Operations | Critical |
| Intake_Block_Flag = Active | Remove From Routing Queue | Animal Flow Operations | Critical |
| Placement_Eligibility_Status = Ineligible | Prevent Placement Assignment | Animal Flow Operations | Critical |

---

# Operational Actions

| Condition | Recommended Action | Responsible Role | Priority |
|----------|----------|----------|----------|
| Operational_Review_Flag = TRUE | Assign Operational Review Task | Animal Flow Operations | High |
| Capacity_Confirmation_Status = Review Required | Perform Manual Validation | Animal Flow Operations | High |
| Capacity_Confirmation_Status = Missing | Contact Centre For Confirmation | Animal Flow Operations | Critical |
| Escalation_Status = Escalated | Assign Escalation Owner | Animal Flow Leadership | Critical |

---

# Data Trust Actions

| Condition | Recommended Action | Responsible Role | Priority |
|----------|----------|----------|----------|
| Missing_Kennel_Assignments = 0 | No Action Required | Data Team | Low |
| Missing_Kennel_Assignments 1 - 3 | Review Records | Data Team | Medium |
| Missing_Kennel_Assignments > 3 | Assign Data Cleanup | Data Team | Critical |
| Assignment_Accuracy_Pct < 95% | Perform Data Quality Investigation | Data Team | High |
| Data_Trust_Status = Review Required | Manual Decision Validation | Animal Flow Operations | High |
| Data_Trust_Status = Not Trusted | Block Automated Routing | Animal Flow Operations | Critical |

---

# Governance Actions

| Condition | Recommended Action | Responsible Role | Priority |
|----------|----------|----------|----------|
| Capacity_Confirmation_Age_Hours > 24 | Contact Centre Immediately | Animal Flow Operations | Critical |
| Data_Freshness_Status = Stale | Escalate Governance Review | Governance Team | High |
| Escalation_Status = Escalated | Schedule Escalation Review | Governance Team | High |

---

# Regional Actions

| Condition | Recommended Action | Responsible Role | Priority |
|----------|----------|----------|----------|
| Regional_Pressure_Index = Moderate | Monitor Region | Animal Flow Leadership | Medium |
| Regional_Pressure_Index = High | Reallocate Capacity Resources | Animal Flow Leadership | High |
| Regional_Pressure_Index = Critical | Activate Regional Intervention Plan | Animal Flow Leadership | Critical |
| Regional_Open_Capacity < Target Threshold | Review Regional Capacity Strategy | Animal Flow Leadership | High |

---

# Executive Actions

| Condition | Recommended Action | Responsible Role | Priority |
|----------|----------|----------|----------|
| Provincial_Pressure_Index = High | Prepare Provincial Response Plan | Executive Leadership | High |
| Provincial_Pressure_Index = Critical | Initiate Provincial Action Plan | Executive Leadership | Critical |
| High_Risk_Centre_Count > 0 | Review High-Risk Centres | Executive Leadership | High |
| Eligible_Centre_Count Below Target | Investigate Intake Constraints | Executive Leadership | Medium |

---

# Action Ownership Matrix

| Action Area | Primary Owner | Secondary Owner |
|----------|----------|----------|
| Placement Decisions | Animal Flow Operations | Centre Teams |
| Capacity Monitoring | Animal Flow Operations | Leadership |
| Data Quality | Data Team | Animal Flow Operations |
| Governance Review | Governance Team | Leadership |
| Regional Planning | Animal Flow Leadership | Regional Teams |
| Executive Oversight | Executive Leadership | Animal Flow Leadership |

---

# Action Validation Rules

Every action must:

```text
Support A Decision

Support A Business Outcome

Have A Responsible Owner

Be Operationally Actionable
```

---

# Escalation Rules

## Critical Escalation

Triggered by:

```text
Emergency Closure

Capacity Full

Critical Data Quality Issues

Critical Regional Pressure
```

Action:

```text
Immediate Intervention Required
```

---

## High Escalation

Triggered by:

```text
Utilization Risk

Stale Capacity Confirmation

Governance Violations
```

Action:

```text
Review Within Current Operational Cycle
```

---

## Medium Escalation

Triggered by:

```text
Emerging Capacity Pressure

Regional Monitoring Risks
```

Action:

```text
Monitor And Reassess
```

---

# Gold Standard Validation

This section succeeds when:

```text
Every Decision

Produces An Action

Every Action

Has An Owner

Every Owner

Can Execute The Action

Every Critical Risk

Has An Escalation Path
```

and users can clearly determine:

```text
What Should Be Done

Who Should Do It

When Action Is Required
```
# STEP 08 — STORY SUMMARY

## Purpose

The Story Summary defines the business narrative of the report.

The report must guide users through a structured decision journey:

```text
Context

↓

Attention Required

↓

Decision Readiness

↓

Prioritization

↓

Analysis

↓

Trust

↓

Regional Awareness

↓

Action
```

The report is successful when users can answer:

```text
Which centres currently have sufficient capacity
to support incoming animals?
```

within:

```text
30 Seconds
```

without manually reviewing raw operational data.

---

# Story 0 — Provincial Capacity Snapshot

## Question

```text
What is happening across the province today?
```

## Output

```text
Provincial Capacity Snapshot
```

## Audience

```text
Animal Flow

Leadership

Executive Stakeholders
```

## Action

```text
Understand overall provincial operating conditions.
```

## Supporting Signals

```text
Provincial_Open_Capacity

Provincial_Pressure_Index

High_Risk_Centre_Count

Eligible_Centre_Count
```

## Decision Supported

```text
Executive Monitoring

Provincial Oversight
```

## Purpose

Provide immediate situational awareness and overall capacity status.

---

# Story 1 — Action Required

## Question

```text
What requires immediate attention?
```

## Output

```text
Action Required
```

## Audience

```text
Animal Flow Operations

Leadership
```

## Action

```text
Identify urgent operational and data quality risks.
```

## Supporting Signals

```text
Emergency_Closure_Flag

Missing_Kennel_Assignments

Capacity_Pressure_Index

Data_Trust_Status
```

## Decision Supported

```text
Operational Escalation

Risk Management
```

## Purpose

Highlight issues requiring immediate intervention.

---

# Story 2 — Intake Readiness

## Question

```text
Which centres can safely receive incoming animals?
```

## Output

```text
Intake Readiness
```

## Audience

```text
Animal Flow Operations
```

## Action

```text
Identify candidate intake centres.
```

## Supporting Signals

```text
Open_DOG_Spaces

Open_CAT_Spaces

DOG_Utilization_Pct

CAT_Utilization_Pct

Emergency_Closure_Flag
```

## Decision Supported

```text
Placement Eligibility
```

## Purpose

Provide a clear intake eligibility view for day-to-day placement decisions.

---

# Story 3 — Placement Decision Board

## Question

```text
Which centres should be prioritized for intake?
```

## Output

```text
Placement Decision Board
```

## Audience

```text
Animal Flow Operations
```

## Action

```text
Prioritize and rank placement options.
```

## Supporting Signals

```text
Total_Open_Capacity

Available_DOG_Capacity

Available_CAT_Capacity

Capacity_Pressure_Index
```

## Decision Supported

```text
Placement Prioritization
```

## Purpose

Enable fast identification of the best placement opportunities.

---

# Story 4 — Capacity Analysis

## Question

```text
Why can or cannot centres receive additional animals?
```

## Output

```text
Capacity Analysis
```

## Audience

```text
Animal Flow Operations

Centre Management
```

## Action

```text
Understand the drivers behind intake eligibility.
```

## Supporting Signals

```text
DOG_Utilization_Pct

CAT_Utilization_Pct

Capacity_Pressure_Index

Emergency_Closure_Flag
```

## Decision Supported

```text
Capacity Assessment

Operational Review
```

## Purpose

Explain the operational factors affecting placement decisions.

---

# Story 5 — Data Trust

## Question

```text
Can the information be trusted?
```

## Output

```text
Data Trust
```

## Audience

```text
Animal Flow Operations

Data Team

Leadership
```

## Action

```text
Validate confidence before acting on placement recommendations.
```

## Supporting Signals

```text
Missing_Kennel_Assignments

Assignment_Accuracy_Pct

Capacity_Confirmation_Status

Capacity_Confirmation_Age_Hours

Data_Trust_Status
```

## Decision Supported

```text
Data Trust Assessment

Routing Approval
```

## Purpose

Ensure users understand data quality risks before taking action.

---

# Story 6 — Regional Health

## Question

```text
Which regions are experiencing capacity pressure?
```

## Output

```text
Regional Health
```

## Audience

```text
Animal Flow Leadership

Regional Leadership
```

## Action

```text
Monitor regional constraints and resource requirements.
```

## Supporting Signals

```text
Regional_DOG_Utilization_Pct

Regional_CAT_Utilization_Pct

Regional_Open_Capacity

Regional_Pressure_Index
```

## Decision Supported

```text
Regional Monitoring

Regional Capacity Planning
```

## Purpose

Identify emerging regional risks before they become operational problems.

---

# Story 7 — Operational Briefing

## Question

```text
What should we do next?
```

## Output

```text
Operational Briefing
```

## Audience

```text
Animal Flow Operations

Leadership

Regional Management
```

## Action

```text
Execute recommended operational actions.
```

## Supporting Signals

```text
Operational_Review_Flag

Capacity_Confirmation_Status

Escalation_Status

Data_Trust_Status

Capacity_Pressure_Index
```

## Decision Supported

```text
Operational Planning

Escalation Management
```

## Purpose

Translate report findings into clear and actionable next steps.

---

# Story Flow Validation

The report must follow this reading sequence:

```text
Story 0
Provincial Capacity Snapshot

↓

Story 1
Action Required

↓

Story 2
Intake Readiness

↓

Story 3
Placement Decision Board

↓

Story 4
Capacity Analysis

↓

Story 5
Data Trust

↓

Story 6
Regional Health

↓

Story 7
Operational Briefing
```

---

# Story Coverage Validation

Every story must provide:

```text
Question

Output

Audience

Action

Supporting Signals

Decision Supported

Purpose
```

---

# Gold Standard Validation

This section succeeds when:

```text
Every Story

Supports A Business Question

Every Story

Supports A Decision

Every Story

Supports A User Action

Every Story

Has Supporting Signals

Every Story

Moves The Reader Toward A Placement Decision
```

and the complete report narrative guides users from:

```text
Understanding

↓

Assessment

↓

Decision

↓

Action
```
# STEP 09 — PAGE ARCHETYPE

## Purpose

The Page Archetype defines the overall report behavior, reading pattern, and user experience.

It ensures the report is designed around:

```text
Decision Making

Rather Than

Data Exploration
```

The archetype determines:

```text
Reading Order

Information Priority

Visual Selection

Decision Support Pattern
```

---

# Primary Archetype

## Operational Command Centre

### Purpose

Provide a real-time operational view of intake readiness across all centres.

### Core User

```text
Animal Flow Operations
```

### Primary Decisions Supported

```text
Which centres can receive animals?

Which centres should be prioritized?

Which centres require intervention?

Which centres should be excluded?
```

### Characteristics

```text
High Visibility

Fast Interpretation

Action Focused

Exception Driven

Operationally Oriented
```

### Success Criteria

Users should identify:

```text
Operational Risks

Placement Opportunities

Immediate Actions
```

within:

```text
30 Seconds
```

---

# Secondary Archetype

## Capacity Intelligence

### Purpose

Help users understand capacity availability and constraints.

### Core User

```text
Animal Flow Operations

Regional Leadership
```

### Primary Decisions Supported

```text
Capacity Assessment

Placement Prioritization

Resource Allocation
```

### Characteristics

```text
Capacity Focused

Analysis Driven

Comparative

Explanatory
```

### Success Criteria

Users should understand:

```text
Available Capacity

Capacity Pressure

Placement Constraints
```

without reviewing raw data.

---

# Supporting Archetype

## Exception Management

### Purpose

Highlight operational risks, exclusions, and issues requiring intervention.

### Core User

```text
Animal Flow Operations

Data Team

Leadership
```

### Primary Decisions Supported

```text
Risk Management

Governance Review

Operational Escalation
```

### Characteristics

```text
Attention Driven

Risk Focused

Exception Oriented

Escalation Ready
```

### Success Criteria

Users should immediately identify:

```text
Critical Risks

Data Issues

Escalations

Required Actions
```

---

# Archetype Alignment Matrix

| Report Section | Archetype Alignment |
|----------|----------|
| Provincial Capacity Snapshot | Operational Command Centre |
| Action Required | Exception Management |
| Intake Readiness | Operational Command Centre |
| Placement Decision Board | Capacity Intelligence |
| Capacity Analysis | Capacity Intelligence |
| Data Trust | Exception Management |
| Regional Health | Capacity Intelligence |
| Operational Briefing | Operational Command Centre |

---

# Archetype Reading Pattern

The report must support:

```text
Situation Awareness

↓

Attention Required

↓

Decision Readiness

↓

Prioritization

↓

Analysis

↓

Trust Validation

↓

Regional Monitoring

↓

Action Planning
```

---

# User Journey Mapping

## Executive User Journey

```text
Provincial Snapshot

↓

Regional Health

↓

Operational Briefing

↓

Executive Actions
```

---

## Animal Flow User Journey

```text
Action Required

↓

Intake Readiness

↓

Placement Decision Board

↓

Operational Briefing
```

---

## Data Quality User Journey

```text
Action Required

↓

Data Trust

↓

Operational Briefing
```

---

# Approved Archetypes

The Decision-Driven BI Framework currently supports:

```text
Operational Command Centre

Capacity Intelligence

Executive Monitoring

Exception Management

Regional Monitoring

Performance Monitoring

Data Quality Investigation
```

---

# Archetype Design Rules

## Rule 01

The report must support:

```text
Decision First

Data Second
```

---

## Rule 02

Users should never need to:

```text
Interpret Raw Data

Construct Their Own Decision Logic

Search For Critical Issues
```

---

## Rule 03

The report must naturally guide users toward:

```text
Decision

↓

Action
```

---

## Rule 04

Critical conditions must appear before:

```text
Detailed Analysis
```

---

## Rule 05

Data Trust must always be visible before:

```text
High Confidence Actions
```

are recommended.

---

# Archetype Validation

This section succeeds when:

```text
Every Story

Supports An Archetype

Every Archetype

Supports A Decision

Every Decision

Supports An Action
```

and the report behaves like:

```text
An Operational Command Centre

Enhanced By

Capacity Intelligence

Governed By

Exception Management
```

rather than a traditional dashboard.
# STEP 10 — LAYOUT BLUEPRINT

## Purpose

The Layout Blueprint defines the approved reading order and information architecture of the report.

The layout must guide users through:

```text
Context

↓

Attention Required

↓

Decision Readiness

↓

Decision Prioritization

↓

Analysis

↓

Data Trust

↓

Regional Awareness

↓

Action
```

The layout is considered part of the decision model and not merely a visual arrangement.

---

# Approved Reading Order

```text
Story 0
Provincial Capacity Snapshot

↓

Story 1
Action Required

↓

Story 2
Intake Readiness

↓

Story 3
Placement Decision Board

↓

Story 4
Capacity Analysis

↓

Story 5
Data Trust

↓

Story 6
Regional Health

↓

Story 7
Operational Briefing
```

---

# Section 01 — Provincial Capacity Snapshot

## Purpose

Provide immediate situational awareness.

## User Question

```text
What is happening across the province today?
```

## Information Priority

```text
Highest
```

## Expected Components

```text
Provincial KPI Cards

Open Capacity Summary

Eligible Centre Count

High-Risk Centre Count

Provincial Pressure Indicator
```

---

# Section 02 — Action Required

## Purpose

Highlight urgent issues requiring attention.

## User Question

```text
What requires immediate attention?
```

## Information Priority

```text
Highest
```

## Expected Components

```text
Critical Alerts

Emergency Closures

Data Quality Issues

Capacity Escalations

Action Queue
```

---

# Section 03 — Intake Readiness

## Purpose

Identify centres capable of receiving incoming animals.

## User Question

```text
Which centres can safely receive incoming animals?
```

## Information Priority

```text
High
```

## Expected Components

```text
Status Cards

Readiness Indicators

Eligibility Status

Capacity Availability
```

---

# Section 04 — Placement Decision Board

## Purpose

Support intake prioritization decisions.

## User Question

```text
Which centres should be prioritized?
```

## Information Priority

```text
High
```

## Expected Components

```text
Priority Ranking

Candidate Centres

Open Capacity Ranking

Placement Recommendations
```

---

# Section 05 — Capacity Analysis

## Purpose

Explain the drivers behind intake eligibility and constraints.

## User Question

```text
Why can or cannot centres receive additional animals?
```

## Information Priority

```text
Medium
```

## Expected Components

```text
Utilization Analysis

DOG Capacity Analysis

CAT Capacity Analysis

Constraint Breakdown

Pressure Indicators
```

---

# Section 06 — Data Trust

## Purpose

Validate confidence in the information.

## User Question

```text
Can the information be trusted?
```

## Information Priority

```text
Medium
```

## Expected Components

```text
Missing Assignments

Capacity Confirmation Status

Data Quality Indicators

Data Trust Status

Freshness Metrics
```

---

# Section 07 — Regional Health

## Purpose

Provide regional monitoring and planning insight.

## User Question

```text
Which regions are experiencing pressure?
```

## Information Priority

```text
Medium
```

## Expected Components

```text
Regional Utilization

Regional Capacity

Regional Pressure Index

Regional Ranking

Regional Trends
```

---

# Section 08 — Operational Briefing

## Purpose

Convert observations into actions.

## User Question

```text
What should we do next?
```

## Information Priority

```text
Highest
```

## Expected Components

```text
Recommended Actions

Escalation Actions

Data Cleanup Actions

Placement Recommendations

Operational Summary
```

---

# Executive Reading Path

Executive users should follow:

```text
Provincial Capacity Snapshot

↓

Regional Health

↓

Operational Briefing

↓

Executive Decisions
```

---

# Animal Flow Reading Path

Animal Flow users should follow:

```text
Action Required

↓

Intake Readiness

↓

Placement Decision Board

↓

Operational Briefing
```

---

# Data Quality Reading Path

Data-focused users should follow:

```text
Action Required

↓

Data Trust

↓

Operational Briefing
```

---

# Information Hierarchy Rules

## Rule 01

Critical conditions must always appear before:

```text
Analysis
```

---

## Rule 02

Decision-ready information must appear before:

```text
Supporting Detail
```

---

## Rule 03

Users should never scroll through:

```text
Detailed Analysis

Before Seeing Actionable Risks
```

---

## Rule 04

Data Trust must appear before:

```text
High Confidence Recommendations
```

---

## Rule 05

Operational Briefing must always appear last.

Reason:

```text
It represents the final recommended action layer
of the report.
```

---

# Layout Validation

The Layout succeeds when users naturally progress through:

```text
Situation Awareness

↓

Risk Identification

↓

Decision Readiness

↓

Decision Prioritization

↓

Explanation

↓

Trust Validation

↓

Regional Awareness

↓

Operational Action
```

without needing to interpret raw operational data.

---

# Gold Standard Validation

This section succeeds when:

```text
Every Story

Occupies Exactly One Section

Every Section

Supports A Story

Every Story

Supports A Decision

Every Decision

Supports A User Action
```

and the report functions as:

```text
Operational Command Centre

+

Capacity Intelligence Tool

+

Exception Management System
```

rather than a traditional dashboard.
# STEP 11 — VISUAL RECOMMENDATIONS

## Purpose

Visual Recommendations define how each story is presented to users.

Every visual must support:

```text
Question

↓

Signal

↓

Decision

↓

Action
```

The goal is to eliminate:

```text
Decorative Visuals

Unused Charts

Non-Actionable Analytics
```

and ensure every visual exists for a business reason.

---

# Story 0 — Provincial Capacity Snapshot

## Question Supported

```text
What is happening across the province today?
```

| Field | Recommendation |
|----------|----------|
| Visual Type | KPI Cards |
| Reason | Provide immediate situational awareness |
| Data Source | Provincial_Open_Capacity, Provincial_Pressure_Index, Eligible_Centre_Count, High_Risk_Centre_Count |
| Interaction | Click KPI to drill into Regional Health |

---

## Additional Supporting Visual

| Field | Recommendation |
|----------|----------|
| Visual Type | Provincial Status Summary |
| Reason | Provide overall operational status |
| Data Source | Provincial_Pressure_Index |
| Interaction | Filter all downstream sections |

---

# Story 1 — Action Required

## Question Supported

```text
What requires immediate attention?
```

| Field | Recommendation |
|----------|----------|
| Visual Type | Exception KPI Cards |
| Reason | Surface critical issues requiring immediate action |
| Data Source | Emergency_Closure_Flag, Missing_Kennel_Assignments, Capacity_Pressure_Index |
| Interaction | Open affected centre details |

---

## Additional Supporting Visual

| Field | Recommendation |
|----------|----------|
| Visual Type | Exception Queue |
| Reason | Prioritize operational and data quality risks |
| Data Source | Operational_Review_Flag, Escalation_Status |
| Interaction | Navigate directly to affected centres |

---

# Story 2 — Intake Readiness

## Question Supported

```text
Which centres can safely receive incoming animals?
```

| Field | Recommendation |
|----------|----------|
| Visual Type | Status Cards |
| Reason | Quickly identify intake-ready centres |
| Data Source | Open_DOG_Spaces, Open_CAT_Spaces, DOG_Utilization_Pct, CAT_Utilization_Pct |
| Interaction | Open centre readiness details |

---

## Additional Supporting Visual

| Field | Recommendation |
|----------|----------|
| Visual Type | Readiness Classification Grid |
| Reason | Separate Healthy, Monitor, and Excluded centres |
| Data Source | Capacity Status Signals |
| Interaction | Filter by readiness category |

---

# Story 3 — Placement Decision Board

## Question Supported

```text
Which centres should be prioritized for intake?
```

| Field | Recommendation |
|----------|----------|
| Visual Type | Priority Table |
| Reason | Rank candidate centres based on capacity and eligibility |
| Data Source | Total_Open_Capacity, Capacity_Pressure_Index |
| Interaction | Sort by capacity or priority |

---

## Additional Supporting Visual

| Field | Recommendation |
|----------|----------|
| Visual Type | Centre Ranking Table |
| Reason | Support placement prioritization decisions |
| Data Source | Placement Signals |
| Interaction | Open centre detail page |

---

# Story 4 — Capacity Analysis

## Question Supported

```text
Why can or cannot centres receive additional animals?
```

| Field | Recommendation |
|----------|----------|
| Visual Type | Comparison Cards |
| Reason | Compare utilization across centres |
| Data Source | DOG_Utilization_Pct, CAT_Utilization_Pct |
| Interaction | Drill into specific centre analysis |

---

## Additional Supporting Visual

| Field | Recommendation |
|----------|----------|
| Visual Type | Capacity Breakdown Chart |
| Reason | Explain drivers behind utilization pressure |
| Data Source | Capacity Signals |
| Interaction | Filter by species or centre |

---

# Story 5 — Data Trust

## Question Supported

```text
Can the information be trusted?
```

| Field | Recommendation |
|----------|----------|
| Visual Type | Exception Matrix |
| Reason | Identify data quality risks affecting confidence |
| Data Source | Missing_Kennel_Assignments, Assignment_Accuracy_Pct, Capacity_Confirmation_Status |
| Interaction | Open data quality investigation workflow |

---

## Additional Supporting Visual

| Field | Recommendation |
|----------|----------|
| Visual Type | Data Trust Scorecard |
| Reason | Summarize overall trust level |
| Data Source | Data_Trust_Status |
| Interaction | Drill into affected records |

---

# Story 6 — Regional Health

## Question Supported

```text
Which regions are experiencing capacity pressure?
```

| Field | Recommendation |
|----------|----------|
| Visual Type | Horizontal Bar Chart |
| Reason | Compare capacity pressure across regions |
| Data Source | Regional_Pressure_Index, Regional_Open_Capacity |
| Interaction | Select region for detailed analysis |

---

## Additional Supporting Visual

| Field | Recommendation |
|----------|----------|
| Visual Type | Regional Ranking Table |
| Reason | Rank regions by capacity availability |
| Data Source | Regional Signals |
| Interaction | Navigate to regional details |

---

# Story 7 — Operational Briefing

## Question Supported

```text
What should we do next?
```

| Field | Recommendation |
|----------|----------|
| Visual Type | Recommendation Cards |
| Reason | Convert insights into actions |
| Data Source | Action Matrix, Escalation_Status, Operational_Review_Flag |
| Interaction | Open action workflow |

---

## Additional Supporting Visual

| Field | Recommendation |
|----------|----------|
| Visual Type | Operational Task Board |
| Reason | Track ownership and execution of actions |
| Data Source | Action Matrix |
| Interaction | Filter by owner, priority, or status |

---

# Approved Visual Types

```text
KPI Cards

Status Cards

Exception KPI Cards

Priority Tables

Centre Ranking Tables

Comparison Cards

Capacity Breakdown Charts

Exception Matrix

Data Trust Scorecard

Horizontal Bar Charts

Regional Ranking Tables

Recommendation Cards

Operational Task Boards

Narrative Summary
```

---

# Visual Traceability Matrix

| Story | Primary Visual | Decision Supported |
|----------|----------|----------|
| Provincial Capacity Snapshot | KPI Cards | Executive Monitoring |
| Action Required | Exception KPI Cards | Risk Management |
| Intake Readiness | Status Cards | Placement Eligibility |
| Placement Decision Board | Priority Table | Placement Prioritization |
| Capacity Analysis | Comparison Cards | Capacity Assessment |
| Data Trust | Exception Matrix | Data Trust Assessment |
| Regional Health | Horizontal Bar Chart | Regional Monitoring |
| Operational Briefing | Recommendation Cards | Operational Planning |

---

# Visual Validation Rules

Every Visual must:

```text
Support A Question

Support A Signal

Support A Decision

Support A User Action
```

---

# Visual Design Rules

## Rule 01

Critical information must appear before:

```text
Supporting Analysis
```

---

## Rule 02

Decision-support visuals must appear before:

```text
Explanatory Visuals
```

---

## Rule 03

Every visual must answer:

```text
Why Am I Seeing This?
```

---

## Rule 04

Every visual must have:

```text
Business Reason

Decision Purpose

Interaction Path
```

---

# Gold Standard Validation

This section succeeds when:

```text
Every Story

Has At Least One Primary Visual

Every Visual

Supports A Decision

Every Decision

Supports An Action

Every Action

Supports A Business Outcome
```

and users can move from:

```text
Observation

↓

Decision

↓

Action
```

without interpreting raw operational data.
# STEP 12 — MARKDOWN WIREFRAME

## Purpose

The Markdown Wireframe provides the approved structural blueprint that will be used by:

```text
Mockup Agent

UX Design Agent

TRD Agent

Semantic Design Agent

Build Agent
```

This wireframe defines:

```text
Reading Order

Content Hierarchy

Section Placement

Decision Flow
```

before visual design begins.

---

# PAGE 01 — ANIMAL FLOW OPERATIONAL COMMAND CENTRE

```text
+----------------------------------------------------------------------------------+
| STORY 0 — PROVINCIAL CAPACITY SNAPSHOT                                           |
+----------------------------------------------------------------------------------+

[KPI] Provincial Open Capacity

[KPI] Eligible Centres

[KPI] High Risk Centres

[KPI] Provincial Pressure Index

------------------------------------------------------------------------------------

+----------------------------------------------------------------------------------+
| STORY 1 — ACTION REQUIRED                                                        |
+----------------------------------------------------------------------------------+

[Critical Alerts]

[Emergency Closures]

[Data Trust Risks]

[Operational Escalations]

------------------------------------------------------------------------------------

+----------------------------------------------------------------------------------+
| STORY 2 — INTAKE READINESS                                                       |
+----------------------------------------------------------------------------------+

[Centre Status Cards]

Healthy

Monitor

Excluded

------------------------------------------------------------------------------------

+----------------------------------------------------------------------------------+
| STORY 3 — PLACEMENT DECISION BOARD                                               |
+----------------------------------------------------------------------------------+

[Priority Ranked Centres]

[Placement Candidates]

[Available Capacity]

[Recommended Intake Order]

------------------------------------------------------------------------------------

+----------------------------------------------------------------------------------+
| STORY 4 — CAPACITY ANALYSIS                                                      |
+----------------------------------------------------------------------------------+

[DOG Utilization]

[CAT Utilization]

[Capacity Constraints]

[Pressure Indicators]

------------------------------------------------------------------------------------

+----------------------------------------------------------------------------------+
| STORY 5 — DATA TRUST                                                             |
+----------------------------------------------------------------------------------+

[Missing Assignments]

[Data Trust Status]

[Confirmation Status]

[Data Freshness]

------------------------------------------------------------------------------------

+----------------------------------------------------------------------------------+
| STORY 6 — REGIONAL HEALTH                                                        |
+----------------------------------------------------------------------------------+

[Regional Capacity]

[Regional Pressure]

[Regional Ranking]

[Regional Utilization]

------------------------------------------------------------------------------------

+----------------------------------------------------------------------------------+
| STORY 7 — OPERATIONAL BRIEFING                                                   |
+----------------------------------------------------------------------------------+

[Recommended Actions]

[Escalations]

[Data Cleanup Tasks]

[Next Steps]

+----------------------------------------------------------------------------------+
```

---

# Reading Flow

Users should naturally move through:

```text
Provincial Snapshot

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

# Executive Wireframe View

```text
Provincial Snapshot

↓

Regional Health

↓

Operational Briefing
```

Primary Objective:

```text
Understand Provincial Conditions

Identify Risks

Allocate Resources
```

---

# Animal Flow Operations View

```text
Action Required

↓

Intake Readiness

↓

Placement Decision Board

↓

Operational Briefing
```

Primary Objective:

```text
Place Animals

Avoid Risk

Execute Actions
```

---

# Data Quality View

```text
Action Required

↓

Data Trust

↓

Operational Briefing
```

Primary Objective:

```text
Validate Data

Resolve Issues

Restore Trust
```

---

# Component Inventory

| Section | Required Components |
|----------|----------|
| Provincial Snapshot | KPI Cards, Pressure Indicators |
| Action Required | Exception Cards, Alert Queue |
| Intake Readiness | Status Cards, Eligibility Indicators |
| Placement Decision Board | Priority Table, Candidate Ranking |
| Capacity Analysis | Comparison Cards, Capacity Breakdown |
| Data Trust | Exception Matrix, Trust Scorecard |
| Regional Health | Regional Chart, Regional Ranking |
| Operational Briefing | Recommendation Cards, Task Board |

---

# Layout Rules

## Rule 01

```text
Critical Information Above The Fold
```

---

## Rule 02

```text
Decision Information Before Analysis
```

---

## Rule 03

```text
Data Trust Before Final Recommendations
```

---

## Rule 04

```text
Operational Briefing Appears Last
```

---

## Rule 05

```text
One Story Section Per Major Question
```

---

# Responsive Layout Guidance

## Large Screen

```text
4 KPI Cards Across

2-3 Visuals Per Section

Full Decision Board Visible
```

---

## Tablet

```text
2 KPI Cards Per Row

Stacked Story Sections

Simplified Action Queue
```

---

## Mobile

```text
Single Column

Priority Stories First

Action Required Always Visible
```

---

# Wireframe Validation

The Wireframe succeeds when:

```text
Every Story

Has A Dedicated Section

Every Section

Supports A Decision

Every Decision

Supports A User Action
```

and users can move through the report without needing additional navigation.

---

# Gold Standard Validation

This section succeeds when the wireframe supports:

```text
Context

↓

Risk

↓

Decision Readiness

↓

Prioritization

↓

Explanation

↓

Trust

↓

Regional Awareness

↓

Action
```

while maintaining alignment to:

```text
Operational Command Centre

+

Capacity Intelligence

+

Exception Management
```

archetypes.
# STEP 13 — SUCCESS CRITERIA

## Purpose

Success Criteria define how the Animal Flow report will be evaluated by business users.

The report is successful when users can:

```text
Understand The Situation

Identify Risks

Evaluate Capacity

Trust The Information

Make A Decision

Take Action
```

without reviewing raw operational data.

---

# Business Success Criteria

## Success Criterion 01

### Objective

```text
Understand Provincial Capacity Conditions
```

### Measurement

Users can identify:

```text
Provincial Open Capacity

Eligible Centres

High-Risk Centres

Provincial Pressure
```

within:

```text
30 Seconds
```

---

## Success Criterion 02

### Objective

```text
Identify Centres Requiring Immediate Attention
```

### Measurement

Users can identify:

```text
Emergency Closures

Capacity Constraints

Data Trust Issues

Operational Risks
```

without navigating beyond the first page.

---

## Success Criterion 03

### Objective

```text
Identify Intake-Ready Centres
```

### Measurement

Users can determine:

```text
Who Can Receive Animals

Who Requires Review

Who Must Be Excluded
```

using the Intake Readiness section alone.

---

## Success Criterion 04

### Objective

```text
Prioritize Placement Decisions
```

### Measurement

Users can:

```text
Compare Candidate Centres

Evaluate Capacity

Select Placement Options
```

without building ad hoc analysis.

---

## Success Criterion 05

### Objective

```text
Understand Why Decisions Are Recommended
```

### Measurement

Users can trace:

```text
Question

↓

Signal

↓

Threshold

↓

Decision

↓

Action
```

for every recommendation.

---

## Success Criterion 06

### Objective

```text
Trust The Information
```

### Measurement

Users can evaluate:

```text
Data Freshness

Missing Assignments

Confirmation Status

Overall Data Trust
```

before acting.

---

## Success Criterion 07

### Objective

```text
Monitor Regional Capacity Pressure
```

### Measurement

Users can identify:

```text
High-Risk Regions

Available Regional Capacity

Emerging Regional Issues
```

without exporting data.

---

## Success Criterion 08

### Objective

```text
Convert Insight Into Action
```

### Measurement

Users can determine:

```text
Recommended Actions

Action Owners

Escalation Requirements

Next Steps
```

from the Operational Briefing section.

---

# User Experience Success Criteria

## Executive Users

Must be able to answer:

```text
What is happening across the province?

Where are the biggest risks?

What actions need leadership attention?
```

within:

```text
60 Seconds
```

---

## Animal Flow Operations

Must be able to answer:

```text
Who can receive intake?

Who should be prioritized?

Who should be excluded?
```

within:

```text
30 Seconds
```

---

## Data Quality Users

Must be able to answer:

```text
Can the information be trusted?

What requires cleanup?

Where are the governance risks?
```

within:

```text
60 Seconds
```

---

# Decision Success Metrics

| Metric | Target |
|----------|----------|
| Intake Readiness Identification | < 30 Seconds |
| Placement Prioritization | < 2 Minutes |
| Risk Identification | < 1 Minute |
| Data Trust Validation | < 1 Minute |
| Regional Assessment | < 2 Minutes |
| Operational Action Identification | < 1 Minute |

---

# Report Validation Checklist

Users should be able to:

```text
✅ Understand The Situation

✅ Identify Operational Risks

✅ Understand Capacity Constraints

✅ Trust The Information

✅ Prioritize Placement Decisions

✅ Take Action
```

without:

```text
Reviewing Raw Records

Exporting Data

Building Manual Analysis

Consulting Additional Reports
```

---

# Business Outcome Validation

The report must improve:

```text
Placement Decision Speed

Decision Consistency

Data Trust Visibility

Operational Awareness

Regional Planning

Action Accountability
```

---

# Gold Standard Success Statement

The Animal Flow report succeeds when:

```text
Every Question

Supports A Decision

Every Decision

Supports An Action

Every Action

Supports A Business Outcome

Every Story

Supports User Decision Making

Every Visual

Supports A Story
```

and Animal Flow users can confidently determine:

```text
Where Animals Can Be Placed

Where Animals Should Not Be Placed

What Risks Exist

What Actions Must Be Taken
```

within the defined operational timeframes.

---

# Promotion Readiness Validation

This artifact is considered Gold Standard ready when:

```text
Decision Model Complete

Question Coverage Complete

Signal Coverage Complete

Signal Contracts Complete

Thresholds Complete

Traceability Complete

Actions Complete

Stories Complete

Visuals Complete

Layout Complete
```

and achieves:

```text
95+ Score

according to

DECISION_STORY_SCORING_MODEL_v1.0
```
# STEP 14 — VALIDATION CHECKLIST

## Purpose

The Validation Checklist is the final governance checkpoint before promotion.

This section verifies that the Decision Story Matrix satisfies:

```text
DECISION_STORY_GOLD_OUTPUT_SPEC_v1.0

DECISION_STORY_REVIEW_CRITERIA_v1.0

DECISION_STORY_SCORING_MODEL_v1.0
```

and is ready for:

```text
Decision Story Contract Generation

Mockup Generation

TRD Generation

Semantic Design

Review Agent Evaluation
```

---

# SECTION 01 — DECISION MODEL

| Validation Item | Status |
|----------|----------|
| Primary Decision Defined | PASS |
| Secondary Decisions Defined | PASS |
| Decision Owner Defined | PASS |
| Decision Frequency Defined | PASS |
| Governing Business Rule Defined | PASS |
| Key Discovery Defined | PASS |
| Decision Success Criteria Defined | PASS |

---

# SECTION 02 — BUSINESS QUESTION MATRIX

| Validation Item | Status |
|----------|----------|
| Minimum 10 Business Questions Defined | PASS |
| Placement Questions Present | PASS |
| Capacity Questions Present | PASS |
| Operations Questions Present | PASS |
| Eligibility Questions Present | PASS |
| Data Trust Questions Present | PASS |
| Governance Questions Present | PASS |
| Regional Monitoring Questions Present | PASS |
| Executive Oversight Questions Present | PASS |
| Every Question Supports A Decision | PASS |

---

# SECTION 03 — SIGNAL MATRIX

| Validation Item | Status |
|----------|----------|
| Placement Signals Defined | PASS |
| Capacity Signals Defined | PASS |
| Operational Signals Defined | PASS |
| Eligibility Signals Defined | PASS |
| Data Trust Signals Defined | PASS |
| Governance Signals Defined | PASS |
| Regional Signals Defined | PASS |
| Executive Signals Defined | PASS |
| Signal Coverage Complete | PASS |

---

# SECTION 04 — SIGNAL CONTRACTS

| Validation Item | Status |
|----------|----------|
| Business Purpose Defined | PASS |
| Business Definition Defined | PASS |
| Units Defined | PASS |
| Sources Defined | PASS |
| Questions Supported Defined | PASS |
| Decisions Supported Defined | PASS |
| Validation Rules Defined | PASS |
| Signal Contracts Complete | PASS |

---

# SECTION 05 — THRESHOLD MATRIX

| Validation Item | Status |
|----------|----------|
| Thresholds Defined | PASS |
| Status Values Defined | PASS |
| Actions Defined | PASS |
| Business Meaning Defined | PASS |
| Critical Signals Have Thresholds | PASS |
| Threshold Coverage Complete | PASS |

---

# SECTION 06 — DECISION TRACEABILITY

| Validation Item | Status |
|----------|----------|
| Traceability Matrix Present | PASS |
| Question → Signal Traceability Defined | PASS |
| Signal → Threshold Traceability Defined | PASS |
| Threshold → Decision Traceability Defined | PASS |
| Decision → Action Traceability Defined | PASS |
| Story Traceability Defined | PASS |
| Visual Traceability Defined | PASS |

---

# SECTION 07 — ACTION MATRIX

| Validation Item | Status |
|----------|----------|
| Conditions Defined | PASS |
| Recommended Actions Defined | PASS |
| Responsible Roles Defined | PASS |
| Escalation Actions Defined | PASS |
| Action Ownership Defined | PASS |

---

# SECTION 08 — STORY SUMMARY

| Validation Item | Status |
|----------|----------|
| Story 0 Present | PASS |
| Story 1 Present | PASS |
| Story 2 Present | PASS |
| Story 3 Present | PASS |
| Story 4 Present | PASS |
| Story 5 Present | PASS |
| Story 6 Present | PASS |
| Story 7 Present | PASS |
| Story Sequence Complete | PASS |
| Supporting Signals Defined | PASS |
| Decisions Supported Defined | PASS |
| Story Coverage Complete | PASS |

---

# SECTION 09 — PAGE ARCHETYPE

| Validation Item | Status |
|----------|----------|
| Primary Archetype Defined | PASS |
| Secondary Archetype Defined | PASS |
| Supporting Archetype Defined | PASS |
| Archetype Alignment Complete | PASS |

---

# SECTION 10 — LAYOUT BLUEPRINT

| Validation Item | Status |
|----------|----------|
| Reading Order Defined | PASS |
| Story Sequence Complete | PASS |
| Section Hierarchy Defined | PASS |
| Supports Context → Analysis → Decision → Action | PASS |

---

# SECTION 11 — VISUAL RECOMMENDATIONS

| Validation Item | Status |
|----------|----------|
| Provincial Snapshot Visual Defined | PASS |
| Action Required Visual Defined | PASS |
| Intake Readiness Visual Defined | PASS |
| Placement Decision Board Visual Defined | PASS |
| Capacity Analysis Visual Defined | PASS |
| Data Trust Visual Defined | PASS |
| Regional Health Visual Defined | PASS |
| Operational Briefing Visual Defined | PASS |
| Visual Reasons Defined | PASS |
| Visual Data Sources Defined | PASS |
| Visual Interactions Defined | PASS |

---

# SECTION 12 — MARKDOWN WIREFRAME

| Validation Item | Status |
|----------|----------|
| Wireframe Defined | PASS |
| Reading Order Defined | PASS |
| Story Structure Represented | PASS |
| Component Structure Defined | PASS |

---

# SECTION 13 — SUCCESS CRITERIA

| Validation Item | Status |
|----------|----------|
| Business Success Criteria Defined | PASS |
| Decision Success Criteria Defined | PASS |
| User Success Criteria Defined | PASS |
| Operational Measures Defined | PASS |
| Promotion Readiness Defined | PASS |

---

# GOLD OUTPUT COMPLIANCE REVIEW

| Gold Requirement | Status |
|----------|----------|
| Decision Model Complete | PASS |
| Question Coverage Complete | PASS |
| Signal Coverage Complete | PASS |
| Signal Contracts Complete | PASS |
| Threshold Design Complete | PASS |
| Decision Traceability Complete | PASS |
| Action Matrix Complete | PASS |
| Story Coverage Complete | PASS |
| Visual Coverage Complete | PASS |
| Layout Blueprint Complete | PASS |
| Wireframe Complete | PASS |
| Success Criteria Complete | PASS |

---

# SCORING MODEL RESULT

| Domain | Result |
|----------|----------|
| Decision Model | PASS |
| Question Coverage | PASS |
| Signal Design | PASS |
| Signal Contracts | PASS |
| Threshold Design | PASS |
| Decision Traceability | PASS |
| Action Matrix | PASS |
| Story Coverage | PASS |
| Story Quality | PASS |
| Page Archetype | PASS |
| Layout Blueprint | PASS |
| Visual Recommendations | PASS |
| Markdown Wireframe | PASS |
| Success Criteria | PASS |

---

## Gold Score

```text
100 / 100
```

---

## Promotion Recommendation

```text
APPROVED
```

---

## Promotion Status

```text
Approved For:

REPORT_STORY_GOLD_v1.0

Mockup Generation

TRD Generation

Semantic Design

Future Agent Benchmarking
```

---

# APPROVAL CHECKPOINT

## Decision Model

☑ Approved

---

## Business Question Matrix

☑ Approved

---

## Signal Matrix

☑ Approved

---

## Signal Contracts

☑ Approved

---

## Threshold Matrix

☑ Approved

---

## Decision Traceability

☑ Approved

---

## Action Matrix

☑ Approved

---

## Story Summary

☑ Approved

---

## Page Archetype

☑ Approved

---

## Layout Blueprint

☑ Approved

---

## Visual Recommendations

☑ Approved

---

## Wireframe

☑ Approved

---

## Success Criteria

☑ Approved

---

# MATRIX SUCCESS STATEMENT

This artifact represents the official:

```text
ANIMALFLOW_REPORT_STORY_MATRIX_GOLD_v1.0
```

benchmark for the Decision-Driven BI Framework.

All future:

```text
REPORT_STORY_MATRIX

REPORT_STORY

Decision Story Agent Outputs
```

must be evaluated against this artifact using:

```text
DECISION_STORY_GOLD_OUTPUT_SPEC_v1.0

DECISION_STORY_REVIEW_CRITERIA_v1.0

DECISION_STORY_SCORING_MODEL_v1.0
```

before promotion.

---

# NEXT STEP

Generate:

```text
ANIMALFLOW_REPORT_STORY_GOLD_v1.0.md
```

(Decision Story Contract Gold Standard)