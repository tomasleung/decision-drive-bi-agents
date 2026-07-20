# ANIMALFLOW_REPORT_STORY_GOLD_v1.0

## Animal Flow — Live Capacity Reporting

### Decision Story Contract (DSC)

---

# DOCUMENT METADATA

Document Type

Decision Story Contract

Version

1.0

Capability

Animal Flow — Live Capacity Reporting

Owner

Animal Flow Team

Purpose

Convert the approved Decision Story Matrix into the authoritative business design contract used by:

- Mockup Agent
- TRD Agent
- Semantic Design Agent
- Build Agent

Audience

- Product Owner
- Business Owner
- Animal Flow Team
- Report Designer
- BI Developer
- Data Architect
- Solution Architect

Related Governance

```text
DECISION_STORY_GOLD_OUTPUT_SPEC_v1.0

DECISION_STORY_REVIEW_CRITERIA_v1.0

DECISION_STORY_SCORING_MODEL_v1.0
```

Source Artifacts

```text
ANIMALFLOW_REPORT_STORY_MATRIX_GOLD_v1.0

INPUT_BRD_AnimalFlow_LiveCapacity_v2.0
```

---

# SECTION 01 — DECISION MODEL

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

---

## Governing Business Rule

Animal placement decisions must not rely solely on:

```text
Open Spaces
```

The governing intake decision is:

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

Capacity Confirmation Status

+

Data Trust

=

Placement Readiness
```

---

## Key Discovery

A centre may appear available while simultaneously being unsuitable for intake because:

```text
Capacity Threshold Reached

OR

Emergency Closure Active

OR

Data Cannot Be Trusted

OR

Capacity Confirmation Is Stale
```

Open capacity alone is not sufficient.

---

## Decision Success Criteria

Users must answer:

```text
Which centres can safely receive incoming animals?
```

within:

```text
30 Seconds
```

without reviewing operational records.

---

## Decision Outcomes

### Outcome 01

Identify candidate intake centres.

### Outcome 02

Identify excluded centres.

### Outcome 03

Identify centres requiring review.

### Outcome 04

Identify operational risks.

### Outcome 05

Prioritize placement decisions.

### Outcome 06

Monitor regional pressure.

---

# SECTION 02 — BUSINESS QUESTION MATRIX

## Placement Questions

| Business Question | Priority |
|----------|----------|
| Which centres currently have available DOG capacity? | Critical |
| Which centres currently have available CAT capacity? | Critical |
| Which centres should be prioritized for intake? | Critical |
| Which centres should be avoided for intake? | High |
| Which centres can safely receive incoming animals? | Critical |

---

## Capacity Questions

| Business Question | Priority |
|----------|----------|
| Which centres are approaching critical utilization? | High |
| Which centres have reached maximum utilization? | High |
| Which centres have the greatest available intake capacity? | High |
| Which centres have limited operational headroom? | High |

---

## Operational Questions

| Business Question | Priority |
|----------|----------|
| Which centres require operational intervention? | High |
| Which centres require immediate follow-up? | High |
| Which centres require manual review before placement? | High |

---

## Eligibility Questions

| Business Question | Priority |
|----------|----------|
| Which centres have emergency closures? | High |
| Which centres should be excluded immediately? | High |
| Which centres fail eligibility rules? | High |

---

## Data Trust Questions

| Business Question | Priority |
|----------|----------|
| Which centres have missing kennel assignments? | High |
| Which centres have stale capacity updates? | High |
| Which centres have not confirmed capacity status? | High |
| Which centres have unreliable operational data? | High |
| Can the information be trusted? | Critical |

---

## Governance Questions

| Business Question | Priority |
|----------|----------|
| Which centres require confirmation before placement? | High |
| Which centres violate freshness requirements? | High |
| Which centres require escalation? | High |

---

## Regional Questions

| Business Question | Priority |
|----------|----------|
| Which regions are experiencing pressure? | Medium |
| Which regions have the highest utilization? | Medium |
| Which regions have the greatest available capacity? | Medium |
| Which regions require intervention? | Medium |

---

## Executive Questions

| Business Question | Priority |
|----------|----------|
| What is happening across the province today? | Medium |
| Where are the biggest operational risks? | Medium |
| What actions should leadership prioritize? | Medium |

---

# SECTION 03 — BUSINESS LOGIC MODEL

## Placement Readiness Logic

Placement Readiness is determined through:

```text
Capacity Availability

+

Eligibility

+

Data Trust

+

Operational Readiness
```

---

## Eligibility Logic

A centre is eligible when:

```text
DOG Capacity Available

AND

CAT Capacity Available

AND

