# INPUT_BRD_AnimalFlow_LiveCapacity_v3.0

## BC SPCA — Animal Flow Capacity Intelligence

### Decision-Driven BI Framework

---

# DOCUMENT METADATA

Document Type:
Business Requirements Document (BRD)

Version:
3.0

Capability Name:
Animal Flow — Live Capacity Reporting

Capability Domain:
Operations / Animal Flow

Department:
Animal Flow

Author:
Tomas Leung

Status:
Draft

Purpose:
Monitor capacity availability, utilization, and data quality across all Community Animal Centres (CACs) to support animal placement, operational prioritization, and capacity management decisions.

---

# SECTION 01 — BUSINESS SUMMARY

## Purpose

Provide Animal Flow with a centralized analytical view of:

- Capacity utilization
- Capacity availability
- Data quality
- Centre comparisons
- Regional monitoring
- Operational prioritization

The solution complements the Live Capacity Management Power App by providing provincial and regional intelligence across all centres.

## Business Goals

- Improve animal placement decisions
- Reduce manual centre review
- Improve operational visibility
- Improve capacity planning
- Improve identification of data quality issues
- Provide actionable operational insights

## Expected Benefits

- Faster placement decisions
- Improved operational visibility
- Increased confidence in capacity information
- Reduced manual review effort
- Improved data quality governance

---

# SECTION 02 — BUSINESS PROBLEM

## Current Challenges

Animal Flow currently reviews centres individually.

Current limitations include:

- No provincial dashboard
- No regional rollup
- No executive KPI monitoring
- No comparative centre analysis
- Limited trend visibility
- Limited narrative insights

## Business Impact

Animal placement decisions depend on manual review and centre-by-centre investigation.

Operational visibility is fragmented and inconsistent.

## Consequences

### Operational Impact

- Placement opportunities may be missed
- Capacity constraints may go unnoticed
- Operational reviews require significant manual effort

### Data Impact

- Data quality issues may remain unresolved
- Stale information may affect decisions

### Decision Impact

- Decision making is slower than desired
- Regional pressure may not be identified early

---

# SECTION 03 — DECISION MODEL

## Primary Decision

Which centres currently have sufficient capacity to support incoming animals?

### Decision Owner

Animal Flow Team

### Decision Frequency

Multiple Times Daily

## Secondary Decision 01

Which centres require operational attention because of:

- Capacity limitations
- Stale updates
- Emergency closures
- Data quality concerns

Owner:
Animal Flow Leadership

Frequency:
Daily

## Secondary Decision 02

Which regions are experiencing capacity pressure and require operational adjustments?

Owner:
Animal Flow Management

Frequency:
Weekly / Monthly

## Secondary Decision 03

Which centres should be prioritized for intake opportunities?

## Secondary Decision 04

Which centres should be temporarily excluded from intake consideration?

## Secondary Decision 05

Which centres require data quality remediation before operational decisions are trusted?

---

# SECTION 03A — DECISION SUCCESS CRITERIA

## Primary Decision Success

Animal Flow personnel can identify qualified intake centres within 30 seconds of opening the report.

Placement decisions can be made without reviewing centres individually.

## Operational Success

- Capacity risks identified proactively
- Emergency closures visible immediately
- Regional pressure visible at a glance

## Data Trust Success

- Data quality issues are visible before decisions are made
- Users can determine confidence in reported capacity

## Business Success

- Faster placement decisions
- Reduced manual operational review
- Increased provincial visibility
- Increased regional visibility

---

# SECTION 04 — CURRENT STATE (AS-IS)

## Current Process

Animal Flow
↓
Live Capacity Management App
↓
Review One Centre At A Time
↓
Manual Comparison
↓
Operational Decision

## Current Limitations

- Provincial visibility unavailable
- Regional visibility unavailable
- Data quality review separated from capacity review
- Decisions rely on local observations rather than aggregate intelligence

---

# SECTION 05 — FUTURE STATE (TO-BE)

## Provincial Monitoring

Required capabilities:

- Total DOG Capacity
- Total CAT Capacity
- Open Space Availability
- Utilization Metrics
- Emergency Closure Monitoring

