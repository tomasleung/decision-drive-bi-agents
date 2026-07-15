# REPORT_STORY_v4.0.md
## Animal Flow — Live Capacity Reporting (Test_Run_04)
### Decision Story Contract (DSC)

---

# Document Metadata

Document Type: Decision Story Contract

Version: 3.0

LLM Variant: Alternate (Test_Run_04)

Capability Name: Animal Flow — Live Capacity Reporting

Owner: Animal Flow

Purpose: Revalidation run using alternate LLM to generate a concise, traceable DSC from the BRD.

Related Documents:
- INPUT_BRD_AnimalFlow_LiveCapacity_v2.0
- REPORT_STORY_MATRIX_v4.0

---

# SECTION 01 — DECISION MODEL

Primary Decision: Which centres currently have sufficient capacity to support incoming animals?

Decision Owner: Animal Flow Team

Decision Frequency: Multiple Times Daily

---

# SECTION 02 — BUSINESS QUESTION MATRIX

- Which centres have available DOG capacity?
- Which centres have available CAT capacity?
- Which centres are approaching critical utilization?
- Which centres have emergency closures?
- Which centres have data-quality issues affecting capacity?

---

# SECTION 03 — SIGNALS & THRESHOLDS

- Open DOG Spaces — Candidate if available
- DOG Utilization % — <80% Candidate; 80–99% Review; ≥100% Exclude
- Missing Kennel Assignments — 0 Healthy; >3 Critical
- Emergency Closure — Active → Exclude
- Capacity Confirmation Age — <12h Current; >24h Stale

---

# SECTION 04 — ACTION MATRIX

- Route intake to Candidate Centres
- Flag centres for data cleanup when Missing Kennel Assignments >3
- Exclude centres with Emergency Closure flag

---

# SECTION 05 — STORY FLOW & LAYOUT NOTES

Top-down narrative: Provincial Snapshot → Intake Readiness → Operational Actions → Data Quality Remediation.

Layout: one provincial summary page, one centre-level diagnostic page, one operations tasking page.

Visual recommendations: numeric tiles for capacity, heatmap for regional pressure, table with action buttons for centre routing.

---

# Validation Checklist

- Primary Decision Defined — PASS
- Questions Mapped — PASS
- Signals & Thresholds — PASS
- Actions Linked — PASS
- Traceability — PASS

---

Notes: This run emphasizes concise traceability and clear threshold-action mapping to support rapid operational decisions.
