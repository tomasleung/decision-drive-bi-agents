# REPORT_STORY_MATRIX_TEMPLATE_v7.0

## Decision Story Matrix

### Decision-Driven BI Framework

---

# DOCUMENT METADATA

Document Type:
Decision Story Matrix

Version:
7.0

Capability:
[Capability Name]

Business Owner:
[Business Owner]

Decision Owner:
[Decision Owner]

Purpose:

Provide a Decision Validation Contract before creation of the full Decision Story Contract (DSC).

The Matrix validates:

- Decision Model
- Business Questions
- Signal Design
- Threshold Design
- Action Design
- Story Coverage
- Traceability
- Report Readiness

before detailed design begins.

Audience:

- Product Owner
- Business Owner
- Report Designer
- BI Developer
- Data Architect
- Solution Architect

Approval Gate:

This artifact must be approved before creation of the Decision Story Contract (DSC).

---

# WRITER GUIDANCE

This template is a business-first artifact.

The purpose is not to document a report.

The purpose is to validate decision thinking.

The generated output must satisfy:

- DECISION_STORY_GOLD_OUTPUT_SPEC
- DECISION_STORY_REVIEW_CRITERIA
- DECISION_STORY_SCORING_MODEL

The generated output must be:

- Business Rich
- Decision Driven
- Action Oriented
- Traceable
- Governed
- Consistent

Every section should improve:

- Decision Clarity
- Business Coverage
- Traceability
- Actionability
- Story Quality

---

# STEP 00 — DECISION READINESS CHECK

## Input Validation

| Readiness Item | Status |
|---------------|---------|
| Primary Decision Defined | PASS / FAIL |
| Secondary Decisions Defined | PASS / FAIL |
| Business Questions Defined | PASS / FAIL |
| Signals Defined | PASS / FAIL |
| KPI Contracts Defined | PASS / FAIL |
| Action Model Defined | PASS / FAIL |
| Stakeholders Defined | PASS / FAIL |
| Success Criteria Defined | PASS / FAIL |

## Readiness Score

[Score]

## Readiness Result

READY

or

RETURN TO DISCOVERY

---

# STEP 01 — DECISION MODEL

## Primary Decision

[Primary Decision]

## Business Purpose

[Why This Decision Exists]

## Decision Owner

[Decision Owner]

## Decision Frequency

[Frequency]

Examples:

- Real Time
- Hourly
- Daily
- Weekly
- Monthly
- Quarterly

## Governing Business Rule

[Business Rule]

Example:

Capacity
+
Eligibility
+
Data Trust
=
Placement Readiness

## Key Discovery

[Key Discovery]

## Decision Success Criteria

Users must answer:

[Primary Business Question]

within:

[Target Time]

## Secondary Decisions

Minimum: 5 Required

- [Secondary Decision 01]
- [Secondary Decision 02]
- [Secondary Decision 03]
- [Secondary Decision 04]
- [Secondary Decision 05]

## Decision Outcomes

- [Outcome 01]
- [Outcome 02]
- [Outcome 03]
- [Outcome 04]
- [Outcome 05]

---

# STEP 02 — COVERAGE DISCOVERY MATRIX