Emergency Closure Inactive

AND

Data Trust Acceptable

AND

Capacity Confirmation Current
```

---

## Capacity Logic

Capacity readiness is determined through:

```text
Open DOG Spaces

Open CAT Spaces

DOG Utilization %

CAT Utilization %

Capacity Pressure Index
```

---

## Data Trust Logic

Trust is determined through:

```text
Missing Assignments

Assignment Accuracy %

Capacity Confirmation

Capacity Confirmation Age

Data Freshness
```

---

## Regional Monitoring Logic

Regional pressure is evaluated through:

```text
Regional Utilization

Regional Open Capacity

Regional Pressure Index
```

---

## Example Placement Logic

```text
IF Emergency_Closure_Flag = TRUE

THEN Exclude Centre

ELSE IF DOG_Utilization_Pct >= 100

THEN Exclude Centre

ELSE IF CAT_Utilization_Pct >= 100

THEN Exclude Centre

ELSE IF Data_Trust_Status = Not Trusted

THEN Review Required

ELSE Candidate Centre
```

---

# SECTION 04 — SIGNAL DEFINITIONS

## Open_DOG_Spaces

| Attribute | Definition |
|----------|----------|
| Purpose | Determine available DOG capacity |
| Definition | Number of DOG spaces immediately available |
| Unit | Spaces |
| Source | Shelter System |
| Validation | Must be >= 0 |
| Example | 12 |

---

## Open_CAT_Spaces

| Attribute | Definition |
|----------|----------|
| Purpose | Determine available CAT capacity |
| Definition | Number of CAT spaces immediately available |
| Unit | Spaces |
| Source | Shelter System |
| Validation | Must be >= 0 |
| Example | 8 |

---

## DOG_Utilization_Pct

| Attribute | Definition |
|----------|----------|
| Purpose | Measure DOG capacity pressure |
| Definition | Percentage of occupied DOG spaces |
| Unit | Percent |
| Source | Shelter System |
| Validation | 0%–200% |
| Example | 84% |

---

## CAT_Utilization_Pct

| Attribute | Definition |
|----------|----------|
| Purpose | Measure CAT capacity pressure |
| Definition | Percentage of occupied CAT spaces |
| Unit | Percent |
| Source | Shelter System |
| Validation | 0%–200% |
| Example | 72% |

---

## Emergency_Closure_Flag

| Attribute | Definition |
|----------|----------|
| Purpose | Determine eligibility |
| Definition | Indicates active emergency closure |
| Unit | Boolean |
| Source | Operations Feed |
| Validation | TRUE/FALSE |
| Example | TRUE |

---

## Missing_Kennel_Assignments

| Attribute | Definition |
|----------|----------|
| Purpose | Measure data quality risk |
| Definition | Number of animals without kennel assignment |
| Unit | Count |
| Source | Intake System |
| Validation | Non-negative integer |
| Example | 4 |

---

## Assignment_Accuracy_Pct

| Attribute | Definition |
|----------|----------|
| Purpose | Measure assignment integrity |
| Definition | Percentage of valid assignments |
| Unit | Percent |
| Source | Intake System |
| Validation | 0%–100% |
| Example | 98% |

---

## Capacity_Confirmation_Age_Hours

| Attribute | Definition |
|----------|----------|
| Purpose | Measure freshness of confirmation |
| Definition | Hours since last confirmed capacity status |
| Unit | Hours |
| Source | Capacity Confirmation Feed |
| Validation | Non-negative |
| Example | 6 |

---
# SECTION 05 — THRESHOLD MATRIX

## Purpose

Thresholds translate business signals into decision outcomes.

Each threshold must answer:

```text
What Happened?

↓

Why It Matters?

↓

