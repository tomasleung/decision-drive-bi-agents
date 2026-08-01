# REPORT_STORY_v7.1

## Decision Story Contract (DSC)
### Decision-Driven BI Framework

---

# DOCUMENT METADATA

Document Type:
Decision Story Contract (DSC)[cite: 18]

Version:
7.1[cite: 18]

Status:
Approved[cite: 18]

Capability:
Animal Flow — Live Capacity Reporting[cite: 22]

Business Owner:
Animal Flow Leadership[cite: 22]

Decision Owner:
Animal Flow Team[cite: 22]

Purpose:
Convert an approved Decision Story Matrix into a complete Decision Story Contract (DSC) to eliminate business rediscovery during downstream implementation[cite: 18].

---

# SECTION 01 — EXECUTIVE SUMMARY
Animal Flow requires a centralized analytical view of capacity utilization, availability, data quality, centre comparisons, regional monitoring, and operational prioritization across all Community Animal Centres (CACs)[cite: 22]. This solution provides provincial and regional intelligence to complement the Live Capacity Management Power App, enabling identification of qualified intake centres within 30 seconds[cite: 22].

---

# SECTION 02 — DECISION MODEL
* **Primary Decision:** Which centres currently have sufficient capacity to support incoming animals?[cite: 22]
* **Decision Owner:** Animal Flow Team[cite: 22]
* **Decision Authority:** Animal Flow Leadership[cite: 22]
* **Governing Business Rule:** Capacity + Data Trust + Operational Status = Placement Readiness.
* **Success Criteria:** Identify qualified centres within 30 seconds[cite: 22].

---

# SECTION 05 — SIGNAL DEFINITIONS (Sample)
* **Signal Name:** DOG Utilization %[cite: 22]
* **Business Definition:** Percentage of operational DOG spaces currently occupied[cite: 22].
* **Business Meaning:** Identifies centres nearing or exceeding capacity limits[cite: 22].
* **Question Supported:** Which centres currently have available DOG capacity?[cite: 22]
* **Action Supported:** Pause or restrict DOG intake[cite: 22].

---

# SECTION 09 — NARRATIVE STORY DESIGN (Full 8-Story Set)

## Story 0 — Executive Context
* **Business Question:** What is the current provincial capacity and data trust status?[cite: 17]
* **Audience:** Animal Flow Leadership / Management[cite: 22]
* **Decision Supported:** Primary Intake Capacity Decision[cite: 22]
* **User Action:** Direct attention to high-level systemic issues[cite: 17].
* **Narrative:** Provides a provincial overview of total available DOG and CAT spaces alongside the overall capacity confirmation rate to establish immediate situational awareness and data trust[cite: 17].

## Story 1 — Action Required
* **Business Question:** Which centres have emergency closures or >= 95% utilization?[cite: 22]
* **Audience:** Animal Flow Team[cite: 22]
* **Decision Supported:** Centre Intake Eligibility Decision[cite: 22]
* **User Action:** Pause or restrict intake / Exclude centre[cite: 22].
* **Narrative:** Immediately surfaces centres that cannot accept animals due to critical capacity exhaustion or emergency closures, preventing invalid placement decisions[cite: 17].

## Story 2 — Decision Readiness
* **Business Question:** Are centre capacities confirmed and data fresh?[cite: 22]
* **Audience:** Animal Flow Leadership[cite: 22]
* **Decision Supported:** Capacity Confidence Review[cite: 22]
* **User Action:** Validate capacity before placement[cite: 22].
* **Narrative:** Assesses operational readiness by highlighting centres that have not confirmed their capacity via the Power App or have stale ShelterBuddy sync times[cite: 17].

## Story 3 — Decision Board
* **Business Question:** Which centres currently have the most open DOG/CAT spaces?[cite: 22]
* **Audience:** Animal Flow Team[cite: 22]
* **Decision Supported:** Centre Intake Eligibility Decision[cite: 22]
* **User Action:** Prioritize intake[cite: 17].
* **Narrative:** Ranks and prioritizes eligible centres based on open capacity and low utilization, enabling the Animal Flow team to select intake destinations within the 30-second target[cite: 17].

## Story 4 — Analysis
* **Business Question:** What are the utilization trends across regions?[cite: 22]
* **Audience:** Animal Flow Management[cite: 22]
* **Decision Supported:** Regional Capacity Planning[cite: 22]
* **User Action:** Review redistribution strategy[cite: 22].
* **Narrative:** Explains underlying pressures contributing to capacity constraints by comparing utilization metrics across different geographic areas[cite: 17].

## Story 5 — Data Trust
* **Business Question:** Which centres have animals missing kennel assignments?[cite: 22]
* **Audience:** Centre Managers / Data Owners[cite: 22]
* **Decision Supported:** Data Quality Remediation[cite: 22]
* **User Action:** Conduct data quality review[cite: 22].
* **Narrative:** Isolates specific centres with missing kennel assignments or assignment accuracy failures, prompting Centre Managers to remediate ShelterBuddy data[cite: 17].

## Story 6 — Regional Monitoring
* **Business Question:** Which regions are experiencing the highest capacity pressures?[cite: 22]
* **Audience:** Regional Management / Animal Flow Leadership[cite: 22]
* **Decision Supported:** Regional Capacity Planning[cite: 22]
* **User Action:** Regional capacity balancing[cite: 17].
* **Narrative:** Provides a geographic breakdown of capacity, allowing leadership to spot emerging regional bottlenecks before they affect provincial operations[cite: 17].

## Story 7 — Operational Briefing
* **Business Question:** What are the recommended intake restrictions and priority centres?[cite: 22]
* **Audience:** Animal Flow Team[cite: 22]
* **Decision Supported:** Centre Intake Eligibility Decision[cite: 22]
* **User Action:** Execute placement decisions[cite: 22].
* **Narrative:** Summarizes final operational directives: which centres are open for intake, which are paused, and which require immediate data remediation[cite: 17].

---

# SECTION 12 — VISUAL RECOMMENDATIONS (Summary)
* **Story 0 (Context):** KPI Scorecards for provincial DOG/CAT spaces and confirmation rates[cite: 17].
* **Story 1 (Action Required):** Priority Alert Table highlighting closures and >= 95% utilization[cite: 17].
* **Story 2 (Readiness):** Status Indicator Matrix showing unconfirmed centres[cite: 17].
* **Story 3 (Decision Board):** Ranked Prioritization Table for open capacity matching[cite: 17].
* **Story 4 (Analysis):** Comparative Bar/Trend Charts for regional pressure[cite: 17].
* **Story 5 (Data Trust):** Exception List for missing kennel assignments[cite: 17].
* **Story 6 (Regional):** Regional Matrix mapping capacity distribution[cite: 17].
* **Story 7 (Briefing):** Action/Recommendation Panel summarizing next steps[cite: 17].

---

# SECTION 13 — IMPLEMENTATION NOTES & SEMANTIC EXPECTATIONS
* **Refresh Expectations:** Near real-time synchronization with Live Capacity Management and ShelterBuddy[cite: 22].
* **Required Facts:** Occupancy, Space Inventory, Confirmation Status.
* **Required Dimensions:** Centres, Regions, Species (DOG/CAT).
* **Required Measures:** DOG Utilization %, CAT Utilization %, Missing Assignment Count, Capacity Confirmation Rate[cite: 22].

---

# DSC QUALITY SCORECARD
* **Total Score:** 60 / 60 (Production Ready)[cite: 18]
* **Status:** APPROVED for implementation pending final human governance sign-off by Animal Flow Leadership[cite: 18, 22].