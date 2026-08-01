# Inputs

## Purpose

The Inputs folder contains the approved Business Requirements Document (BRD) artifacts consumed by the Decision Story Agent.

The purpose of the Input layer is to provide a governed and repeatable business input contract before Decision Story generation begins.

The quality of:

- REPORT_STORY_MATRIX
- REPORT_STORY (DSC)

depends directly on the quality of the BRD provided.

The framework follows:

Business Problem
↓
Business Capability
↓
Business Outcome
↓
Decision
↓
Question
↓
Signal
↓
Threshold
↓
Action
↓
Story
↓
Visual

Poor input quality leads to poor output quality.

The Input layer exists to reduce business rediscovery and improve consistency across Decision Story outputs.

---

# Input Contract

## Approved Template

INPUT_BRD_TEMPLATE_v1.1.md

Purpose:

Defines the required structure for all Business Requirements Documents consumed by the Decision Story Agent.

The template establishes a standard input contract and ensures the BRD contains sufficient information to generate:

- REPORT_STORY_MATRIX
- REPORT_STORY (DSC)

without significant business rediscovery.

---

# Gold Input Example

## Approved Example

INPUT_BRD_AnimalFlow_LiveCapacity_v3.1.md

Purpose:

Provides a reference implementation of the approved input contract.

This example demonstrates the expected level of:

- Business Context
- Business Capability Definition
- Business Outcome Definition
- Decision Modeling
- Business Questions
- Signal Design
- KPI Definition
- Action Design
- Governance Design
- Human Authority Definition
- Risk Documentation
- Data Sources
- Success Criteria

The example serves as a quality benchmark when developing future BRDs.

The example does not define framework requirements.

The template remains the authoritative input contract.

---

# Required BRD Sections

All BRDs should contain:

01 Business Summary

02 Business Problem

02A Business Capability

02B Business Outcomes

03 Decision Model

03A Decision Success Criteria

04 Current State (As-Is)

04A Existing Report Ecosystem

05 Future State (To-Be)

06 Business Questions

07 Required Information (Signals)

08 KPI Contracts

09 Action Model

10 Data Sources

11 Scope

12 Assumptions

13 Constraints

13A Risks And Failure Conditions

14 Success Criteria

15 Data Validation Requirements

16 Acceptance Criteria

17 Stakeholders

18 Decision Story Readiness Check

---

# Human Authority Requirements

Critical decisions should identify:

- Decision Owner
- Outcome Owner
- Approval Authority
- Escalation Authority

Human ownership must remain explicit.

The framework is:

AI Assisted
↓
Human Governed

---

# Regression Protection Requirements

When redesigning existing reports review:

- Existing Reports
- Existing Dashboards
- Existing KPIs
- Existing Decisions
- Existing Signals
- Existing Business Rules

Approved business logic should be preserved unless a justified business reason exists.

---

# Failure Awareness Requirements

BRDs should identify:

- Business Outcome Risks
- Decision Risks
- Operational Risks
- Data Risks
- Governance Risks
- Adoption Risks

Known failure conditions should be documented whenever possible.

---

# Input Validation

Before execution the Decision Story Agent should verify:

✅ Business Capability Defined

✅ Business Outcomes Defined

✅ Outcome Owner Defined

✅ Primary Decision Defined

✅ Secondary Decisions Defined

✅ Decision Authority Defined

✅ Approval Authority Defined

✅ Escalation Authority Defined

✅ Business Questions Defined

✅ Signals Defined

✅ KPI Contracts Defined

✅ Action Model Defined

✅ Data Sources Defined

✅ Risks Defined

✅ Existing Reports Reviewed

✅ Success Criteria Defined

✅ Validation Requirements Defined

✅ Stakeholders Defined

If critical sections are missing:

STOP EXECUTION

and return a BRD Readiness Assessment.

---

# Readiness Scoring

90 - 100

Ready For Decision Story Agent

70 - 89

Ready With Assumptions

Below 70

Return To BRD Author

---

# Relationship To Decision Story Agent

The Decision Story Agent consumes:

INPUT_BRD_TEMPLATE_v1.1 compliant BRDs

and produces:

REPORT_STORY_MATRIX
↓
REPORT_STORY (DSC)

The Input layer serves as the governing business contract for all downstream Decision Story activities.

---

# Input Success Statement

A BRD succeeds when:

Every Business Problem
supports a Business Capability

Every Business Capability
supports a Business Outcome

Every Business Outcome
supports a Decision

Every Decision
supports a Business Question

Every Business Question
supports a Signal

Every Signal
supports a KPI, Threshold, or Action

Every Action
supports a Business Outcome

Every Critical Decision
has human ownership

Every Outcome
has accountability

Every Risk
has visibility

and the Decision Story Agent can generate:

- REPORT_STORY_MATRIX
- REPORT_STORY (DSC)

without requiring significant business rediscovery.