What Action Should Be Taken?
```

---

# DOG_Utilization_Pct

## Business Question

```text
Can this centre safely receive additional DOG intake?
```

## Supported Decision

```text
DOG Intake Eligibility
```

| Threshold | Status | Action | Business Meaning |
|----------|----------|----------|----------|
| < 80% | Healthy | Candidate Centre | Centre has sufficient DOG intake capacity available. |
| 80% - 99% | Monitor | Review Before Routing | Centre remains eligible but is approaching capacity pressure. |
| >= 100% | Full | Do Not Intake | Centre has reached or exceeded DOG intake capacity. |

---

# CAT_Utilization_Pct

## Business Question

```text
Can this centre safely receive additional CAT intake?
```

## Supported Decision

```text
CAT Intake Eligibility
```

| Threshold | Status | Action | Business Meaning |
|----------|----------|----------|----------|
| < 80% | Healthy | Candidate Centre | Centre has sufficient CAT intake capacity available. |
| 80% - 99% | Monitor | Review Before Routing | Centre is approaching CAT capacity pressure. |
| >= 100% | Full | Do Not Intake | Centre has reached or exceeded CAT intake capacity. |

---

# Total_Open_Capacity

## Business Question

```text
Which centres should be prioritized?
```

## Supported Decision

```text
Placement Prioritization
```

| Threshold | Status | Action | Business Meaning |
|----------|----------|----------|----------|
| > 20 | High Capacity | Prioritize | Strong candidate for intake placement. |
| 10 - 20 | Moderate Capacity | Consider | Suitable for placement activity. |
| 1 - 9 | Limited Capacity | Use With Caution | Capacity available but constrained. |
| 0 | No Capacity | Exclude | No intake capacity available. |

---

# Capacity_Pressure_Index

## Business Question

```text
Which centres require operational review?
```

## Supported Decision

```text
Capacity Risk Assessment
```

| Threshold | Status | Action | Business Meaning |
|----------|----------|----------|----------|
| Low | Healthy | Continue Operations | Capacity pressure is minimal. |
| Moderate | Monitor | Daily Review | Pressure beginning to increase. |
| High | Risk | Operational Review | Capacity constraints impacting operations. |
| Critical | Escalate | Immediate Intervention | Immediate leadership attention required. |

---

# Emergency_Closure_Flag

## Business Question

```text
Is the centre eligible for intake?
```

## Supported Decision

```text
Intake Eligibility
```

| Threshold | Status | Action | Business Meaning |
|----------|----------|----------|----------|
| FALSE | Eligible | Continue Evaluation | Centre remains eligible for intake review. |
| TRUE | Excluded | Exclude Centre | Centre must not receive intake while closure remains active. |

---

# Missing_Kennel_Assignments

## Business Question

```text
Can operational data be trusted?
```

## Supported Decision

```text
Data Trust Assessment
```

| Threshold | Status | Action | Business Meaning |
|----------|----------|----------|----------|
| 0 | Healthy | No Action | Data quality acceptable. |
| 1 - 3 | Warning | Review | Minor data quality issues present. |
| > 3 | Critical | Data Cleanup Required | Data quality risk impacts decision confidence. |

---

# Assignment_Accuracy_Pct

## Business Question

```text
Can placement decisions rely on assignment data?
```

## Supported Decision

```text
Data Trust Assessment
```

| Threshold | Status | Action | Business Meaning |
|----------|----------|----------|----------|
| >= 99% | Trusted | Use Normally | Assignment quality highly reliable. |
| 95% - 98% | Review | Validate | Minor quality concerns require validation. |
| < 95% | High Risk | Escalate | Data quality risk may impact decisions. |

---

# Capacity_Confirmation_Age_Hours

## Business Question

```text
Can capacity information be trusted?
```

## Supported Decision

```text
Governance Review
```

| Threshold | Status | Action | Business Meaning |
|----------|----------|----------|----------|
| < 12 Hours | Current | Use Normally | Capacity confirmation remains reliable. |
| 12 - 24 Hours | Aging | Validate | Confirmation becoming stale. |
| > 24 Hours | Stale | Contact Centre | Confirmation required before placement decisions. |

---

# Data_Trust_Status

## Business Question

```text
Should automated placement decisions proceed?
```

## Supported Decision

```text
Routing Approval
```

| Threshold | Status | Action | Business Meaning |
|----------|----------|----------|----------|
| Trusted | Proceed | Continue Routing | Automated routing approved. |
| Review Required | Validate | Manual Review | Additional confirmation needed. |
| Not Trusted | Block | Stop Automated Routing | Automated decisions must not proceed. |

---

# Regional_Pressure_Index

## Business Question

```text
Which regions require operational intervention?
```

## Supported Decision

```text
Regional Capacity Planning
```

| Threshold | Status | Action | Business Meaning |
|----------|----------|----------|----------|
| Low | Healthy | Monitor | Region operating normally. |
| Moderate | Watch | Monitor Closely | Capacity pressure beginning to emerge. |
| High | Risk | Allocate Resources | Resource balancing required. |
| Critical | Escalate | Leadership Intervention | Immediate regional intervention required. |

---

# Provincial_Pressure_Index

## Business Question

```text
What is happening across the province today?
```

## Supported Decision

```text
Executive Monitoring
```

| Threshold | Status | Action | Business Meaning |
|----------|----------|----------|----------|
| Low | Healthy | Continue Operations | Provincial capacity stable. |
| Moderate | Monitor | Increase Observation | Conditions require monitoring. |
| High | Alert | Prepare Response | Province-wide pressure emerging. |
| Critical | Escalate | Provincial Action Plan | Immediate leadership response required. |

---

# SECTION 06 — DECISION TRACEABILITY

## Purpose

Traceability guarantees that every decision recommendation can be explained.

Required flow:

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

---

## Placement Traceability

| Business Question | Signal | Threshold | Decision | Action |
|----------|----------|----------|----------|----------|
| Which centres currently have available DOG capacity? | Open_DOG_Spaces | > 0 | Placement Eligibility | Candidate Centre |
| Which centres currently have available CAT capacity? | Open_CAT_Spaces | > 0 | Placement Eligibility | Candidate Centre |
| Which centres can safely receive incoming animals? | DOG_Utilization_Pct | < 80% | Intake Eligibility | Candidate Centre |
| Which centres can safely receive incoming animals? | CAT_Utilization_Pct | < 80% | Intake Eligibility | Candidate Centre |
| Which centres should be prioritized for intake? | Total_Open_Capacity | > 20 | Placement Prioritization | Prioritize Centre |
| Which centres should be avoided? | DOG_Utilization_Pct | >= 100% | Placement Exclusion | Do Not Intake |
| Which centres should be avoided? | CAT_Utilization_Pct | >= 100% | Placement Exclusion | Do Not Intake |

---

## Eligibility Traceability

| Business Question | Signal | Threshold | Decision | Action |
|----------|----------|----------|----------|----------|
| Which centres have emergency closures? | Emergency_Closure_Flag | TRUE | Centre Eligibility | Exclude Centre |
| Which centres should be excluded immediately? | Emergency_Closure_Flag | TRUE | Intake Exclusion | Exclude Centre |
| Which centres fail eligibility rules? | Intake_Block_Flag | Active | Eligibility Review | Do Not Intake |

---

## Data Trust Traceability

| Business Question | Signal | Threshold | Decision | Action |
|----------|----------|----------|----------|----------|
| Which centres have missing kennel assignments? | Missing_Kennel_Assignments | > 3 | Data Trust Assessment | Data Cleanup Required |
| Which centres have stale updates? | Capacity_Confirmation_Age_Hours | > 24 | Data Freshness Review | Contact Centre |
| Which centres have unreliable data? | Data_Trust_Status | Not Trusted | Routing Approval | Block Automated Routing |
| Can the information be trusted? | Assignment_Accuracy_Pct | < 95% | Data Trust Review | Escalate Review |

---

## Regional Traceability

| Business Question | Signal | Threshold | Decision | Action |
|----------|----------|----------|----------|----------|
| Which regions are experiencing pressure? | Regional_Pressure_Index | High | Regional Capacity Review | Allocate Resources |
| Which regions require intervention? | Regional_Pressure_Index | Critical | Regional Escalation | Leadership Review |

---

# SECTION 07 — ACTION MATRIX

## Purpose

Convert decisions into operational responses.

Every decision must have a defined owner.

---

# Placement Actions

| Condition | Recommended Action | Responsible Role | Priority |
|----------|----------|----------|----------|
| Open_DOG_Spaces > 0 AND DOG_Utilization_Pct < 80% | Designate Candidate Centre | Animal Flow Operations | High |
| Open_CAT_Spaces > 0 AND CAT_Utilization_Pct < 80% | Designate Candidate Centre | Animal Flow Operations | High |
| Total_Open_Capacity > 20 | Prioritize Intake Routing | Animal Flow Operations | High |
| Total_Open_Capacity 10 - 20 | Consider For Placement | Animal Flow Operations | Medium |
| Total_Open_Capacity < 10 | Use With Caution | Animal Flow Operations | Medium |
| Total_Open_Capacity = 0 | Remove From Candidate List | Animal Flow Operations | Critical |

---

# Capacity Actions

| Condition | Recommended Action | Responsible Role | Priority |
|----------|----------|----------|----------|
| DOG_Utilization_Pct 80% - 99% | Review Before Routing | Animal Flow Operations | High |
| DOG_Utilization_Pct >= 100% | Do Not Intake DOGs | Animal Flow Operations | Critical |
| CAT_Utilization_Pct 80% - 99% | Review Before Routing | Animal Flow Operations | High |
| CAT_Utilization_Pct >= 100% | Do Not Intake CATs | Animal Flow Operations | Critical |
| Capacity_Pressure_Index = High | Operational Review | Animal Flow Leadership | High |
| Capacity_Pressure_Index = Critical | Immediate Escalation | Animal Flow Leadership | Critical |

---

# Eligibility Actions

| Condition | Recommended Action | Responsible Role | Priority |
|----------|----------|----------|----------|
| Emergency_Closure_Flag = TRUE | Exclude Centre Immediately | Animal Flow Operations | Critical |
| Intake_Block_Flag = Active | Remove From Routing Queue | Animal Flow Operations | Critical |

---

# Data Trust Actions

| Condition | Recommended Action | Responsible Role | Priority |
|----------|----------|----------|----------|
| Missing_Kennel_Assignments > 3 | Assign Data Cleanup | Data Team | Critical |
| Assignment_Accuracy_Pct < 95% | Investigate Data Quality | Data Team | High |
| Data_Trust_Status = Review Required | Manual Validation | Animal Flow Operations | High |
| Data_Trust_Status = Not Trusted | Block Automated Routing | Animal Flow Operations | Critical |

---

# Governance Actions

| Condition | Recommended Action | Responsible Role | Priority |
|----------|----------|----------|----------|
| Capacity_Confirmation_Age_Hours > 24 | Contact Centre | Animal Flow Operations | Critical |
| Data_Freshness_Status = Stale | Governance Review | Governance Team | High |
| Escalation_Status = Escalated | Assign Escalation Owner | Governance Team | Critical |

---

# Regional Actions

| Condition | Recommended Action | Responsible Role | Priority |
|----------|----------|----------|----------|
| Regional_Pressure_Index = High | Allocate Resources | Animal Flow Leadership | High |
| Regional_Pressure_Index = Critical | Activate Intervention Plan | Animal Flow Leadership | Critical |

---

# Executive Actions

| Condition | Recommended Action | Responsible Role | Priority |
|----------|----------|----------|----------|
| Provincial_Pressure_Index = High | Prepare Provincial Response Plan | Executive Leadership | High |
| Provincial_Pressure_Index = Critical | Initiate Provincial Action Plan | Executive Leadership | Critical |
| High_Risk_Centre_Count > 0 | Executive Risk Review | Executive Leadership | High |

---

## Action Ownership Matrix

| Action Area | Primary Owner | Secondary Owner |
|----------|----------|----------|
| Placement Decisions | Animal Flow Operations | Centre Teams |
| Capacity Monitoring | Animal Flow Operations | Leadership |
| Data Quality | Data Team | Animal Flow Operations |
| Governance Review | Governance Team | Leadership |
| Regional Planning | Animal Flow Leadership | Regional Teams |
| Executive Oversight | Executive Leadership | Animal Flow Leadership |

---

## Action Validation

Every action must:

```text
Support A Decision

