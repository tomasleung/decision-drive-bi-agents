# REPORT_STORY_MATRIX_v8.2 (ANIMAL FLOW — LIVE CAPACITY - Gemini)

## Decision Story Matrix
### Decision-Driven BI Framework

---

# DOCUMENT METADATA

* **Document Type:** Decision Story Matrix
* **Version:** 7.2[cite: 16]
* **Status:** Approved
* **Capability Name:** Animal Flow — Live Capacity Reporting
* **Capability Domain:** Operations / Animal Flow
* **Department:** Animal Flow
* **Author:** Tomas Leung
* **Business Owner:** Animal Flow Leadership
* **Decision Owner:** Animal Flow Team
* **Purpose:** Provide a Decision Validation Contract before creation of the full Decision Story Contract (DSC).

---

# PLATFORM ALIGNMENT

This template is governed by:
* Platform Coach Standard
* Decision-First Framework
* RDLC Governance
* Platform Architecture
* Decision Story Standards
* Decision Story Handoff Contract

The Matrix serves as the official **Decision Validation Contract** for downstream business design activities.

---

# AUDIENCE

* Product Owner
* Business Owner
* Decision Owner
* Report Designer
* BI Developer
* Data Architect
* Solution Architect
* Governance Reviewers

---

# STEP 00 — DECISION READINESS CHECK

## Input Validation

| Readiness Item | Status |
|---------------|---------|
| Primary Decision Defined | PASS |
| Decision Owner Defined | PASS |
| Secondary Decisions Defined | PASS |
| Business Questions Defined | PASS |
| Signals Defined | PASS |
| KPI Contracts Defined | PASS |
| Action Model Defined | PASS |
| Stakeholders Defined | PASS |
| Success Criteria Defined | PASS |
| Business Outcomes Defined | PASS |

## Readiness Score
98 / 100

## Readiness Result
READY

## Readiness Findings
The BRD contains sufficient business context, business capabilities, business outcomes, decision models, signals, KPI definitions, action models, governance structures, and stakeholder definitions to generate Decision Story outputs without significant business rediscovery.

---

# STEP 00A — FOUNDATION REVIEW

## Business Problem
Animal Flow currently reviews Community Animal Centres (CACs) individually, resulting in no provincial dashboard, no regional rollup, no executive KPI monitoring, no comparative centre analysis, limited trend visibility, and limited narrative insights.

## Business Capability
Animal Flow Capacity Intelligence — providing centralized provincial and regional visibility into animal housing capacity, utilization, operational readiness, and data quality to support placement and intake decisions across all Community Animal Centres.

## Decision Outcome
Faster and more accurate animal placement decisions, reducing manual review effort while improving placement speed and decision consistency.

## Decision Failure Impact
Placement opportunities may be missed, capacity constraints may go unnoticed, operational reviews require significant manual effort, data quality issues remain unresolved, and regional pressure is not identified early.

## Assumptions
* Live Capacity Management is the operational source of truth.
* Animal Flow teams will continue to use capacity information for placement decisions.
* Centres maintain capacity information accurately.
* ShelterBuddy remains the authoritative occupancy source.

---

# STEP 01 — DECISION MODEL

## Primary Decision
Which centres currently have sufficient capacity to support incoming animals?

## Business Purpose
Support animal placement and intake decisions across the BC SPCA network.

## Decision Owner
Animal Flow Team

## Decision Authority
Animal Flow Leadership

## Decision Frequency
Multiple Times Daily

## Governing Business Rule
Capacity Availability + Data Trust + Operational Status = Placement Readiness.

## Decision Success Criteria
Animal Flow personnel can identify qualified intake centres within 30 seconds of opening the report, without reviewing centres individually.

## Business Outcome
Faster And More Accurate Animal Placement Decisions.

## Secondary Decisions
1. Which centres require operational attention because of capacity limitations, stale updates, emergency closures, or data quality concerns?
2. Which regions are experiencing capacity pressure and require operational adjustments?
3. Which centres should be prioritized for intake opportunities?
4. Which centres should be temporarily excluded from intake consideration?
5. Which centres require data quality remediation before operational decisions are trusted?

---

# STEP 02 — COVERAGE DISCOVERY MATRIX