## Regional Monitoring

Required capabilities:

- Capacity By Region
- Capacity By Centre
- Capacity Comparison
- Operational Risk Monitoring

## Data Quality Monitoring

Required capabilities:

- Missing Kennel Assignments
- Unconfirmed Capacity Updates
- Stale Data
- Assignment Accuracy

## Decision Support

Required capabilities:

- Centre Prioritization
- Capacity Risk Identification
- Operational Exception Management
- Narrative Analysis
- Commentary

---

# SECTION 06 — BUSINESS QUESTIONS

## Capacity Questions

- Which centres currently have available DOG capacity?
- Which centres currently have available CAT capacity?
- Which centres are approaching critical utilization?
- Which centres have no available capacity?
- Which centres have emergency closures in effect?

## Data Quality Questions

- Which centres have animals missing kennel assignments?
- Which centres have stale capacity updates?
- Which centres have not confirmed capacity status?
- Which centres require data quality review?

## Operational Questions

- Which regions have the highest utilization?
- Which centres require intervention?
- Which centres should be prioritized for intake decisions?

## Executive Questions

- Where is provincial capacity pressure increasing?
- Which regions require leadership attention?

## Governance Questions

- Which centres have low confidence data?
- Which centres require compliance review?

---

# SECTION 07 — REQUIRED INFORMATION (SIGNALS)

## Capacity Signals

- Total DOG Spaces
- Open DOG Spaces
- Total CAT Spaces
- Open CAT Spaces
- DOG Utilization %
- CAT Utilization %
- Emergency Closure Status

Purpose:
Identify capacity availability and placement opportunities.

## Data Quality Signals

- Missing Kennel Assignments
- Assignment Accuracy %
- Capacity Confirmation Status
- Last Capacity Update
- ShelterBuddy Last Sync

Purpose:
Validate trust and confidence in operational information.

## Governance Signals

- Capacity Confirmation Rate
- Data Freshness
- Data Quality Score

## Regional Signals

- Regional Utilization %
- Regional Available Capacity

---

# SECTION 08 — KPI CONTRACTS

## Capacity Utilization %

Business Definition:
Percentage of operational spaces currently occupied.

Calculation:
In Use Spaces ÷ Total Capacity

Owner:
Animal Flow

Type:
Operational KPI

Update Frequency:
Near Real-Time

## Missing Assignment Count

Business Definition:
Animals assigned to a shelter location without a valid kennel.

Owner:
Centre Manager

Type:
Data Quality KPI

Update Frequency:
Near Real-Time

## Capacity Confirmation Rate

Business Definition:
Percentage of centres that have confirmed capacity status.

Owner:
Animal Flow

Type:
Governance KPI

Update Frequency:
Daily

---

# SECTION 09 — DATA SOURCES

| Data Domain | Source System | Purpose |
|------------|---------------|----------|
| Capacity Configuration | CAT Master | Space Inventory |
| Capacity Configuration | DOG Master | Space Inventory |
| Animal Occupancy | ShelterBuddy | Occupancy Source |
| Capacity Confirmation | Power App | Operational Sign-Off |
| Utilization Summary | Live Capacity Management | KPI Generation |

---

# SECTION 09A — ACTION MODEL

## Action 01

Condition:
DOG Utilization >= 95%

Recommended Action:
Pause or restrict DOG intake.

Responsible Role:
Animal Flow

Expected Outcome:
Prevent over-capacity conditions.

## Action 02

Condition:
CAT Utilization >= 95%

Recommended Action:
Pause or restrict CAT intake.

Responsible Role:
Animal Flow

Expected Outcome:
Protect centre operating capacity.

## Action 03

Condition:
Emergency Closure Active

Recommended Action:
Exclude centre from intake consideration.

Responsible Role:
Animal Flow

Expected Outcome:
Prevent invalid placement decisions.

## Action 04

Condition:
Capacity Confirmation Missing

Recommended Action:
Validate capacity information before placement.

Responsible Role:
Animal Flow Leadership

Expected Outcome:
Improve decision confidence.

## Action 05

Condition:
Missing Kennel Assignments Detected

