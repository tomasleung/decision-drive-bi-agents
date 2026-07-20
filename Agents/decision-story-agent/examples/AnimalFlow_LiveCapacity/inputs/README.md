# Inputs
## Decision Story Agent

---

# Purpose

This folder contains the inputs used by the Decision Story Agent.

Inputs provide the business context, objectives, decisions, and success criteria required to create Decision Story artifacts.

The Decision Story Agent transforms:

```text
Business Requirements

↓

Decision Design

↓

Story Design
```

using the approved inputs contained within this folder.

---

# Input Classification

The Decision Story Agent is the first agent in the framework.

Because it is the starting point of the pipeline, its primary input originates from the business rather than another agent.

Inputs are divided into:

```text
Required Inputs

Reference Inputs
```

---

# Required Inputs

## Business Requirements Document (BRD)

Purpose:

```text
Capture Business Intent
```

Provides:

```text
Business Problem

Business Goals

Success Criteria

Business Decisions

Business Questions

Stakeholders

Constraints
```

Role:

```text
Authoritative Business Input
```

---

# Recommended BRD Content

A quality BRD should contain:

```text
Business Context

Current State

Desired State

Pain Points

Business Goals

Business Decisions

Success Metrics

Stakeholders

Constraints

Assumptions
```

---

# Reference Inputs

## Existing Reports (Optional)

Purpose:

```text
Provide Current-State Context
```

Provides:

```text
Existing Metrics

Existing Visuals

Current User Experience

Known Pain Points
```

Role:

```text
Reference Only
```

---

## Existing Dashboards (Optional)

Purpose:

```text
Understand Existing Reporting
```

Provides:

```text
Current KPI Usage

Current User Workflow

Existing Report Structure
```

Role:

```text
Reference Only
```

---

## Business Process Documentation (Optional)

Purpose:

```text
Understand Operational Workflows
```

Provides:

```text
Business Activities

Operational Processes

Decision Timing

Action Triggers
```

Role:

```text
Reference Only
```

---

# Input Priority

When conflicts exist:

```text
1. BRD

2. Business Stakeholder Direction

3. Existing Process Documentation

4. Existing Reports

5. Existing Dashboards
```

The approved BRD remains the governing document.

---

# Folder Structure

```text
inputs/

README.md

required/

└── BRD_vX.X.md

reference/

├── Existing_Report.pdf
├── Existing_Dashboard.pbix
├── Process_Documentation.docx
└── Supporting_Material
```

---

# Input Responsibilities

Inputs define:

```text
Business Intent

Business Decisions

Business Goals

Business Problems

Business Questions

Success Criteria
```

Inputs do not define:

```text
Story Design

Narrative Design

Layout Design

Visual Recommendations

Decision Story Structure
```

Those artifacts are created by the Decision Story Agent.

---

# Relationship To Outputs

```text
BRD

↓

Decision Story Agent

↓

REPORT_STORY_MATRIX

↓

REPORT_STORY (DSC)
```

The inputs explain:

```text
What the business needs
```

The outputs explain:

```text
How decisions will be supported
```

---

# Input Validation Checklist

Before executing the Decision Story Agent verify:

```text
□ BRD Available

□ Business Goals Defined

□ Business Decisions Identified

□ Stakeholders Identified

□ Success Criteria Defined

□ Input Approved

□ Scope Understood
```

---

# Success Statement

The Inputs folder succeeds when:

```text
The Decision Story Agent

can fully understand

the business problem,

the business decisions,

and the desired outcomes
```

before story design begins.

The result is:

```text
Decision-Driven

Business-Aligned

Traceable

Story Design
```