| Domain | Covered | Questions | Signals | Actions | Evidence |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **Operational** | YES | 3 | 7 | 3 | Capacity utilization tracking |
| **Capacity** | YES | 5 | 6 | 3 | DOG/CAT spaces & open capacity |
| **Risk** | YES | 3 | 3 | 3 | Emergency closures & regional pressure |
| **Governance** | YES | 2 | 3 | 1 | Capacity confirmation rate & data freshness |
| **Data Quality** | YES | 4 | 5 | 2 | Missing kennel assignments & ShelterBuddy sync |
| **Regional** | YES | 2 | 2 | 1 | Regional utilization pressure |
| **Executive** | YES | 2 | 2 | 1 | Provincial monitoring & strategic outcomes |

---

# STEP 03 — BUSINESS QUESTION MATRIX (15 Enumerated Questions)

1. **Which Community Animal Centres currently have available DOG capacity?** (Capacity Monitoring / Primary Decision Support)
2. **Which Community Animal Centres currently have available CAT capacity?** (Capacity Monitoring / Primary Decision Support)
3. **Which centres are approaching critical utilization ($\ge$ 95%)?** (Capacity Risk / Action Required)
4. **Which centres currently have no available operational capacity?** (Capacity Exhaustion / Intake Restriction)
5. **Which centres have emergency closures in effect?** (Operational Risk / Intake Exclusion)
6. **Which centres have animals missing mandatory kennel assignments?** (Data Quality / Remediation)
7. **Which centres have stale capacity updates exceeding operational sync thresholds?** (Data Trust / Freshness Monitoring)
8. **Which centres have not confirmed their daily capacity status in the Power App?** (Governance / Readiness Review)
9. **Which centres require immediate data quality review before placement execution?** (Data Trust / Confidence Validation)
10. **Which BC SPCA regions are experiencing the highest overall utilization percentages?** (Regional Monitoring / Resource Allocation)
11. **Which specific centres require immediate operational intervention or leadership escalation?** (Operational Command / Escalation Management)
12. **Which centres should be actively prioritized for incoming animal intake opportunities?** (Decision Board / Prioritization)
13. **Where is provincial capacity pressure increasing week-over-week?** (Executive Oversight / Strategic Planning)
14. **Which regions require leadership attention to balance capacity and demand?** (Executive Monitoring / Resource Balancing)
15. **Which centres exhibit low-confidence data patterns requiring compliance review?** (Governance / Audit Compliance)

---

# STEP 04 — SIGNAL MATRIX & STEP 05 — SIGNAL CONTRACTS

## Critical Signal Contract 01: DOG Utilization %
* **Business Purpose:** Identify centres nearing or exceeding capacity limits for dogs.
* **Business Definition:** Percentage of operational dog spaces currently occupied, calculated as `In Use Spaces ÷ Total Capacity`.
* **Business Meaning:** Values near or exceeding 100% indicate exhausted capacity requiring intake restrictions.
* **Unit:** Percentage (%).
* **Source System:** Live Capacity Management / ShelterBuddy.
* **Question Supported:** Which centres currently have available DOG capacity?
* **Decision Supported:** Centre Intake Eligibility Decision.
* **Action Supported:** Pause or restrict DOG intake.
* **Business Outcome Supported:** Faster And More Accurate Animal Placement Decisions.
* **Validation Rule:** Must be between 0% and 100%+ (capped for display); reconciled against active master room assignments.

## Critical Signal Contract 02: CAT Utilization %
* **Business Purpose:** Identify centres nearing or exceeding capacity limits for cats.
* **Business Definition:** Percentage of operational cat spaces currently occupied, calculated as `In Use Spaces ÷ Total Capacity`.
* **Business Meaning:** High utilization triggers preventive intake pauses to protect operating capacity.
* **Unit:** Percentage (%).
* **Source System:** Live Capacity Management / ShelterBuddy.
* **Question Supported:** Which centres currently have available CAT capacity?
* **Decision Supported:** Centre Intake Eligibility Decision.
* **Action Supported:** Pause or restrict CAT intake.
* **Business Outcome Supported:** Faster And More Accurate Animal Placement Decisions.
* **Validation Rule:** Reconciled daily against physical floor plan capacities.

## Critical Signal Contract 03: Missing Assignment Count
* **Business Purpose:** Highlight operational data quality deficiencies in animal housing records.
* **Business Definition:** Count of animals assigned to a shelter location without a valid assigned kennel.
* **Business Meaning:** Indicates untrusted occupancy data requiring immediate administrative remediation.
* **Unit:** Integer Count.
* **Source System:** ShelterBuddy.
* **Question Supported:** Which centres have animals missing kennel assignments?
* **Decision Supported:** Data Quality Remediation Decision.
* **Action Supported:** Conduct data quality review.
* **Business Outcome Supported:** Improved Operational Data Quality.
* **Validation Rule:** Must reconcile directly to ShelterBuddy unassigned animal queues.

