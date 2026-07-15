# REPORT_STORY_MATRIX_v4.0.md
## Animal Flow — Live Capacity — Decision Matrix (Test_Run_04)

LLM Variant: Alternate (Test_Run_04)

---

# Primary Decision

Which centres currently have sufficient capacity to support incoming animals?

---

# Questions

- Which centres have available DOG capacity?
- Which centres have available CAT capacity?
- Which centres are approaching critical utilization?
- Which centres have emergency closures?
- Which centres have data-quality issues affecting capacity?

---

# Signals

- Open DOG Spaces
- Open CAT Spaces
- DOG Utilization %
- CAT Utilization %
- Emergency Closure Flag
- Missing Kennel Assignments
- Last Capacity Confirmation Age

---

# Thresholds (examples)

- DOG Utilization <80% → Candidate Centre
- DOG Utilization 80–99% → Review Before Routing
- DOG Utilization ≥100% → Exclude Centre
- Missing Kennel Assignments = 0 → Healthy
- Missing Kennel Assignments 1–3 → Warning
- Missing Kennel Assignments >3 → Critical

---

# Actions

- Route intake to Candidate Centres
- Flag centres for data cleanup when Missing Kennel Assignments >3
- Temporarily exclude centres with Emergency Closure flag

---

# Validation Checklist

- Primary Decision present
- Questions mapped to signals
- Thresholds provided for key signals
- Actions linked to thresholds
- Traceability from question → signal → threshold → action
