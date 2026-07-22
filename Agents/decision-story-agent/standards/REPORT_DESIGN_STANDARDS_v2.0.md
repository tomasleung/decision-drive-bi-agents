# REPORT_DESIGN_STANDARDS_v2.0

## Decision-Driven BI Report Design Standards

---

# DOCUMENT METADATA

Document Name:
REPORT_DESIGN_STANDARDS

Version:
2.0

Owner:
Decision-Driven BI Framework

Status:
Approved Standard

Purpose:

Provide the governing design standards for creating:

- Reports
- Dashboards
- Scorecards
- Operational Command Centres
- Decision Story Contracts

The standard ensures all reporting begins with business decisions and business actions rather than data, visuals, KPIs, or technical implementation.

---

# SECTION 01 — REPORT DESIGN PHILOSOPHY

## Core Principle

The purpose of a report is to support business decisions.

The purpose of a dashboard is not to display information.

The purpose of a dashboard is to improve decision quality and business action.

---

## Traditional BI Approach

Data
↓
Charts
↓
Dashboard
↓
User Determines Action

---

## Decision-Driven BI Approach

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
Layout
↓
Visual

---

## Success Definition

A report succeeds when users can answer:

"What should I do?"

within 30 seconds of opening the report.

---

# SECTION 02 — DECISION-FIRST DESIGN

## Governing Rule

Every report must begin with a decision.

Never begin with:

- Data
- Measures
- KPIs
- Charts
- Dashboards
- Layouts

---

## Required Decision Declaration

Every report must define:

- Primary Decision
- Secondary Decisions
- Decision Owner
- Decision Frequency
- Decision Success Criteria

---

## Validation Rule

If a primary decision cannot be stated clearly:

STOP REPORT DESIGN

until the decision is defined.

---

# SECTION 03 — BUSINESS QUESTION DESIGN

## Purpose

Business questions translate decisions into information requirements.

---

## Question Requirements

Every question must:

- Support a Decision
- Be Business Relevant
- Be Measurable
- Be Actionable
- Support Future User Action

---

## Validation Rule

If a question does not support a decision:

Remove It.

---

# SECTION 04 — SIGNAL DESIGN

## Signal Definition

A signal is measurable information used to answer a business question.

---

## Signal Hierarchy

Decision
↓
Question
↓
Signal

---

## Signal Requirements

Every signal must:

- Support a Question
- Support a Decision
- Support an Action
- Be Measurable
- Be Explainable
- Be Actionable

---

## Signal Validation

If a signal cannot influence a decision or action:

Remove It.

---

# SECTION 05 — THRESHOLD DESIGN

## Purpose

Signals become meaningful when thresholds define business interpretation.

---

## Threshold Structure

Every threshold must define:

- Threshold
- Status
- Action
- Business Meaning

---

## Threshold Validation

Every threshold must answer:

- What Happened?
- Why Does It Matter?
- What Should Be Done?

---

## Validation Rule

If no action exists:

Threshold Not Required.

---

# SECTION 06 — ACTION DESIGN

## Purpose

Actions define why reporting exists.

---

## Action Structure

Every action must define:

- Condition
- Recommended Action
- Responsible Role
- Expected Outcome
- Decision Supported

---

## Action Validation

Every action must support:

- Human Decision
- Business Outcome
- Operational Response

---

# SECTION 07 — KPI DESIGN

## KPI Purpose

KPIs are decision signals.

KPIs are not decorative metrics.

---

## KPI Qualification Test

Every KPI must answer:

"What business action becomes easier because of this KPI?"

---

## KPI Structure

Every KPI must define:

- Signal
- Threshold
- Status
- Action
- Decision

---

# SECTION 08 — REPORT STORY DESIGN

## Purpose

Reports communicate a decision story.

---

## Story Progression

Reports should progress through:

Context
↓
Analysis
↓
Decision
↓
Action

---

## Story Validation

Every story section must answer at least one business question.

---

## User Validation

A user should understand:

- What is happening?
- Why is it happening?
- What requires attention?
- What decision must be made?
- What action should occur?

