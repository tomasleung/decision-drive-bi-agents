# Inputs

## Purpose

The Inputs folder contains the approved Business Requirements Document (BRD) artifacts used by the Decision Story Agent.

The purpose of the Input layer is to provide a consistent and governed business input contract before Decision Story generation begins.

The quality of:

- REPORT_STORY_MATRIX
- REPORT_STORY (DSC)

depends directly on the quality of the BRD provided.

The framework follows:

Business Requirements
↓
Decision Discovery
↓
Question Discovery
↓
Signal Discovery
↓
Action Discovery
↓
Story Design
↓
Decision Story Generation

Poor input quality leads to poor output quality.

The Input layer exists to reduce business rediscovery and improve consistency across Decision Story outputs.

---

# Input Contract

## Approved Template

INPUT_BRD_TEMPLATE_v1.0.md

Purpose:

Defines the required structure for all Business Requirements Documents consumed by the Decision Story Agent.

The template establishes a standard input contract and ensures the BRD contains sufficient information to generate:

- REPORT_STORY_MATRIX
- REPORT_STORY

without significant business rediscovery.

---

# Gold Input Example

## Approved Example

INPUT_BRD_AnimalFlow_LiveCapacity_v3.0.md

Purpose:

Provides a reference implementation of the approved input contract.

This example demonstrates the expected level of:

- Business Context
- Decision Modeling
- Business Questions
- Signal Design
- KPI Definition
- Action Design
- Data Sources
- Success Criteria
- Governance Readiness

The example should be used as a quality reference when creating future BRDs.

The example does not define framework requirements.

The template remains the authoritative input contract.

---

# Required BRD Sections

All BRDs should contain:

01 Business Summary

02 Business Problem

03 Decision Model

03A Decision Success Criteria

04 Current State (As-Is)

05 Future State (To-Be)

06 Business Questions

07 Required Information (Signals)

08 KPI Contracts

09 Data Sources

09A Action Model

10 Scope

11 Assumptions

12 Constraints

13 Success Criteria

14 Data Validation Requirements

15 Acceptance Criteria

16 Stakeholders

17 Decision Story Readiness Check

---

# Input Validation

Before execution the Decision Story Agent should verify:

✅ Primary Decision Defined

✅ Secondary Decisions Defined

✅ Business Questions Defined

✅ Signals Defined

✅ KPI Contracts Defined

✅ Action Model Defined

✅ Data Sources Defined

✅ Success Criteria Defined

✅ Validation Requirements Defined

✅ Stakeholders Defined

If critical sections are missing:

STOP EXECUTION

and return a BRD readiness assessment.

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

INPUT_BRD_TEMPLATE_v1.0 compliant BRDs

and produces:

REPORT_STORY_MATRIX
↓
REPORT_STORY (DSC)

The Input layer therefore serves as the governing business contract for all downstream Decision Story activities.

---

# Input Success Statement

A BRD succeeds when:

Every Business Goal
supports a Decision

Every Decision
supports a Business Question

Every Business Question
supports a Signal

Every Signal
supports an Action or KPI

Every Action
supports a Business Outcome

and the Decision Story Agent can generate:

- REPORT_STORY_MATRIX
- REPORT_STORY

without requiring significant business rediscovery.