Have A Responsible Owner

Produce A Business Outcome

Be Operationally Actionable
```

---
# SECTION 08 — NARRATIVE STORY

## Purpose

The Narrative Story transforms business requirements into a decision-driven report experience.

The report must tell a complete decision story:

```text
Situation

↓

Risk

↓

Readiness

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

The narrative is the primary contract consumed by:

```text
Mockup Agent

TRD Agent

Semantic Design Agent

Build Agent
```

---

# STORY 0 — PROVINCIAL CAPACITY SNAPSHOT

## Business Question

```text
What is happening across the province today?
```

## Business Objective

Provide immediate situational awareness.

---

## Audience

```text
Animal Flow

Leadership

Executive Stakeholders
```

---

## Output

```text
Provincial Capacity Snapshot
```

---

## Supporting Signals

```text
Provincial_Open_Capacity

Provincial_Pressure_Index

Eligible_Centre_Count

High_Risk_Centre_Count
```

---

## Decision Supported

```text
Executive Monitoring

Provincial Oversight
```

---

## User Action

```text
Understand overall provincial conditions.
```

---

## Narrative

This section provides a province-wide view of capacity, pressure, risk, and placement readiness.

Users should immediately understand:

```text
Current Operating Conditions

Overall Intake Readiness

Emerging Provincial Risks
```