---

# SECTION 09 — STORY COVERAGE STANDARD

## Minimum Story Coverage

Decision-driven reports should include:

### Story 0

Executive Context

### Story 1

Action Required

### Story 2

Decision Readiness

### Story 3

Decision Prioritization

### Story 4

Analysis and Explanation

### Story 5

Data Trust

### Story 6

Regional Monitoring

### Story 7

Operational Briefing

---

## Validation Rule

Every story must:

- Support a Decision
- Support a User Action
- Support a Business Outcome

---

# SECTION 10 — PAGE ARCHETYPE DESIGN

## Purpose

Every page should represent a recognizable decision pattern.

---

## Approved Archetypes

- Operational Command Centre
- Capacity Intelligence
- Executive Monitoring
- Exception Management
- Regional Monitoring
- Data Quality Investigation
- Performance Monitoring

---

# SECTION 11 — LAYOUT DESIGN

## Purpose

Define report reading order.

---

## Reading Order

Users should naturally progress through:

Context
↓
Exception
↓
Decision Support
↓
Analysis
↓
Action

---

## Validation Rule

Layout must support report story progression.

---

# SECTION 12 — VISUAL DESIGN

## Purpose

Visuals exist only to support decisions.

---

## Visual Selection Rule

Always select:

Decision
↓
Question
↓
Signal
↓
Action
↓
Visual

Never select visuals first.

---

## Visual Validation

Every visual must support:

- Decision
- Question
- Signal
- Action

---

# SECTION 13 — TRACEABILITY DESIGN STANDARD

## Purpose

Every report element must remain fully traceable.

---

## Required Traceability Chain

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

---

## Validation Rule

No orphan:

- Questions
- Signals
- Thresholds
- Actions
- Stories
- Visuals

are permitted.

---

# SECTION 14 — DECISION READINESS STANDARD

## Purpose

Reports should be built only when sufficient business context exists.

---

## Required Inputs

Before design begins:

- Primary Decision Defined
- Secondary Decisions Defined
- Business Questions Defined
- Signals Defined
- Actions Defined
- Success Criteria Defined
- Stakeholders Defined

---

## Validation Rule

If decision readiness is not achieved:

STOP REPORT DESIGN.

Return to business discovery.

---

# SECTION 15 — SVG DESIGN STANDARDS

## Purpose

SVG is a rendering artifact.

SVG may:

- Render Approved Layout
- Render Approved Sections
- Render Approved Visuals

SVG may not:

- Create Decisions
- Create Signals
- Create Actions
- Create Thresholds
- Create KPIs

---

# SECTION 16 — DECISION STORY CONTRACT STANDARD

## Purpose

The Decision Story Contract (DSC) is the governing design artifact.

---

## Required Sections

01 Decision Model

02 Business Question Matrix

03 Business Logic Model

04 Signal Definitions

05 Threshold Matrix

06 Decision Traceability

07 Action Matrix

08 Narrative Story

09 Page Archetype

10 Layout Blueprint

11 Visual Recommendations

12 Implementation Notes

13 Validation Checklist

14 Approval Gate

---

# SECTION 17 — REPORT QUALITY CHECKLIST

Before approval verify:

□ Primary Decision Defined

□ Secondary Decisions Defined

□ Questions Defined

□ Signals Defined

□ Thresholds Defined

□ Actions Defined

□ Story Coverage Complete

□ Decision Traceability Complete

□ Layout Approved

□ Visuals Approved

□ User Action Supported

---

# FINAL REPORT VALIDATION

Every report must satisfy:

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

Nothing should appear in a report unless it can be traced through this chain.

---

# STANDARD SUCCESS STATEMENT

A reporting solution succeeds when:

Every Decision
supports Business Action

Every Question
supports a Decision

Every Signal
supports a Question

Every Threshold
supports an Action

Every Action
supports a Business Outcome

Every Story
supports User Decisions

Every Visual
supports Business Action

The resulting artifact becomes a:

Decision Product

rather than a:

Reporting Product.