# INPUT_BRD_AnimalFlow_LiveCapacity_v3.1

## BC SPCA — Animal Flow Capacity Intelligence

### Decision-Driven BI Framework

---

# DOCUMENT METADATA

Document Type:
Business Requirements Document (BRD)

Version:
3.1

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

# SECTION 02A — BUSINESS CAPABILITY

## Capability Name

Animal Flow Capacity Intelligence

## Capability Description

Provide centralized provincial and regional visibility into animal housing capacity, utilization, operational readiness, and data quality to support placement and intake decisions across all Community Animal Centres.

## Capability Owner

Animal Flow Leadership

## Strategic Importance

The Animal Flow function is responsible for matching animal placement needs with available operational capacity across the BC SPCA network.

The capability supports:

- Animal placement decisions
- Capacity planning
- Operational prioritization
- Regional balancing
- Data quality governance

Without centralized visibility, placement decisions require manual investigation and centre-by-centre review.

## Current Capability Challenges

- Provincial capacity visibility is limited
- Regional capacity visibility is limited
- Capacity decision making requires manual analysis
- Data quality review is disconnected from operational review
- Operational prioritization is time consuming

## Desired Capability Improvements

- Provincial operational visibility
- Regional operational visibility
- Faster placement decisions
- Unified operational and data quality monitoring
- Improved operational intelligence

---

# SECTION 02B — BUSINESS OUTCOMES

## Primary Outcome

Outcome:

Faster And More Accurate Animal Placement Decisions

Outcome Owner:

Animal Flow Leadership

Success Measure:

Time Required To Identify Qualified Intake Centres

Target:

Identify Qualified Centres Within 30 Seconds

Business Impact:

Reduce manual review effort while improving placement speed and decision consistency.

---

## Secondary Outcomes

### Outcome 01

Improved Provincial Capacity Visibility

### Outcome 02

Improved Regional Capacity Visibility

### Outcome 03

Improved Operational Data Quality

---

## Strategic Outcomes

- Improved Capacity Utilization
- Improved Provincial Resource Management
- Improved Decision Consistency
- Improved Organizational Visibility

---

## Outcome Success Criteria

Animal Flow personnel can identify placement opportunities quickly without reviewing centres individually.

Operational capacity issues become visible before they affect placement decisions.

Data quality concerns become visible before operational decisions are made.

---

# SECTION 03 — DECISION MODEL

## Primary Decision

Which centres currently have sufficient capacity to support incoming animals?

### Decision Owner

Animal Flow Team

### Decision Authority

Animal Flow Leadership

### Approval Authority

Animal Flow Management

### Escalation Authority

Animal Flow Management

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

# SECTION 04A — EXISTING REPORT ECOSYSTEM

## Existing Reports

- Live Capacity Management Reporting
- Centre-Level Capacity Views

## Existing Dashboards

- Live Capacity Management Power App

## Existing KPIs

- Capacity Utilization %
- Missing Assignment Count
- Capacity Confirmation Rate

## Existing Decisions

- Centre Intake Eligibility
- Regional Capacity Review

## Existing Signals

- Open Capacity
- Utilization Percentage
- Capacity Confirmation Status
- Missing Kennel Assignments

## Existing Known Issues

- Centre-by-centre review required
- Limited provincial visibility
- Limited regional visibility
- Data quality review separated from operational review

## Preservation Requirements

The solution should preserve approved capacity calculations, occupancy calculations, confirmed capacity processes, and Live Capacity Management operational workflows.

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

### Question Documentation Template

Question:

Which centres currently have sufficient capacity to receive incoming animals?

Business Purpose:

Support animal placement decisions.

Business Outcome Supported:

Faster And More Accurate Animal Placement Decisions

Decision Supported:

Primary Intake Capacity Decision

Priority:

Critical

Question Owner:

Animal Flow Team

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

### Signal Documentation Template

Signal Name:

DOG Utilization %

Business Purpose:

Identify centres nearing capacity limits.

Business Outcome Supported:

Faster And More Accurate Animal Placement Decisions

Question Supported:

Which centres currently have available DOG capacity?

Decision Supported:

Centre Intake Eligibility Decision

Business Owner:

Animal Flow

Signal Criticality:

Critical

Source System:

Live Capacity Management

---

# SECTION 08 — KPI CONTRACTS

## Capacity Utilization %

Business Definition:

Percentage of operational spaces currently occupied.

Calculation:

In Use Spaces ÷ Total Capacity

Owner:

Animal Flow

Business Outcome Supported:

Faster And More Accurate Animal Placement Decisions

Decision Supported:

Centre Intake Eligibility

Type:

Operational KPI

Update Frequency:

Near Real-Time

Business Purpose:

Identify available operational capacity.

Success Target:

Maintain operational awareness of capacity availability and capacity pressure.

Threshold Classification:

Healthy | Warning | Critical

---

## Missing Assignment Count

Business Definition:

Animals assigned to a shelter location without a valid kennel.

Owner:

Centre Manager

Business Outcome Supported:

Improved Operational Data Quality

Decision Supported:

Data Quality Review

Type:

Data Quality KPI

Update Frequency:

Near Real-Time

Business Purpose:

Identify operational data quality concerns.

Success Target:

Minimize unresolved assignment issues.

Threshold Classification:

Healthy | Warning | Critical

---

## Capacity Confirmation Rate

Business Definition:

Percentage of centres that have confirmed capacity status.

Owner:

Animal Flow

Business Outcome Supported:

Improved Operational Data Quality

Decision Supported:

Capacity Confidence Review

Type:

Governance KPI

Update Frequency:

Daily

Business Purpose:

Measure confidence in reported capacity.

Success Target:

100% confirmation where operationally feasible.

Threshold Classification:

Healthy | Warning | Critical

---

# SECTION 09A — ACTION MODEL

## Action 01

Condition:

DOG Utilization >= 95%

Recommended Action:

Pause or restrict DOG intake.

Responsible Role:

Animal Flow

Approval Authority:

Animal Flow Management

Escalation Authority:

Animal Flow Management

Expected Outcome:

Prevent over-capacity conditions.

Business Outcome Supported:

Faster And More Accurate Animal Placement Decisions

Decision Supported:

Centre Intake Eligibility

Success Criteria:

Capacity constraints remain visible and manageable.

---

## Action 02

Condition:

CAT Utilization >= 95%

Recommended Action:

Pause or restrict CAT intake.

Responsible Role:

Animal Flow

Approval Authority:

Animal Flow Management

Escalation Authority:

Animal Flow Management

Expected Outcome:

Protect centre operating capacity.

Business Outcome Supported:

Faster And More Accurate Animal Placement Decisions

Decision Supported:

Centre Intake Eligibility

Success Criteria:

Over-capacity conditions are prevented.

---

## Action 03

Condition:

Emergency Closure Active

Recommended Action:

Exclude centre from intake consideration.

Responsible Role:

Animal Flow

Approval Authority:

Animal Flow Management

Escalation Authority:

Animal Flow Management

Expected Outcome:

Prevent invalid placement decisions.

Business Outcome Supported:

Faster And More Accurate Animal Placement Decisions

Decision Supported:

Centre Intake Eligibility

Success Criteria:

Closed centres are excluded from placement decisions.

---

## Action 04

Condition:

Capacity Confirmation Missing

Recommended Action:

Validate capacity information before placement.

Responsible Role:

Animal Flow Leadership

Approval Authority:

Animal Flow Management

Escalation Authority:

Animal Flow Management

Expected Outcome:

Improve decision confidence.

Business Outcome Supported:

Improved Operational Data Quality

Decision Supported:

Capacity Confidence Review

Success Criteria:

Placement decisions are based on trusted information.

---

## Action 05

Condition:

Missing Kennel Assignments Detected

Recommended Action:

Conduct data quality review.

Responsible Role:

Centre Manager

Approval Authority:

Animal Flow Leadership

Escalation Authority:

Animal Flow Management

Expected Outcome:

Improve operational data quality.

Business Outcome Supported:

Improved Operational Data Quality

Decision Supported:

Data Quality Remediation

Success Criteria:

Assignment issues are identified and resolved.

---

## Action 06

Condition:

Regional Utilization Exceeds Threshold

Recommended Action:

Review redistribution strategy.

Responsible Role:

Animal Flow Management

Approval Authority:

Animal Flow Leadership

Escalation Authority:

Animal Flow Leadership

Expected Outcome:

Reduce regional pressure.

Business Outcome Supported:

Improved Regional Capacity Visibility

Decision Supported:

Regional Capacity Planning

Success Criteria:

Regional capacity pressure becomes manageable.

---

# SECTION 10 — DATA SOURCES

| Data Domain | Source System | Purpose |
|------------|---------------|----------|
| Capacity Configuration | CAT Master | Space Inventory |
| Capacity Configuration | DOG Master | Space Inventory |
| Animal Occupancy | ShelterBuddy | Occupancy Source |
| Capacity Confirmation | Power App | Operational Sign-Off |
| Utilization Summary | Live Capacity Management | KPI Generation |

---

## Data Quality Requirements

Reporting should clearly identify stale, missing, inconsistent, or unconfirmed operational information.

Operational users should be able to determine confidence before making placement decisions.

---

## Data Ownership

| Data Domain | Business Owner |
|------------|----------------|
| Capacity Management | Animal Flow |
| Occupancy Information | Animal Flow |
| Capacity Confirmation | Animal Flow |
| Data Quality Monitoring | Animal Flow Leadership |

---

## Data Trust Considerations

- Data quality depends on centre compliance.
- Capacity confirmation depends on operational participation.
- Reporting confidence depends on data freshness.
- Synchronization delays may affect operational confidence.

---

# SECTION 11 — SCOPE

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

## Future Considerations

Document future enhancements explicitly excluded from the current initiative.

- Predictive Capacity Forecasting
- Capacity Trend Forecast Modeling
- Automated Capacity Recommendations
- Automated Placement Recommendations
- Advanced Resource Optimization

---

# SECTION 12 — ASSUMPTIONS

## Business Assumptions

- Live Capacity Management is the operational source of truth.
- Animal Flow teams will continue to use capacity information for placement decisions.

## Operational Assumptions

- Centres maintain capacity information accurately.
- Capacity confirmation processes remain in place.

## Data Assumptions

- ShelterBuddy remains the authoritative occupancy source.
- Power App information is available for reporting.

---

## Assumption Validation Requirements

Capacity totals, utilization measures, and data quality indicators should be validated against existing operational processes prior to report deployment.

---

# SECTION 13 — CONSTRAINTS

## Business Constraints

- Capacity decisions depend on timely operational updates.

## Technical Constraints

- Reporting depends on source system availability and synchronization.

## Process Constraints

- Capacity confirmation requires centre participation.

## Resource Constraints

- Data quality remediation depends on centre operational capacity.

---

# SECTION 13A — RISKS AND FAILURE CONDITIONS

## Business Outcome Risks

- Placement decisions do not become faster.
- Provincial visibility does not significantly improve.
- Regional awareness remains limited.

## Decision Risks

- Capacity decisions made using stale information.
- Centres incorrectly prioritized.
- Intake opportunities missed.

## Operational Risks

- Capacity pressure not identified early.
- Emergency closures not reflected quickly enough.
- Regional pressure continues to increase unnoticed.

## Data Risks

- Missing kennel assignments.
- Delayed synchronization.
- Incomplete capacity confirmation.
- Data freshness issues.

## Governance Risks

- KPI definitions interpreted inconsistently.
- Capacity confirmation process not followed.
- Reporting trust reduced through inconsistent operational processes.

## Adoption Risks

- Users continue manual review processes.
- Dashboard adoption remains low.
- Operational decisions continue outside approved reporting processes.

---

## Known Failure Conditions

Capacity information becomes outdated.

Emergency closure information is unavailable or delayed.

Data quality concerns reduce trust in reported capacity.

Users bypass reporting and rely on manual centre-by-centre review.

---

## Mitigation Approaches