without reviewing detailed centre-level information.

---

# STORY 1 — ACTION REQUIRED

## Business Question

```text
What requires immediate attention?
```

## Business Objective

Surface urgent operational and governance issues.

---

## Audience

```text
Animal Flow Operations

Leadership
```

---

## Output

```text
Action Required
```

---

## Supporting Signals

```text
Emergency_Closure_Flag

Missing_Kennel_Assignments

Capacity_Pressure_Index

Escalation_Status
```

---

## Decision Supported

```text
Risk Management

Operational Escalation
```

---

## User Action

```text
Identify and address critical issues.
```

---

## Narrative

Users must immediately see:

```text
Emergency Closures

Capacity Exclusions

Data Quality Risks

Escalations
```

before reviewing intake candidates.

Critical risks should never be hidden beneath detailed analysis.

---

# STORY 2 — INTAKE READINESS

## Business Question

```text
Which centres can safely receive incoming animals?
```

## Business Objective

Identify intake-ready centres.

---

## Audience

```text
Animal Flow Operations
```

---

## Output

```text
Intake Readiness
```

---

## Supporting Signals

```text
Open_DOG_Spaces

Open_CAT_Spaces

DOG_Utilization_Pct

CAT_Utilization_Pct

Emergency_Closure_Flag
```