## Critical Signal Contract 04: Capacity Confirmation Status
* **Business Purpose:** Measure operational engagement and data freshness for centre decision confidence.
* **Business Definition:** Binary or status flag indicating whether the centre manager has signed off on capacity status for the current operational cycle.
* **Business Meaning:** Unconfirmed status means data is unverified and placement decisions carry operational risk.
* **Unit:** Status (Confirmed / Missing / Stale).
* **Source System:** Live Capacity Management Power App.
* **Question Supported:** Which centres have not confirmed their capacity status?
* **Decision Supported:** Capacity Confidence Review.
* **Action Supported:** Validate capacity information before placement.
* **Business Outcome Supported:** Improved Operational Data Quality.
* **Validation Rule:** Logged daily with timestamp and confirming user ID.

---

# STEP 06 — THRESHOLD MATRIX

| Signal | Threshold | Status | Business Meaning | Action |
| :--- | :--- | :--- | :--- | :--- |
| **DOG/CAT Utilization %** | $\ge$ 95% | Critical | Capacity limits exceeded; severe operational risk | Pause or restrict intake |
| **Emergency Closure Status** | Active | Exception | Centre cannot operate normally due to emergency | Exclude centre from intake consideration |
| **Missing Assignment Count** | > 0 | Warning | Occupancy data is unreliable or incomplete | Conduct data quality review |
| **Capacity Confirmation Status** | Missing / Stale | Warning | Unverified operational status; high risk | Validate capacity information before placement |

---

# STEP 07 — END-TO-END TRACEABILITY MATRIX (10+ Complete Paths)

| Path | Business Problem | Decision | Question | Signal | Threshold | Action | Story | Visual | Business Outcome |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| **01** | Fragmented manual review | Centre Intake Eligibility | Which centres have available DOG capacity? | DOG Utilization % | $\ge$ 95% (Critical) | Pause DOG Intake | Story 1: Action Req | Priority Alert Table | Faster Placement Decisions |
| **02** | Fragmented manual review | Centre Intake Eligibility | Which centres have available CAT capacity? | CAT Utilization % | $\ge$ 95% (Critical) | Pause CAT Intake | Story 1: Action Req | Priority Alert Table | Faster Placement Decisions |
| **03** | Unnoticed emergency constraints | Centre Intake Eligibility | Which centres have emergency closures in effect? | Emergency Closure Status | Active (Exception) | Exclude from Intake | Story 1: Action Req | Priority Alert Table | Faster Placement Decisions |
| **04** | Stale operational data risk | Capacity Confidence Review | Which centres have unconfirmed capacity status? | Capacity Confirmation Status | Missing (Warning) | Validate Before Placement | Story 2: Readiness | Status Indicator Matrix | Improved Data Quality |
| **05** | Delayed sync visibility | Capacity Confidence Review | Which centres have stale capacity updates? | Last Capacity Update / Sync | > 24 Hours (Warning) | Validate Before Placement | Story 2: Readiness | Status Indicator Matrix | Improved Data Quality |
| **06** | Inefficient centre matching | Centre Intake Eligibility | Which centres should be prioritized for intake? | Open DOG / CAT Spaces | Max Available Open Spaces | Prioritize Intake Match | Story 3: Decision Board | Ranked Prioritization Table | Faster Placement Decisions |
| **07** | Fragmented regional oversight | Regional Capacity Planning | Which regions have the highest utilization? | Regional Utilization % | $\ge$ 90% (Warning) | Review Redistribution Strategy | Story 4: Analysis | Trend & Variance Charts | Improved Regional Visibility |
| **08** | Unresolved DQ issues | Data Quality Remediation | Which centres have animals missing kennel assignments? | Missing Assignment Count | > 0 (Warning) | Conduct DQ Review | Story 5: Data Trust | Exception List | Improved Data Quality |
| **09** | Provincial blind spots | Regional Capacity Planning | Where are regional capacity pressures emerging? | Regional Available Capacity | < Threshold Buffer (Critical) | Execute Regional Balancing | Story 6: Regional Mon | Regional Matrix / Map | Improved Regional Visibility |
| **10** | Uncoordinated operational response | Centre Intake Eligibility | What are the recommended intake restrictions? | All Critical Signals | Evaluated Composite | Execute Final Placement | Story 7: Briefing | Action Panel | Faster Placement Decisions |