- Data freshness monitoring
- Capacity confirmation monitoring
- Data quality KPI monitoring
- Governance reviews
- Operational training and adoption activities

---

# SECTION 14 — SUCCESS CRITERIA

## Business Outcome Success

Animal Flow personnel can identify intake opportunities significantly faster than current manual review processes.

## Decision Success

Users can determine qualified intake centres within 30 seconds.

## Operational Success

Capacity pressure, closures, and priority centres are visible immediately.

## Reporting Success

Provincial and regional visibility is available within a single reporting experience.

## Adoption Success

Power BI becomes the primary monitoring and intelligence layer.

## Governance Success

Data quality issues and confidence indicators are visible before operational decisions occur.

---

# SECTION 15 — DATA VALIDATION REQUIREMENTS

## Reconciliation Requirements

- Dashboard totals reconcile to Live Capacity Management.
- Capacity totals reconcile to configured floor plans.

## Audit Requirements

- Capacity confirmation status must be auditable.
- Data freshness status must be auditable.

## Data Quality Requirements

- Missing assignment counts reconcile to ShelterBuddy.
- Capacity confirmation information is accurate.

## Trust Requirements

- Data quality indicators must reflect actual conditions.
- Confidence indicators must accurately represent operational trust.

---

## Data Freshness Requirements

- Dashboard refresh status is visible.
- Last update timestamps are visible.
- Stale information can be identified quickly.

---

## Validation Success Criteria

Operational users can determine whether reported information is trustworthy before making placement decisions.

---

# SECTION 16 — ACCEPTANCE CRITERIA

## Governance Approval

- Product Owner Approval
- Data Owner Approval
- KPI Definition Approval

## Business Approval

- Animal Flow Leadership Approval

## Operational Approval

- Provincial Dashboard Operational
- Regional Dashboard Operational
- Operational KPI Monitoring Operational

## Data Approval

- Capacity Counts Reconcile
- Data Quality Metrics Validated
- Dashboard Refresh Validation Completed

---

## Report Acceptance Criteria

- Provincial visibility available
- Regional visibility available
- Centre comparison functionality available
- Data quality monitoring available

---

## Decision Support Acceptance Criteria

- Intake eligibility decisions supported
- Regional capacity decisions supported
- Data confidence decisions supported

---

# SECTION 17 — STAKEHOLDERS

## Product Owner

Cynthia Boulter

## Business Owner

Animal Flow Leadership

## Outcome Owner

Animal Flow Leadership

## Decision Owner

Animal Flow Team

## Approval Authority

Animal Flow Management

## Escalation Authority

Animal Flow Management

## Data Owner

Kahlee Demers

## Technical Owner

Tomas Leung

## Report Consumers

- Animal Flow Team
- Animal Flow Leadership
- Animal Flow Management

---

## Governance Participants

- Animal Flow Leadership
- Product Owner
- Data Owner

---

# SECTION 18 — DECISION STORY READINESS CHECK

| Check | Status |
|---------|---------|
| Business Capability Defined | YES |
| Business Outcomes Defined | YES |
| Outcome Owner Defined | YES |
| Primary Decision Defined | YES |
| Secondary Decisions Defined | YES |
| Decision Authority Defined | YES |
| Approval Authority Defined | YES |
| Escalation Authority Defined | YES |
| Business Questions Defined | YES |
| Signals Defined | YES |
| KPI Contracts Defined | YES |
| Actions Defined | YES |
| Data Sources Defined | YES |
| Risks Defined | YES |
| Existing Reports Reviewed | YES |
| Stakeholders Defined | YES |
| Success Criteria Defined | YES |
| Validation Requirements Defined | YES |

## Readiness Score

Score:

98 / 100

### Promotion Rules

90-100

Ready For Decision Story Agent

70-89

Ready With Assumptions

Below 70

Return To BRD Author

---

## Readiness Findings

The BRD contains sufficient business context, business capabilities, business outcomes, decision models, signals, KPI definitions, action models, governance structures, and stakeholder definitions to generate Decision Story outputs without significant business rediscovery.

---

## Readiness Recommendation

Ready

---