---

## Decision Supported

```text
Placement Eligibility
```

---

## User Action

```text
Select intake-ready centres.
```

---

## Narrative

This section answers the primary business question.

Users must immediately classify centres as:

```text
Eligible

Monitor

Excluded
```

and understand who can safely receive intake.

---

# STORY 3 — PLACEMENT DECISION BOARD

## Business Question

```text
Which centres should be prioritized for intake?
```

## Business Objective

Support placement ranking.

---

## Audience

```text
Animal Flow Operations
```

---

## Output

```text
Placement Decision Board
```

---

## Supporting Signals

```text
Total_Open_Capacity

Available_DOG_Capacity

Available_CAT_Capacity

Capacity_Pressure_Index
```

---

## Decision Supported

```text
Placement Prioritization
```

---

## User Action

```text
Rank and compare placement options.
```

---

## Narrative

Once eligible centres are identified, users must determine:

```text
Best Option

Second Best Option

Fallback Option
```

based on available capacity and operational readiness.

---

# STORY 4 — CAPACITY ANALYSIS

## Business Question

```text
Why can or cannot centres receive additional animals?
```

## Business Objective

Explain placement constraints.

---

## Audience

```text
Animal Flow Operations

Centre Management
```

---

## Output

```text
Capacity Analysis
```

---

## Supporting Signals

```text
DOG_Utilization_Pct

CAT_Utilization_Pct

Capacity_Pressure_Index
```

---

## Decision Supported

```text
Capacity Assessment

Operational Review
```

---

## User Action

```text
Understand the causes of capacity pressure.
```

---

## Narrative

This section provides explanatory context.

Users should understand:

```text
Why Centres Are Full

Why Centres Are At Risk

Why Certain Placements Are Recommended
```

---

# STORY 5 — DATA TRUST

## Business Question

```text
Can the information be trusted?
```

## Business Objective

Validate confidence in the data.

---

## Audience

```text
Animal Flow Operations

Data Team

Leadership
```

---

## Output

```text
Data Trust
```

---

## Supporting Signals

```text
Missing_Kennel_Assignments

Assignment_Accuracy_Pct

Capacity_Confirmation_Status

Capacity_Confirmation_Age_Hours

Data_Trust_Status
```

---

## Decision Supported

```text
Data Trust Assessment

Routing Approval
```

---

## User Action

```text
Determine whether decisions can be trusted.
```

---

## Narrative

Data quality directly impacts placement decisions.

Users must understand:

```text
Data Completeness

Data Freshness

Data Reliability
```

before acting.

---

# STORY 6 — REGIONAL HEALTH

## Business Question

```text
Which regions are experiencing capacity pressure?
```

## Business Objective

Monitor regional capacity trends.

---

## Audience

```text
Animal Flow Leadership

Regional Leadership
```

---

## Output

```text
Regional Health
```

---

## Supporting Signals

```text
Regional_DOG_Utilization_Pct

Regional_CAT_Utilization_Pct

Regional_Open_Capacity

Regional_Pressure_Index
```

---

## Decision Supported

```text
Regional Monitoring

Regional Capacity Planning
```

---

## User Action

```text
Identify regional constraints and opportunities.
```

---

## Narrative

Regional risks often appear before local issues escalate.

This section helps leadership:

```text
Detect Emerging Pressure

Balance Capacity

Plan Resource Allocation
```

---

# STORY 7 — OPERATIONAL BRIEFING

## Business Question

```text
What should we do next?
```

## Business Objective

Convert findings into actions.

---

## Audience

```text
Animal Flow Operations

Leadership

Regional Management
```

---

## Output

```text
Operational Briefing
```

---

## Supporting Signals

```text
Operational_Review_Flag

Escalation_Status

Capacity_Confirmation_Status

Data_Trust_Status
```

---

## Decision Supported

```text
Operational Planning

Escalation Management
```

---

## User Action

```text
Execute recommended actions.
```

---

## Narrative

The report concludes with operational guidance.

Users should leave the report knowing:

```text
What To Do

Who Should Do It

What Requires Escalation

What Should Be Monitored
```

---

# SECTION 09 — PAGE ARCHETYPE

## Primary Archetype