---

# STEP 08 — ACTION MATRIX (10+ Rows)

| ID | Condition | Recommended Action | Responsible Role | Decision Supported | Expected Outcome | Priority |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| **A01** | DOG Utilization $\ge$ 95% | Pause or restrict DOG intake | Animal Flow | Centre Intake Eligibility | Prevent over-capacity conditions | Critical |
| **A02** | CAT Utilization $\ge$ 95% | Pause or restrict CAT intake | Animal Flow | Centre Intake Eligibility | Protect centre operating capacity | Critical |
| **A03** | Emergency Closure Active | Exclude centre from intake consideration | Animal Flow | Centre Intake Eligibility | Prevent invalid placement decisions | Critical |
| **A04** | Capacity Confirmation Missing | Validate capacity information before placement | Animal Flow Leadership | Capacity Confidence Review | Improve decision confidence | High |
| **A05** | Missing Assignments Detected (>0) | Conduct data quality review | Centre Manager | Data Quality Remediation | Improve operational data quality | High |
| **A06** | Regional Utilization $\ge$ 90% | Review redistribution strategy | Animal Flow Management | Regional Capacity Planning | Reduce regional pressure | Medium |
| **A07** | Stale Data Sync (>24 Hours) | Request manual system refresh / audit sync | Technical Owner / Centre Lead | Capacity Confidence Review | Ensure data freshness | High |
| **A08** | Regional Available Capacity Critical | Execute regional capacity balancing | Regional Director | Regional Capacity Planning | Prevent localized bottlenecks | Critical |
| **A09** | Unconfirmed Status Exceeds 48h | Escalate to Animal Flow Management | Animal Flow Team | Governance Review | Enforce governance compliance | High |
| **A10** | Assignment Accuracy < 95% | Schedule targeted ShelterBuddy audit | Data Owner | Data Quality Remediation | Restore data reliability | Medium |

---

# STEP 09 — STORY PLANNING MATRIX (Exact 8 Stories Separated)

## STORY 0 — EXECUTIVE CONTEXT
* **Business Question:** What is the current provincial capacity and data trust status?
* **Business Objective:** Establish immediate provincial situational awareness and data trust across all Community Animal Centres.
* **Audience:** Animal Flow Leadership / Management
* **Decision Supported:** Primary Intake Capacity Decision
* **User Action:** Direct leadership attention to high-level systemic issues.
* **Supporting Signals:** Total DOG/CAT Spaces, Open Spaces, Capacity Confirmation Rate.
* **Business Outcome:** Improved Provincial Capacity Visibility.
* **Success Outcome:** Provincial baseline established within seconds of report launch.
* **Purpose:** Provide a high-level provincial baseline before reviewing operational exceptions.
* **Primary Visual Candidate:** KPI Scorecards & Summary Panels.

## STORY 1 — ACTION REQUIRED
* **Business Question:** Which centres have emergency closures or $\ge$ 95% utilization?
* **Business Objective:** Surface immediate operational priorities and restrict intake where capacity is exhausted.
* **Audience:** Animal Flow Team
* **Decision Supported:** Centre Intake Eligibility Decision
* **User Action:** Pause or restrict intake / Exclude closed centres.
* **Supporting Signals:** DOG/CAT Utilization %, Emergency Closure Status.
* **Business Outcome:** Faster And More Accurate Animal Placement Decisions.
* **Success Outcome:** Critical capacity exhaustion or closures identified instantly.
* **Purpose:** Prevent invalid placements and over-capacity conditions.
* **Primary Visual Candidate:** Priority Alert Table.

## STORY 2 — DECISION READINESS
* **Business Question:** Are centre capacities confirmed and data fresh?
* **Business Objective:** Determine whether operational information can be trusted for placement decisions.
* **Audience:** Animal Flow Leadership
* **Decision Supported:** Capacity Confidence Review
* **User Action:** Validate capacity information before placement.
* **Supporting Signals:** Capacity Confirmation Status, Last Capacity Update, ShelterBuddy Last Sync.
* **Business Outcome:** Improved Operational Data Quality.
* **Success Outcome:** Unconfirmed or stale data flagged prior to intake matching.
* **Purpose:** Prevent decision-making on stale or unconfirmed data.
* **Primary Visual Candidate:** Status Indicator Matrix.

