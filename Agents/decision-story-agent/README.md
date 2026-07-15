# Decision Story Agent

## Purpose

The Decision Story Agent converts a Business Requirements Document (BRD) into a Decision Story Contract (DSC).

The agent follows the Decision-Driven BI Framework and ensures report design begins with business decisions and operational actions rather than visuals, charts, or technical implementation.

The output becomes the governing design contract for all downstream agents.

---

# Question Answered

The Decision Story Agent exists to answer:

```text
What decisions should the report support?

What business questions must be answered?

What signals should be monitored?

What thresholds define success or risk?

What actions should users take?

What story should the report tell?
```

---

# Transformation

```text
BRD

↓

Decision Story Agent

↓

REPORT_STORY_MATRIX

↓

REPORT_STORY (DSC)
```

The Decision Story Agent transforms:

```text
Business Requirements

↓

Decision Design

↓

Story Design

↓

Decision Story Contract
```

---

# Agent Position

```text
BRD

↓

Decision Story Agent

↓

REPORT_STORY_MATRIX

↓

REPORT_STORY (DSC)

↓

Mockup Agent

↓

MOCKUP.md

↓

MOCKUP.svg

↓

TRD Agent

↓

TRD

↓

Semantic Design Agent

↓

DATA_MODEL_MATRIX

↓

SEMANTIC_MODEL_SPEC

↓

MEASURE_CONTRACT

↓

Semantic Build Agent

↓

Fabric Semantic Model

↓

Report Build Agent

↓

Power BI Report
```

---

# Inputs

## Required

```text
Business Requirements Document (BRD)
```

---

## Expected Content

```text
Business Problem

Business Goals

Business Decisions

Business Questions

Signals

Thresholds

Actions

Stakeholders

Success Criteria

Constraints
```

---

# Standards

The agent must follow:

```text
REPORT_DESIGN_STANDARDS_v1.0
```

Location:

```text
standards/
```

Purpose:

```text
Decision Modeling

Question Modeling

Signal Identification

Action Alignment

Story Design Standards
```

---

# Templates

The agent populates approved templates.

## Template 01

```text
REPORT_STORY_MATRIX_TEMPLATE_v1.0
```

Purpose:

```text
Decision Validation

Question Validation

Signal Validation

Threshold Validation

Action Validation
```

---

## Template 02

```text
REPORT_STORY_TEMPLATE_v1.0
```

Purpose:

```text
Decision Story Contract

Narrative Design

Story Flow Design

Layout Blueprint Design

Visual Recommendation Design
```

Location:

```text
templates/
```

---

# Guidelines

The agent should follow:

```text
DECISION_STORY_GUIDELINES_v1.0
```

Location:

```text
guidelines/
```

Purpose:

```text
Decision Modeling Guidance

Signal Design Guidance

Story Design Guidance

Narrative Design Guidance

Validation Guidance
```

---

# Outputs

## Output 01

```text
REPORT_STORY_MATRIX_vX.X.md
```

Purpose:

```text
Validate the Decision Framework
```

Documents:

```text
Decisions

Business Questions

Signals

Thresholds

Actions

Story Flow
```

---

### Key Question Answered

```text
What decisions should the report support?
```

---

## Output 02

```text
REPORT_STORY_vX.X.md
```

Purpose:

```text
Create the governing Decision Story Contract
```

Documents:

```text
Decision Model

Business Logic

Narrative Story

Audience

Story Flow

Layout Blueprint

Visual Recommendations

Business Journey
```

---

### Key Question Answered

```text
What story should the report tell?
```

---

# Workflow

```text
BRD

↓

Decision Analysis

↓

Business Questions

↓

Signal Analysis

↓

Threshold Analysis

↓

Action Analysis

↓

Story Design

↓

Narrative Structure

↓

Layout Blueprint

↓

Visual Recommendations

↓

REPORT_STORY_MATRIX

↓

REPORT_STORY (DSC)
```

---

# Validation

The Decision Story Agent must validate:

```text
Decision Completeness

Business Question Coverage

Signal Coverage

Threshold Coverage

Action Coverage

Story Consistency

Narrative Consistency

Decision Traceability
```

---

# Approval Gate

Approve:

```text
REPORT_STORY_MATRIX

REPORT_STORY (DSC)
```

Approval confirms:

```text
Business Decisions Approved

Business Questions Approved

Signals Approved

Thresholds Approved

Actions Approved

Story Approved
```

---

# Folder Structure

```text
decision-story-agent/

README.md

skill.md

standards/

templates/

guidelines/

inputs/

outputs/

test-run/

examples/
```

---

# Relationship Between Inputs and Outputs

Inputs provide:

```text
Business Intent

Business Context

Decision Requirements
```

Outputs provide:

```text
Decision Framework

Story Framework

Design Contract
```

Transformation:

```text
Business Requirements

↓

Decision Requirements

↓

Business Story

↓

Design Contract
```

---

# Production Status

Version

```text
1.0
```

Status

```text
Production Ready
```

Validation

```text
Approved

Framework Compliant

Ready For Production Use
```

---

# Success Criteria

The agent succeeds when:

```text
Every Decision

supports a Business Question

Every Business Question

supports a Signal

Every Signal

supports a Threshold

Every Threshold

supports an Action

Every Action

supports a Decision

Every Story Section

supports User Action
```

and stakeholders can answer:

```text
What is happening?

Why is it happening?

What requires attention?

What decision must be made?

What action should be taken?
```

without reviewing implementation details.

---

# Success Statement

The final output must function as a:

```text
Decision Product
```

rather than a:

```text
Reporting Product
```

The Decision Story Agent succeeds when approved business requirements are transformed into a governed Decision Story Contract that can guide:

```text
Mockup Design

Technical Design

Semantic Design

Future Report Development
```

without revisiting the original business requirements.