### Operational Command Centre

Purpose:

```text
Enable rapid placement decisions and operational awareness.
```

Core User:

```text
Animal Flow Operations
```

---

## Secondary Archetype

### Capacity Intelligence

Purpose:

```text
Explain capacity availability and placement constraints.
```

Core User:

```text
Animal Flow Leadership

Regional Leadership
```

---

## Supporting Archetype

### Exception Management

Purpose:

```text
Highlight risks, exclusions, escalations, and data quality issues.
```

Core User:

```text
Operations

Leadership

Data Team
```

---

# SECTION 10 — LAYOUT BLUEPRINT

## Approved Reading Order

```text
Provincial Capacity Snapshot

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

## Layout Design Principles

### Principle 01

```text
Decision Information Before Analysis
```

---

### Principle 02

```text
Risk Before Detail
```

---

### Principle 03

```text
Data Trust Before Final Action
```

---

### Principle 04

```text
Operational Briefing Always Last
```

---

## Layout Validation

The layout succeeds when users move naturally through:

```text
Context

↓

Attention

↓

Decision

↓

Analysis

↓

Trust

↓

Action
```

without needing additional navigation.

---
# SECTION 11 — VISUAL RECOMMENDATIONS

## Purpose

Visual Recommendations define how each story is visually represented.

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

Visuals exist to accelerate decisions, not to display data.

---

# STORY 0 — PROVINCIAL CAPACITY SNAPSHOT

## Question Supported

```text
What is happening across the province today?
```

### Primary Visual

**KPI Cards**

Reason:

```text
Provide immediate situational awareness.
```

Signals:

```text
Provincial_Open_Capacity

Provincial_Pressure_Index

Eligible_Centre_Count

High_Risk_Centre_Count
```

Interaction:

```text
Click KPI to drill to Regional Health.
```

---

### Supporting Visual

**Provincial Status Banner**

Reason:

```text
Summarize overall operating condition.
```

Signals:

```text
Provincial_Pressure_Index
```

---

# STORY 1 — ACTION REQUIRED

## Question Supported

```text
What requires immediate attention?
```

### Primary Visual

**Exception KPI Cards**

Reason:

```text
Surface critical operational risks.
```

Signals:

```text
Emergency_Closure_Flag

Escalation_Status

Missing_Kennel_Assignments
```

Interaction:

```text
Drill to affected centres.
```

---

### Supporting Visual

**Exception Queue**

Reason:

```text
Provide prioritized action list.
```

---

# STORY 2 — INTAKE READINESS

## Question Supported

```text
Which centres can safely receive incoming animals?
```

### Primary Visual

**Status Cards**

Reason:

```text
Quickly classify all centres.
```

Signals:

```text
Open_DOG_Spaces

Open_CAT_Spaces

DOG_Utilization_Pct

CAT_Utilization_Pct
```

---

### Supporting Visual

**Eligibility Matrix**

Reason:

```text
Separate Healthy, Monitor, and Excluded centres.
```

---

# STORY 3 — PLACEMENT DECISION BOARD

## Question Supported

```text
Which centres should be prioritized?
```

### Primary Visual

**Priority Table**

Reason:

```text
Support intake prioritization.
```

Signals:

```text
Total_Open_Capacity

Available_DOG_Capacity

Available_CAT_Capacity
```

---

### Supporting Visual

**Centre Ranking Table**

Reason:

```text
Compare placement candidates.
```

---

# STORY 4 — CAPACITY ANALYSIS

## Question Supported

```text
Why can or cannot centres receive additional animals?
```

### Primary Visual

**Comparison Cards**

Reason:

```text
Explain capacity constraints.
```

Signals:

```text
DOG_Utilization_Pct

CAT_Utilization_Pct

Capacity_Pressure_Index
```

---

### Supporting Visual

**Capacity Breakdown Chart**

Reason:

```text
Explain drivers of intake restrictions.
```

---

# STORY 5 — DATA TRUST

## Question Supported

```text
Can the information be trusted?
```

### Primary Visual

**Exception Matrix**

Reason:

```text
Highlight data quality issues affecting confidence.
```

Signals:

```text
Missing_Kennel_Assignments

Assignment_Accuracy_Pct

Capacity_Confirmation_Status
```

---

### Supporting Visual

**Data Trust Scorecard**

Reason:

```text
Provide overall trust assessment.
```

---

# STORY 6 — REGIONAL HEALTH

## Question Supported

```text
Which regions are experiencing capacity pressure?
```

### Primary Visual

**Horizontal Bar Chart**

Reason:

```text
Compare regional pressure levels.
```

Signals:

```text
Regional_Pressure_Index