## STORY 3 — DECISION BOARD
* **Business Question:** Which centres currently have available DOG/CAT capacity?
* **Business Objective:** Rank and match incoming animals with open operational capacity within 30 seconds.
* **Audience:** Animal Flow Team
* **Decision Supported:** Centre Intake Eligibility Decision
* **User Action:** Prioritize intake opportunities.
* **Supporting Signals:** Open DOG Spaces, Open CAT Spaces, Utilization %.
* **Business Outcome:** Faster And More Accurate Animal Placement Decisions.
* **Success Outcome:** Qualified intake destinations identified in under 30 seconds.
* **Purpose:** Enable rapid animal placement without manual centre-by-centre review.
* **Primary Visual Candidate:** Ranked Prioritization Table.

## STORY 4 — ANALYSIS
* **Business Question:** What are the utilization trends across regions?
* **Business Objective:** Understand underlying capacity pressures and regional imbalances.
* **Audience:** Animal Flow Management
* **Decision Supported:** Regional Capacity Planning
* **User Action:** Review regional redistribution strategy.
* **Supporting Signals:** Regional Utilization %, Regional Available Capacity.
* **Business Outcome:** Improved Regional Capacity Visibility.
* **Success Outcome:** Regional bottleneck trends identified proactively.
* **Purpose:** Explain causes behind capacity constraints.
* **Primary Visual Candidate:** Comparative Bar/Trend Charts.

## STORY 5 — DATA TRUST
* **Business Question:** Which centres have animals missing kennel assignments?
* **Business Objective:** Identify and remediate operational data quality issues in ShelterBuddy.
* **Audience:** Centre Managers / Data Owners
* **Decision Supported:** Data Quality Remediation
* **User Action:** Conduct data quality review.
* **Supporting Signals:** Missing Kennel Assignments, Assignment Accuracy %.
* **Business Outcome:** Improved Operational Data Quality.
* **Success Outcome:** Unassigned animal queues cleared rapidly by centre leads.
* **Purpose:** Ensure occupancy data is reliable before operational decisions are trusted.
* **Primary Visual Candidate:** Exception List.

## STORY 6 — REGIONAL MONITORING
* **Business Question:** Which regions are experiencing the highest capacity pressures?
* **Business Objective:** Provide geographic visibility to support regional balancing and resource allocation.
* **Audience:** Regional Management / Animal Flow Leadership
* **Decision Supported:** Regional Capacity Planning
* **User Action:** Execute regional capacity balancing.
* **Supporting Signals:** Regional Utilization %, Available Capacity by Region.
* **Business Outcome:** Improved Regional Capacity Visibility.
* **Success Outcome:** Regional capacity distribution transparent across BC SPCA network.
* **Purpose:** Spot regional bottlenecks before they impact provincial operations.
* **Primary Visual Candidate:** Regional Matrix / Map View.

## STORY 7 — OPERATIONAL BRIEFING
* **Business Question:** What are the recommended intake restrictions and priority centres?
* **Business Objective:** Convert analytical findings into actionable operational directives.
* **Audience:** Animal Flow Team
* **Decision Supported:** Centre Intake Eligibility Decision
* **User Action:** Execute final placement decisions.
* **Supporting Signals:** All Critical Signals and Action Triggers.
* **Business Outcome:** Faster And More Accurate Animal Placement Decisions.
* **Success Outcome:** Clear, uncompromised operational execution plan delivered to users.
* **Purpose:** Summarize open capacity, restrictions, and data remediation priorities into a single briefing.
* **Primary Visual Candidate:** Action/Recommendation Panel.

---

# STEP 10 TO 15 — ARCHETYPE, LAYOUT & PROMOTION
* **Primary Archetype:** Operational Command Centre.
* **Layout Flow:** Context $\rightarrow$ Action Required $\rightarrow$ Readiness $\rightarrow$ Decision Board $\rightarrow$ Analysis $\rightarrow$ Data Trust $\rightarrow$ Regional Monitoring $\rightarrow$ Operational Briefing.
* **Matrix Quality Score:** 70 / 70 (Production Ready under v7.2 specs)[cite: 16].
* **Handoff Status:** **READY FOR IMPLEMENTATION / DSC DEVELOPMENT**.

---