Recommended Action:
Conduct data quality review.

Responsible Role:
Centre Manager

Expected Outcome:
Improve operational data quality.

## Action 06

Condition:
Regional Utilization Exceeds Threshold

Recommended Action:
Review redistribution strategy.

Responsible Role:
Animal Flow Management

Expected Outcome:
Reduce regional pressure.

---

# SECTION 10 — SCOPE

## In Scope

- Provincial Capacity Dashboard
- Regional Capacity Dashboard
- Centre Comparison Reporting
- Capacity Utilization KPIs
- Data Quality KPIs
- Confirmation Tracking
- Narrative Analysis
- Power App Drillthrough Links

## Out Of Scope

- Capacity Management
- Floor Plan Editing
- ShelterBuddy Record Maintenance
- Kennel Configuration Management
- Predictive Analytics
- Automated Animal Placement

---

# SECTION 11 — ASSUMPTIONS

- Live Capacity Management is the operational source of truth.
- ShelterBuddy is the authoritative occupancy source.
- Centres maintain information accurately.
- Power App information is available for reporting.

---

# SECTION 12 — CONSTRAINTS

- Reporting depends on operational updates.
- Data quality depends on centre compliance.
- Narrative insights depend on underlying data quality.
- Data latency depends on synchronization schedules.

---

# SECTION 13 — SUCCESS CRITERIA

## Visibility

Animal Flow can monitor all centres through a single dashboard.

Regional and provincial capacity can be reviewed without opening multiple centre views.

## Decision Support

Capacity-related decisions become faster.

Priority centres can be identified quickly.

## Data Quality

Missing kennel assignments are visible.

Stale or unconfirmed data is easily identified.

## Adoption

Power BI becomes the monitoring layer.

Power App remains the operational management layer.

---

# SECTION 14 — DATA VALIDATION REQUIREMENTS

The solution must validate:

- Dashboard totals reconcile to Live Capacity Management
- Capacity counts reconcile to floor plan calculations
- Missing assignment counts reconcile to ShelterBuddy
- Data freshness indicators are accurate
- Narrative insights align with metrics

---

# SECTION 15 — ACCEPTANCE CRITERIA

## Governance

- Product Owner Approval
- Data Owner Approval
- KPI Definitions Approved

## Operational Readiness

- Provincial Dashboard Available
- Regional Dashboard Available
- Centre Drillthrough Operational

## Data Integrity

- Capacity Counts Reconcile
- Data Quality Metrics Validated
- Dashboard Refresh Successful

---

# SECTION 16 — STAKEHOLDERS

## Product Owner

Cynthia Boulter

## Data Owner

Kahlee Demers

## Data Architecture

Tomas Leung

## Primary Consumers

- Animal Flow Team
- Animal Flow Leadership
- Animal Flow Management

---

# SECTION 17 — DECISION STORY READINESS CHECK

| Check | Status |
|---------|---------|
| Primary Decision Defined | YES |
| Secondary Decisions Defined | YES |
| Decision Owner Defined | YES |
| Business Questions Defined | YES |
| Signals Defined | YES |
| KPI Contracts Defined | YES |
| Action Model Defined | YES |
| Data Sources Defined | YES |
| Success Criteria Defined | YES |
| Validation Requirements Defined | YES |
| Acceptance Criteria Defined | YES |
| Stakeholders Defined | YES |

## Readiness Score

95 / 100

## Readiness Status

READY FOR DECISION STORY AGENT

## Validation Notes

This BRD contains sufficient business context, decision logic, questions, signals, actions, governance requirements, and stakeholder information to generate:

- REPORT_STORY_MATRIX
- REPORT_STORY (DSC)

without significant business rediscovery.

---

# BRD SUCCESS STATEMENT

This BRD succeeds when:

Every Business Goal supports a Decision.

Every Decision supports Business Questions.

Every Business Question supports a Signal.

Every Signal supports a KPI, Threshold, or Action.

Every Action supports a Business Outcome.

The Decision Story Agent can generate:

- REPORT_STORY_MATRIX
- REPORT_STORY

without requiring additional business discovery.