| Domain | Covered | Questions | Signals | Actions | Evidence |
|----------|----------|----------|----------|----------|----------|
| Operational | YES / NO | [#] | [#] | [#] | [Evidence] |
| Capacity | YES / NO | [#] | [#] | [#] | [Evidence] |
| Risk | YES / NO | [#] | [#] | [#] | [Evidence] |
| Governance | YES / NO | [#] | [#] | [#] | [Evidence] |
| Data Quality | YES / NO | [#] | [#] | [#] | [Evidence] |
| Regional | YES / NO | [#] | [#] | [#] | [Evidence] |
| Executive | YES / NO | [#] | [#] | [#] | [Evidence] |

## Coverage Validation

All relevant business domains must be evaluated.

No critical business domain may be omitted without documented justification.

---

# STEP 03 — BUSINESS QUESTION MATRIX

## Minimum Coverage Requirements

Questions should be evaluated across:

- Placement
- Capacity
- Operations
- Eligibility
- Data Trust
- Governance
- Regional Monitoring
- Executive Oversight

---

## Placement Questions

| Business Question | Business Purpose | Decision Supported | Action Supported | Priority |
|----------|----------|----------|----------|----------|
| [Question] | [Purpose] | [Decision] | [Action] | Critical |

---

## Capacity Questions

| Business Question | Business Purpose | Decision Supported | Action Supported | Priority |
|----------|----------|----------|----------|----------|
| [Question] | [Purpose] | [Decision] | [Action] | High |

---

## Operations Questions

| Business Question | Business Purpose | Decision Supported | Action Supported | Priority |
|----------|----------|----------|----------|----------|
| [Question] | [Purpose] | [Decision] | [Action] | High |

---

## Eligibility Questions

| Business Question | Business Purpose | Decision Supported | Action Supported | Priority |
|----------|----------|----------|----------|----------|
| [Question] | [Purpose] | [Decision] | [Action] | High |

---

## Data Trust Questions

| Business Question | Business Purpose | Decision Supported | Action Supported | Priority |
|----------|----------|----------|----------|----------|
| [Question] | [Purpose] | [Decision] | [Action] | High |

---

## Governance Questions

| Business Question | Business Purpose | Decision Supported | Action Supported | Priority |
|----------|----------|----------|----------|----------|
| [Question] | [Purpose] | [Decision] | [Action] | High |

---

## Regional Monitoring Questions

| Business Question | Business Purpose | Decision Supported | Action Supported | Priority |
|----------|----------|----------|----------|----------|
| [Question] | [Purpose] | [Decision] | [Action] | Medium |

---

## Executive Oversight Questions

| Business Question | Business Purpose | Decision Supported | Action Supported | Priority |
|----------|----------|----------|----------|----------|
| [Question] | [Purpose] | [Decision] | [Action] | Medium |

---

## Question Validation

Minimum:

10 Questions

Recommended:

15+

Every Question Must:

- Support A Decision
- Support A Signal
- Support A Story
- Support A User Action

---
# STEP 04 — SIGNAL MATRIX

## Signal Group Guidance

Signal Groups exist to organize business monitoring and decision support.

Every Signal Group Must Define:

- Business Purpose
- Supported Decisions
- Supported Questions
- Supported Actions
- Critical Signals

---

## Placement Signals

### Signal Group Purpose

Support placement and intake decisions.

### Supported Decisions

[Supported Decision]

### Supported Questions

[Questions]

### Supported Actions

[Actions]

### Critical Signals

- [Signal]
- [Signal]
- [Signal]

---

## Capacity Signals

### Signal Group Purpose

Measure available capacity and utilization.

### Supported Decisions

[Supported Decision]

### Supported Questions

[Questions]

### Supported Actions

[Actions]

### Critical Signals

- [Signal]
- [Signal]
- [Signal]

---

## Operations Signals

### Signal Group Purpose

Monitor operational performance and exceptions.

### Supported Decisions

[Supported Decision]

### Supported Questions

[Questions]

### Supported Actions

[Actions]

### Critical Signals

- [Signal]
- [Signal]
- [Signal]

---

## Eligibility Signals

### Signal Group Purpose

Support qualification and eligibility decisions.

### Supported Decisions

[Supported Decision]

### Supported Questions

[Questions]

### Supported Actions

[Actions]

### Critical Signals

- [Signal]
- [Signal]

---

## Data Trust Signals

### Signal Group Purpose

Validate confidence in reported information.

### Supported Decisions

[Supported Decision]

### Supported Questions

[Questions]

### Supported Actions

[Actions]

### Critical Signals

- [Signal]
- [Signal]
- [Signal]

---

## Governance Signals

### Signal Group Purpose

Support compliance and oversight decisions.

### Supported Decisions

[Supported Decision]

### Supported Questions

[Questions]

### Supported Actions

[Actions]

### Critical Signals

- [Signal]
- [Signal]

---

## Regional Signals

### Signal Group Purpose

Support regional performance monitoring.

### Supported Decisions

[Supported Decision]

### Supported Questions

[Questions]

### Supported Actions

[Actions]

### Critical Signals

- [Signal]
- [Signal]

---

## Executive Signals

### Signal Group Purpose

Support executive oversight and prioritization.

### Supported Decisions

[Supported Decision]

### Supported Questions

[Questions]

### Supported Actions

[Actions]

### Critical Signals

- [Signal]
- [Signal]

---

## Signal Validation

Every Signal Must:

- Support A Question
- Support A Decision
- Support An Action
- Be Measurable
- Be Explainable
- Be Actionable

Every Signal Group Must:

- Have A Business Purpose
- Have Supporting Decisions
- Have Supporting Questions
- Have Supporting Actions

---

# STEP 05 — SIGNAL CONTRACTS

## Critical Rule

Signal Contracts are required for all critical signals.

The reader should understand:

- Why the signal exists
- What the signal means
- What decision it supports
- What action it influences

without reviewing technical documentation.

---

## Signal Contract Template

| Field | Value |
|---------|---------|
| Signal Name | [Signal] |
| Business Purpose | [Purpose] |
| Business Definition | [Definition] |
| Business Meaning | [Meaning] |
| Unit | [Unit] |
| Source | [Source] |
| Question Supported | [Question] |
| Decision Supported | [Decision] |
| Action Supported | [Action] |
| Validation Rule | [Rule] |
| Example | [Example] |

---

## Signal Contract Validation

Every Signal Contract Must Define:

- Business Purpose
- Business Definition
- Business Meaning
- Unit
- Source
- Question Supported
- Decision Supported
- Action Supported
- Validation Rule

---

# STEP 06 — THRESHOLD MATRIX

## Threshold Design Guidance

Thresholds convert signals into decisions.

Every threshold should answer:

- What happened?
- Why does it matter?
- What should happen next?

---

## Threshold Matrix

| Signal | Threshold | Status | Business Meaning | Action |
|----------|----------|----------|----------|----------|
| [Signal] | [Threshold] | [Status] | [Meaning] | [Action] |

---

## Recommended Status Categories

### Healthy

Expected operating conditions.

### Warning

Requires monitoring.

### Critical

Requires immediate action.

---

## Threshold Validation

Every Threshold Must Define:

- Signal
- Threshold
- Status
- Business Meaning
- Action

---

# STEP 07 — END-TO-END TRACEABILITY

## Traceability Requirement

Every report element must be traceable.

Required Chain:

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

## Traceability Matrix

| Decision | Question | Signal | Threshold | Action | Story | Visual |
|----------|----------|----------|----------|----------|----------|----------|
| [Decision] | [Question] | [Signal] | [Threshold] | [Action] | [Story] | [Visual] |

---

## Traceability Validation

No orphan:

- Decisions
- Questions
- Signals
- Thresholds
- Actions
- Stories
- Visuals

allowed.

Every Question must map to:

- At Least One Signal
- At Least One Threshold
- At Least One Action

---

# STEP 08 — ACTION MATRIX

## Action Design Guidance

Actions define why the report exists.

Every Action Must:

- Support A Decision
- Support A Business Outcome
- Have A Responsible Role

---

## Action Matrix

| Condition | Recommended Action | Responsible Role | Expected Outcome | Decision Supported | Priority |
|----------|----------|----------|----------|----------|----------|
| [Condition] | [Action] | [Role] | [Outcome] | [Decision] | [Priority] |

---

## Action Validation

Every Action Must:

- Support A Decision
- Have An Owner
- Have An Expected Outcome
- Support A Business Outcome

---

# STEP 08A — BUSINESS RISKS

## Risk Assessment Purpose

Document business risks identified during decision analysis.

Risks should remain visible throughout report design.

---

## Risk Matrix

| Risk | Impact | Decision Affected | Mitigation |
|----------|----------|----------|----------|
| [Risk] | [Impact] | [Decision] | [Mitigation] |

---

## Risk Validation

Every Risk Must Define:

- Risk Description
- Business Impact
- Decision Affected
- Mitigation Strategy

Every Critical Risk should be represented by:

- A Question
- A Signal
- A Threshold
- An Action

where applicable.

---

# STEP 09 — STORY PLANNING MATRIX

## CRITICAL RULE

The output MUST generate all stories.

The output may NOT use:

- Repeat For All Stories
- Same Structure
- See Previous Story
- Same As Above

Every Story must be planned individually.

---

# STORY 0 — EXECUTIVE CONTEXT

## Business Question

[Question]

## Business Objective

[Objective]

## Audience

[Audience]

## Decision Supported

[Decision]

## User Action

[Action]

## Supporting Signals

[Signals]

## Success Outcome

[Outcome]

## Purpose

[Purpose]

## Primary Visual Candidate

[Visual]

---

# STORY 1 — ACTION REQUIRED

## Business Question

[Question]

## Business Objective

[Objective]

## Audience

[Audience]

## Decision Supported

[Decision]

## User Action

[Action]

## Supporting Signals

[Signals]

## Success Outcome

[Outcome]

## Purpose

[Purpose]

## Primary Visual Candidate

[Visual]

---

# STORY 2 — DECISION READINESS

## Business Question

[Question]

## Business Objective

[Objective]

## Audience

[Audience]

## Decision Supported

[Decision]

## User Action

[Action]

## Supporting Signals

[Signals]

## Success Outcome

[Outcome]

## Purpose

[Purpose]

## Primary Visual Candidate

[Visual]

---

# STORY 3 — DECISION BOARD

## Business Question

[Question]

## Business Objective

[Objective]

## Audience

[Audience]

## Decision Supported

[Decision]

## User Action

[Action]

## Supporting Signals

[Signals]

## Success Outcome

[Outcome]

## Purpose

[Purpose]

## Primary Visual Candidate

[Visual]

---

# STORY 4 — ANALYSIS

## Business Question

[Question]

## Business Objective

[Objective]

## Audience

[Audience]

## Decision Supported

[Decision]

## User Action

[Action]

## Supporting Signals

[Signals]

## Success Outcome

[Outcome]

## Purpose

[Purpose]

## Primary Visual Candidate

[Visual]

---

# STORY 5 — DATA TRUST

## Business Question

[Question]

## Business Objective

[Objective]

## Audience

[Audience]

## Decision Supported

[Decision]

## User Action

[Action]

## Supporting Signals

[Signals]

## Success Outcome

[Outcome]

## Purpose

[Purpose]

## Primary Visual Candidate

[Visual]

---

# STORY 6 — REGIONAL MONITORING

## Business Question

[Question]

## Business Objective

[Objective]

## Audience

[Audience]

## Decision Supported

[Decision]

## User Action

[Action]

## Supporting Signals

[Signals]

## Success Outcome

[Outcome]

## Purpose

[Purpose]

## Primary Visual Candidate

[Visual]

---

# STORY 7 — OPERATIONAL BRIEFING

## Business Question

[Question]

## Business Objective

[Objective]

## Audience

[Audience]

## Decision Supported

[Decision]

## User Action

[Action]

## Supporting Signals

[Signals]

## Success Outcome

[Outcome]

## Purpose

[Purpose]

## Primary Visual Candidate

[Visual]

---

## STORY VALIDATION

Minimum:

8 Stories Required

Every Story Must Define:

- Business Question
- Business Objective
- Audience
- Decision Supported
- User Action
- Supporting Signals
- Success Outcome
- Purpose
- Primary Visual Candidate

Every Story Must Answer:

- What is happening?
- Why is it important?
- What decision is supported?
- What action should occur?
- What successful outcome is expected?

---

# STEP 10 — PAGE ARCHETYPE

## Primary Archetype

[Primary Archetype]

Purpose:

[Purpose]

Core User:

[User]

---

## Secondary Archetype

[Secondary Archetype]

Purpose:

[Purpose]

Core User:

[User]

---

## Supporting Archetype

[Supporting Archetype]

Purpose:

[Purpose]

Core User:

[User]

---

## Archetype Validation

Every Archetype Must:

- Support The Primary Decision
- Support The Story Flow
- Support User Action

---

# STEP 11 — LAYOUT BLUEPRINT

## Required Reading Order

Story 0
↓
Story 1
↓
Story 2
↓
Story 3
↓
Story 4
↓
Story 5
↓
Story 6
↓
Story 7

---

## Layout Design Objective

The layout should guide users through:

Context
↓
Attention
↓
Decision
↓
Explanation
↓
Trust
↓
Action

---

## Layout Validation

The layout must support:

- Business Understanding
- Decision Making
- Action Taking

without requiring additional explanation.

---

# STEP 12 — VISUAL RECOMMENDATIONS

## CRITICAL RULE

Minimum:

8 Visual Recommendations

Required:

1 Primary Visual Recommendation per Story

---

## Visual Recommendation Template

| Field | Recommendation |
|---------|---------|
| Story | [Story] |
| Question Supported | [Question] |
| Decision Supported | [Decision] |
| Action Supported | [Action] |
| Visual Type | [Visual] |
| Reason | [Reason] |
| Data Source | [Signals] |
| Interaction | [Interaction] |

---

## Visual Validation

Every Visual Must Support:

- A Question
- A Decision
- A Signal
- A User Action

Visual selection should follow:

Decision
↓
Question
↓
Signal
↓
Action
↓
Visual

Never:

Visual
↓
Dashboard
↓
Decision

---

# STEP 13 — MARKDOWN WIREFRAME

## Draft Reading Order

Story 0 — Executive Context

Story 1 — Action Required

Story 2 — Decision Readiness

Story 3 — Decision Board

Story 4 — Analysis

Story 5 — Data Trust

Story 6 — Regional Monitoring

Story 7 — Operational Briefing

---

## Wireframe Validation

The wireframe should support:

Context
↓
Risk
↓
Decision
↓
Trust
↓
Action

---

# STEP 14 — SUCCESS CRITERIA

✅ [Success Criterion]

✅ [Success Criterion]

✅ [Success Criterion]

✅ [Success Criterion]

✅ [Success Criterion]

✅ [Success Criterion]

---

## User Validation

Users should be able to:

- Understand the situation
- Identify important risks
- Understand available options
- Trust the information
- Make decisions
- Take action

within:

30 Seconds

or an approved business duration.

---

# STEP 15 — VALIDATION CHECKLIST

## Decision Validation

☐ Primary Decision Defined

☐ Secondary Decisions Defined

☐ Decision Outcomes Defined

☐ Decision Success Criteria Defined

---

## Coverage Validation

☐ Operational Coverage

☐ Capacity Coverage

☐ Risk Coverage

☐ Governance Coverage

☐ Data Quality Coverage

☐ Regional Coverage

☐ Executive Coverage

---

## Question Validation

☐ Questions Defined

☐ Questions Support Decisions

☐ Questions Support Actions

---

## Signal Validation

☐ Signals Defined

☐ Signal Contracts Defined

☐ Signals Support Questions

☐ Signals Support Decisions

☐ Signals Support Actions

---

## Threshold Validation

☐ Thresholds Defined

☐ Business Meaning Defined

☐ Actions Defined

---

## Traceability Validation

☐ Decision Traceability Complete

☐ No Orphan Questions

☐ No Orphan Signals

☐ No Orphan Actions

☐ No Orphan Stories

☐ No Orphan Visuals

---

## Story Validation

☐ Story Coverage Complete

☐ All 8 Stories Defined

☐ Story Objectives Defined

☐ Story Success Outcomes Defined

☐ Visual Candidates Identified

---

## Design Validation

☐ Archetypes Defined

☐ Layout Defined

☐ Visual Recommendations Defined

---

# APPROVAL CHECKPOINT

☐ Decision Readiness

☐ Decision Model

☐ Coverage Discovery

☐ Business Questions

☐ Signal Matrix

☐ Signal Contracts

☐ Threshold Matrix

☐ Traceability

☐ Action Matrix

☐ Risk Review

☐ Story Planning

☐ Archetypes

☐ Layout

☐ Visual Recommendations

☐ Success Criteria

---

# MATRIX SUCCESS STATEMENT

A Decision Story Matrix succeeds when:

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
supports User Action

Every Visual
supports Business Action

while maintaining complete:

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

traceability.

The Matrix serves as the approved:

Decision Validation Contract

for creation of the:

REPORT_STORY (Decision Story Contract).