Regional_Open_Capacity
```

---

### Supporting Visual

**Regional Ranking Table**

Reason:

```text
Identify strongest and weakest regions.
```

---

# STORY 7 — OPERATIONAL BRIEFING

## Question Supported

```text
What should we do next?
```

### Primary Visual

**Recommendation Cards**

Reason:

```text
Convert insights into actions.
```

Signals:

```text
Operational_Review_Flag

Escalation_Status

Action Matrix
```

---

### Supporting Visual

**Operational Task Board**

Reason:

```text
Track ownership and action execution.
```

---

# Visual Design Standards

Every visual must:

```text
Support A Question

Support A Signal

Support A Decision

Support A User Action
```

---

# SECTION 12 — IMPLEMENTATION NOTES

## Purpose

Provide guidance for downstream:

```text
TRD Agent

Semantic Design Agent

Build Agent
```

while keeping the DSC business focused.

---

## Data Freshness Expectations

| Data Set | Expected Refresh |
|----------|----------|
| Capacity Utilization | < 2 Hours |
| Emergency Closures | < 15 Minutes |
| Capacity Confirmation | Daily Minimum |
| Data Quality Metrics | Daily |
| Regional Aggregates | Hourly |

---

## Expected Business Grain

### Centre Level

```text
Centre

Species

DateTime
```

---

### Regional Level

```text
Region

DateTime
```

---

### Executive Level

```text
Province

DateTime
```

---

## Business Calculation References

### DOG Utilization

```text
DOG Occupied

/

DOG Capacity
```

---

### CAT Utilization

```text
CAT Occupied

/

CAT Capacity
```

---

### Capacity Pressure Index

```text
Business Composite Indicator

Derived From:

DOG Utilization

CAT Utilization

Available Capacity
```

---

## Semantic Design Expectations

Must support:

```text
Placement Readiness

Capacity Utilization

Regional Monitoring

Data Trust

Operational Escalation
```

---

## Technical Constraints

Not defined in DSC.

Technical implementation belongs to:

```text
TRD

Semantic Design

Build Artifacts
```

---

# SECTION 13 — VALIDATION CHECKLIST

## Decision Model

☑ Primary Decision Defined

☑ Secondary Decisions Defined

☑ Owner Defined

☑ Success Criteria Defined

---

## Business Questions

☑ Question Coverage Complete

☑ Categories Complete

☑ Decisions Supported

---

## Signals

☑ Signal Coverage Complete

☑ Signal Definitions Complete

☑ Signal Contracts Complete

---

## Thresholds

☑ Thresholds Defined

☑ Business Meaning Defined

☑ Actions Defined

---

## Traceability

☑ Question → Signal

☑ Signal → Threshold

☑ Threshold → Decision

☑ Decision → Action

☑ Story Traceability

☑ Visual Traceability

---

## Stories

☑ Story 0 Complete

☑ Story 1 Complete

☑ Story 2 Complete

☑ Story 3 Complete

☑ Story 4 Complete

☑ Story 5 Complete

☑ Story 6 Complete

☑ Story 7 Complete

---

## Design

☑ Archetype Complete

☑ Layout Complete

☑ Visual Recommendations Complete

☑ Wireframe Alignment Complete

---

# SECTION 14 — APPROVAL GATE

## Decision Model

☑ Approved

---

## Business Question Matrix

☑ Approved

---

## Business Logic Model

☑ Approved

---

## Signal Definitions

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

## Narrative Story

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

## Implementation Notes

☑ Approved

---

# DSC SUCCESS STATEMENT

This artifact represents:

```text
ANIMALFLOW_REPORT_STORY_GOLD_v1.0
```

The official benchmark Decision Story Contract for:

```text
Decision Story Agent

Decision Story Review Agent

Template Evolution Agent

Mockup Agent

TRD Agent

Semantic Design Agent
```

A Decision Story Contract succeeds when:

```text
Every Question

Supports A Decision

Every Signal

Supports A Question

Every Threshold

Supports An Action

Every Action

Supports A Business Outcome

Every Story

Supports User Decision Making

Every Visual

Supports A Story
```

and users can confidently determine:

```text
Where Animals Can Be Placed

Where Animals Should Not Be Placed

What Risks Exist

What Actions Must Be Taken
```

within the defined operational timeframes.

---

# NEXT STEP

Generate:

```text
MOCKUP_GOLD_v1.0.md
```

using:

```text
ANIMALFLOW_REPORT_STORY_MATRIX_GOLD_v1.0

+

ANIMALFLOW_REPORT_STORY_GOLD_v1.0
```

as the governing design contracts.