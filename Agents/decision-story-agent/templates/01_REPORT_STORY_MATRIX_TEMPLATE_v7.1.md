# REPORT_STORY_MATRIX_TEMPLATE_v7.1

## Decision Story Matrix

### Decision-Driven BI Framework

---

# DOCUMENT METADATA

Document Type:

Decision Story Matrix

Version:

7.1

Status:

Approved

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
- Business Outcomes
- Handoff Readiness
- Design Readiness

before detailed report design begins.

---

# PLATFORM ALIGNMENT

This template is governed by:

```text
Platform Coach Standard

Decision-First Framework

RDLC Governance

Platform Architecture

Decision Story Standards

Decision Story Handoff Contract
```

The Matrix serves as the official:

```text
Decision Validation Contract
```

for downstream business design activities.

---

# AUDIENCE

- Product Owner
- Business Owner
- Decision Owner
- Report Designer
- BI Developer
- Data Architect
- Solution Architect
- Governance Reviewers

---

# APPROVAL GATE

This artifact must be approved before creation of the:

```text
REPORT_STORY (DSC)
```

No downstream design work should begin before Matrix approval.

---

# WRITER GUIDANCE

This template is a business-first artifact.

The purpose is not to design a report.

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
- Outcome Focused

---

## Matrix Purpose

Validate:

```text
Business Problem

Decision Design

Question Design

Signal Design

Action Design

Business Outcomes

Story Design Readiness
```

Not:

```text
Report Design

Visual Design

Technical Design
```

Those belong to downstream phases.

---

## Framework Rule

```text
No Decision
↓
No Artifact
```

Every section should improve:

- Decision Clarity
- Business Coverage
- Traceability
- Actionability
- Story Quality
- Business Outcome Alignment

---

# STEP 00 — DECISION READINESS CHECK

## Input Validation

| Readiness Item | Status |
|---------------|---------|
| Primary Decision Defined | PASS / FAIL |
| Decision Owner Defined | PASS / FAIL |
| Secondary Decisions Defined | PASS / FAIL |
| Business Questions Defined | PASS / FAIL |
| Signals Defined | PASS / FAIL |
| KPI Contracts Defined | PASS / FAIL |
| Action Model Defined | PASS / FAIL |
| Stakeholders Defined | PASS / FAIL |
| Success Criteria Defined | PASS / FAIL |
| Business Outcomes Defined | PASS / FAIL |

---

## Readiness Score

[Score]

---

## Readiness Result

READY

or

RETURN TO DISCOVERY

---

## Readiness Notes

Document:

- Missing Information
- Assumptions
- Discovery Risks
- Readiness Concerns

---

# STEP 00A — FOUNDATION REVIEW

## Purpose

Validate that the correct business problem is being solved before decision modeling begins.

This section aligns the Matrix with the Platform Coach Standard.

---

## Business Problem

What problem are we solving?

[Business Problem]

---

## Business Capability

What capability is being created?

[Capability Description]

---

## Decision Outcome

What business outcome improves if the solution succeeds?

[Business Outcome]

---

## Decision Failure Impact

What happens if the decision is made incorrectly?

[Impact Description]

---

## Assumptions

List key assumptions.

- [Assumption]
- [Assumption]
- [Assumption]

---

## Foundation Risks

Identify foundational risks.

| Risk | Impact | Mitigation |
|--------|--------|--------|
| [Risk] | [Impact] | [Mitigation] |

---

## Foundation Validation

Verify:

☐ Business Problem Clearly Defined

☐ Capability Clearly Defined

☐ Business Outcome Defined

☐ Decision Impact Defined

☐ Assumptions Documented

☐ Foundation Risks Documented

---

# STEP 01 — DECISION MODEL

## Primary Decision

[Primary Decision]

---

## Business Purpose

[Business Purpose]

---

## Decision Owner

[Decision Owner]

---

## Decision Authority

Decision authority belongs to:

[Responsible Owner]

---

## Decision Frequency

[Frequency]

Examples:

- Real Time
- Hourly
- Daily
- Weekly
- Monthly
- Quarterly

---

## Governing Business Rule

[Business Rule]

Example:

```text
Capacity
+
Eligibility
+
Data Trust
=
Placement Readiness
```

---

## Key Discovery

[Key Discovery]

---

## Decision Success Criteria

Users must answer:

[Primary Business Question]

within:

[Target Time]

---

## Business Outcome

The decision should improve:

[Business Outcome]

Examples:

- Capacity Optimization
- Risk Reduction
- Faster Response
- Cost Reduction
- Service Improvement
- Operational Visibility

---

## Secondary Decisions

Minimum:

5 Required

- [Secondary Decision 01]
- [Secondary Decision 02]
- [Secondary Decision 03]
- [Secondary Decision 04]
- [Secondary Decision 05]

---

## Decision Outcomes

- [Outcome 01]
- [Outcome 02]
- [Outcome 03]
- [Outcome 04]
- [Outcome 05]

---

## Human Authority Validation

AI may:

- Recommend Decisions
- Analyze Decisions
- Validate Decision Logic

AI may not:

- Approve Business Decisions
- Approve Governance
- Approve Decision Ownership

Human approval remains mandatory.

---

## Decision Model Validation

☐ Primary Decision Defined

☐ Decision Owner Defined

☐ Decision Authority Defined

☐ Business Purpose Defined

☐ Business Outcome Defined

☐ Decision Success Criteria Defined

☐ Secondary Decisions Defined

☐ Outcome Alignment Verified

---
# STEP 02 — COVERAGE DISCOVERY MATRIX

## Purpose

Validate that the decision space has been explored sufficiently before business design begins.

Coverage discovery ensures no critical business domain is omitted.

The objective is to identify:

- Missing Questions
- Missing Signals
- Missing Actions
- Missing Risks
- Missing Business Outcomes

before downstream design activities begin.

---

## Coverage Discovery Matrix

| Domain | Covered | Questions | Signals | Actions | Evidence |
|----------|----------|----------|----------|----------|----------|
| Operational | YES / NO | [#] | [#] | [#] | [Evidence] |
| Capacity | YES / NO | [#] | [#] | [#] | [Evidence] |
| Risk | YES / NO | [#] | [#] | [#] | [Evidence] |
| Governance | YES / NO | [#] | [#] | [#] | [Evidence] |
| Data Quality | YES / NO | [#] | [#] | [#] | [Evidence] |
| Regional | YES / NO | [#] | [#] | [#] | [Evidence] |
| Executive | YES / NO | [#] | [#] | [#] | [Evidence] |

---

## Coverage Validation

All relevant business domains must be evaluated.

No critical domain may be omitted without documented justification.

For omitted domains document:

Reason:

[Reason]

Impact:

[Impact]

Approval:

[Approver]

---

## Coverage Gaps

Document known gaps.

| Gap | Impact | Mitigation | Owner |
|--------|--------|--------|--------|
| [Gap] | [Impact] | [Mitigation] | [Owner] |

---

## Coverage Outcome Validation

Verify:

☐ Operational Coverage Evaluated

☐ Risk Coverage Evaluated

☐ Governance Coverage Evaluated

☐ Data Quality Coverage Evaluated

☐ Regional Coverage Evaluated

☐ Executive Coverage Evaluated

☐ Coverage Gaps Documented

☐ Mitigation Defined

---

# STEP 03 — BUSINESS QUESTION MATRIX

## Purpose

Define the business questions required to support decision making.

Questions establish information requirements.

Questions should be discovered before:

- Metrics
- KPIs
- Measures
- Visuals

are discussed.

---

## Question Design Principles

Every question must:

```text
Support A Decision

Support A Signal

Support A Story

Support An Action

Support A Business Outcome
```

Questions without decision relevance are not permitted.

---

## Minimum Coverage Requirements

Questions should be evaluated across:

- Operational Monitoring
- Capacity Management
- Risk Management
- Governance
- Data Trust
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

## Question-to-Outcome Mapping

Every critical question should identify:

| Question | Decision | Action | Business Outcome |
|-----------|-----------|-----------|-----------|
| [Question] | [Decision] | [Action] | [Outcome] |

---

## Question Validation

Minimum:

```text
10 Questions Required
```

Recommended:

```text
15+ Questions
```

Every Question Must:

☐ Support A Decision

☐ Support A Signal

☐ Support A Story

☐ Support A User Action

☐ Support A Business Outcome

☐ Have Clear Business Purpose

---

## Question Quality Review

Review each question for:

```text
Clarity

Relevance

Actionability

Decision Support Value

Outcome Contribution
```

Questions that do not materially influence a decision should be removed.

---

# STEP 04 — SIGNAL MATRIX

## Purpose

Define the signals required to answer business questions and support decisions.

Signals provide evidence.

Signals are not collected because data exists.

Signals exist because decisions require evidence.

---

## Signal Group Guidance

Signal Groups organize business monitoring and decision support.

Every Signal Group Must Define:

- Business Purpose
- Supported Decisions
- Supported Questions
- Supported Actions
- Supported Business Outcomes
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

### Supported Business Outcomes

[Outcomes]

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

### Supported Business Outcomes

[Outcomes]

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

### Supported Business Outcomes

[Outcomes]

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

### Supported Business Outcomes

[Outcomes]

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

### Supported Business Outcomes

[Outcomes]

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

### Supported Business Outcomes

[Outcomes]

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

### Supported Business Outcomes

[Outcomes]

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

### Supported Business Outcomes

[Outcomes]

### Critical Signals

- [Signal]
- [Signal]

---

## Signal Validation

Every Signal Must:

☐ Support A Question

☐ Support A Decision

☐ Support An Action

☐ Support A Business Outcome

☐ Be Measurable

☐ Be Explainable

☐ Be Actionable

Every Signal Group Must:

☐ Have Business Purpose

☐ Have Supported Decisions

☐ Have Supported Questions

☐ Have Supported Actions

☐ Have Supported Outcomes

---

# STEP 05 — SIGNAL CONTRACTS

## Purpose

Signal Contracts provide business definitions for critical signals.

The objective is to ensure stakeholders understand:

- Why the signal exists
- What the signal means
- What decisions it supports
- What actions it influences

without reviewing technical documentation.

Signal Contracts translate data into business understanding.

---

## Critical Rule

Signal Contracts are required for all critical signals.

Critical signals should be understandable by:

- Business Owners
- Decision Owners
- Report Designers
- BI Developers
- Executives

without requiring technical interpretation.

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
| Business Outcome Supported | [Outcome] |
| Validation Rule | [Rule] |
| Example | [Example] |

---

## Signal Contract Validation

Every Signal Contract Must Define:

☐ Business Purpose

☐ Business Definition

☐ Business Meaning

☐ Unit

☐ Source

☐ Question Supported

☐ Decision Supported

☐ Action Supported

☐ Business Outcome Supported

☐ Validation Rule

---

## Signal Governance Review

Verify:

☐ Signal Is Business Relevant

☐ Signal Supports Decision Making

☐ Signal Supports Action

☐ Signal Supports Business Outcome

☐ Signal Has Clear Ownership

☐ Signal Is Explainable

---

# STEP 06 — THRESHOLD MATRIX

## Purpose

Thresholds transform signals into operational decisions.

Thresholds define when:

- Attention Is Required
- Escalation Is Required
- Intervention Is Required
- Action Should Occur

Signals provide evidence.

Thresholds drive responses.

---

## Threshold Design Guidance

Every threshold should answer:

```text
What happened?

Why does it matter?

What should happen next?
```

Every threshold should support:

```text
Decision Making

Business Action

Business Outcomes
```

---

## Threshold Matrix

| Signal | Threshold | Status | Business Meaning | Action |
|----------|----------|----------|----------|----------|
| [Signal] | [Threshold] | [Status] | [Meaning] | [Action] |

---

## Recommended Status Categories

### Healthy

Expected operating conditions.

No intervention required.

---

### Warning

Attention recommended.

Monitoring required.

Potential intervention planning begins.

---

### Critical

Immediate attention required.

Intervention expected.

Escalation may be required.

---

## Threshold-to-Outcome Mapping

| Threshold | Action | Business Outcome |
|-----------|-----------|-----------|
| [Threshold] | [Action] | [Outcome] |

---

## Threshold Validation

Every Threshold Must Define:

☐ Signal

☐ Threshold

☐ Status

☐ Business Meaning

☐ Action

☐ Business Outcome

Every Threshold Must Support:

☐ A Decision

☐ A User Response

☐ A Business Outcome

---

## Threshold Governance Review

Verify:

☐ Threshold Is Understandable

☐ Threshold Supports Action

☐ Threshold Supports Business Outcome

☐ Escalation Logic Exists

☐ Status Categories Defined

---

# STEP 07 — END-TO-END TRACEABILITY

## Purpose

Ensure complete traceability across the Decision Story lifecycle.

Every report element should be traceable back to a business need.

Traceability is mandatory.

Not optional.

---

## Required Traceability Chain

```text
Business Problem
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
↓
Business Outcome
```

No orphan elements permitted.

---

## Traceability Matrix

| Business Problem | Decision | Question | Signal | Threshold | Action | Story | Visual | Business Outcome |
|----------|----------|----------|----------|----------|----------|----------|----------|----------|
| [Value] | [Value] | [Value] | [Value] | [Value] | [Value] | [Value] | [Value] | [Value] |

---

## Traceability Rules

Every Decision must map to:

☐ At Least One Question

☐ At Least One Business Outcome

---

Every Question must map to:

☐ At Least One Signal

☐ At Least One Action

---

Every Signal must map to:

☐ At Least One Threshold

☐ At Least One Decision

---

Every Threshold must map to:

☐ At Least One Action

☐ At Least One Outcome

---

Every Story must map to:

☐ At Least One Decision

☐ At Least One Question

☐ At Least One Signal

☐ At Least One Business Outcome

---

Every Visual must map to:

☐ At Least One Story

☐ At Least One Decision

☐ At Least One User Action

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
- Outcomes

allowed.

---

## Traceability Quality Review

Verify:

☐ Decision Traceability Complete

☐ Signal Traceability Complete

☐ Action Traceability Complete

☐ Story Traceability Complete

☐ Business Outcome Traceability Complete

☐ No Orphan Elements Exist

---

# STEP 08 — ACTION MATRIX

## Purpose

Actions define why the report exists.

The purpose of reporting is not information.

The purpose of reporting is:

```text
Business Action
```

Actions convert:

```text
Insights
↓
Decisions
↓
Business Outcomes
```

Every approved action should contribute to a measurable business outcome.

---

## Action Design Guidance

Every action should answer:

```text
What should happen?

Who should take action?

Why is action required?

What outcome is expected?
```

Actions should be:

- Specific
- Actionable
- Accountable
- Measurable
- Outcome Focused

---

## Action Contract Template

Condition:

[Condition]

Recommended Action:

[Action]

Responsible Role:

[Role]

Decision Supported:

[Decision]

Priority:

[Priority]

Expected Outcome:

[Outcome]

Business Impact:

[Impact]

Escalation Required:

YES / NO

Escalation Path:

[Escalation Path]

---

## Action Matrix

| Condition | Recommended Action | Responsible Role | Decision Supported | Expected Outcome | Priority |
|------------|------------|------------|------------|------------|------------|
| [Condition] | [Action] | [Role] | [Decision] | [Outcome] | [Priority] |

---

## Action-to-Outcome Mapping

| Action | Outcome | Success Indicator |
|----------|----------|----------|
| [Action] | [Outcome] | [Indicator] |

---

## Action Validation

Every Action Must Define:

☐ Condition

☐ Recommended Action

☐ Responsible Role

☐ Decision Supported

☐ Expected Outcome

☐ Business Impact

☐ Escalation Requirement

☐ Success Indicator

---

## Action Governance Review

Verify:

☐ Action Supports A Decision

☐ Action Supports A Business Outcome

☐ Accountability Is Defined

☐ Business Impact Is Clear

☐ Escalation Path Exists Where Appropriate

---

# STEP 08A — BUSINESS RISKS

## Purpose

Document business risks identified during decision analysis.

Risks should remain visible throughout:

```text
Decision Design

Business Design

Technical Design

Semantic Design

Implementation
```

The objective is to reduce decision failure risk.

---

## Risk Matrix

| Risk | Impact | Decision Affected | Mitigation |
|----------|----------|----------|----------|
| [Risk] | [Impact] | [Decision] | [Mitigation] |

---

## Risk Register

### Risk 01

Risk Description:

[Risk]

Business Impact:

[Impact]

Decision Affected:

[Decision]

Signal Used To Monitor Risk:

[Signal]

Mitigation Strategy:

[Mitigation]

Owner:

[Owner]

---

### Risk 02

Risk Description:

[Risk]

Business Impact:

[Impact]

Decision Affected:

[Decision]

Signal Used To Monitor Risk:

[Signal]

Mitigation Strategy:

[Mitigation]

Owner:

[Owner]

---

## Risk Validation

Every Risk Must Define:

☐ Risk Description

☐ Business Impact

☐ Decision Affected

☐ Mitigation Strategy

☐ Risk Owner

Every Critical Risk Should Be Represented By:

☐ Question

☐ Signal

☐ Threshold

☐ Action

where applicable.

---

## Risk Traceability

Every Critical Risk should trace to:

```text
Business Problem
↓
Decision
↓
Question
↓
Signal
↓
Action
↓
Mitigation
```

---

# STEP 08B — REGRESSION & DECISION RISK REVIEW

## Purpose

Evaluate risks introduced by:

- Missing Signals
- Weak Questions
- Incorrect Assumptions
- Incomplete Coverage
- Poor Decision Design

This section aligns with the Platform Coach Standard's Regression Analysis capability.

---

## Decision Failure Analysis

Identify:

### Failure Mode 01

Decision:

[Decision]

Potential Failure:

[Failure]

Root Cause:

[Cause]

Business Impact:

[Impact]

Mitigation:

[Mitigation]

---

### Failure Mode 02

Decision:

[Decision]

Potential Failure:

[Failure]

Root Cause:

[Cause]

Business Impact:

[Impact]

Mitigation:

[Mitigation]

---

## Assumption Risk Review

| Assumption | Risk If Incorrect | Severity | Mitigation |
|------------|------------|------------|------------|
| [Assumption] | [Risk] | High / Medium / Low | [Mitigation] |

---

## Missing Information Risk Review

| Missing Item | Impact | Severity | Action Required |
|------------|------------|------------|------------|
| [Item] | [Impact] | High / Medium / Low | [Action] |

---

## Regression Protection Review

Verify:

☐ Existing Business Rules Preserved

☐ Existing Decision Logic Preserved

☐ Existing Governance Requirements Preserved

☐ Existing Traceability Preserved

☐ Existing Business Outcomes Preserved

☐ Existing User Actions Preserved

---

## Decision Risk Validation

Verify:

☐ Failure Modes Evaluated

☐ Mitigation Strategies Defined

☐ Assumption Risks Documented

☐ Potential Decision Failures Identified

☐ Business Impact Assessed

☐ Risk Owners Identified

---

## Risk Outcome Summary

Document:

### Highest Risk

[Risk]

### Highest Impact Decision

[Decision]

### Highest Priority Mitigation

[Mitigation]

### Overall Risk Rating

Low / Medium / High

---

## Coach Alignment Validation

Verify:

☐ Problem Framing Complete

☐ Foundation Analysis Complete

☐ Assumptions Reviewed

☐ Failure Modes Reviewed

☐ Strategic Risks Identified

☐ Regression Risks Reviewed

---
# STEP 09 — STORY PLANNING MATRIX

## Purpose

Transform validated decision logic into business stories.

Stories are the mechanism through which:

```text
Business Problems

become

Business Understanding

which enables

Decision Making

which enables

Business Action
```

Stories should explain:

- What is happening
- Why it matters
- What decision is required
- What action should occur
- What outcome should be achieved

---

## CRITICAL STORY RULE

The output MUST generate all stories.

The output may NOT use:

- Repeat For All Stories
- Same As Above
- Same Structure
- See Previous Story

Every Story must be planned individually.

---

## STORY SUCCESS RULE

Every Story Must Support:

```text
Decision
↓
Action
↓
Business Outcome
```

A story that does not support action should be removed.

A story that does not support a business outcome should be redesigned.

---

# STORY 0 — EXECUTIVE CONTEXT

## Business Question

[Question]

---

## Business Objective

[Objective]

---

## Audience

[Audience]

---

## Decision Supported

[Decision]

---

## User Action

[Action]

---

## Supporting Signals

[Signals]

---

## Business Outcome

[Outcome]

---

## Success Outcome

[Outcome]

---

## Purpose

[Purpose]

---

## Primary Visual Candidate

[Visual]

---

# STORY 1 — ACTION REQUIRED

## Business Question

[Question]

---

## Business Objective

[Objective]

---

## Audience

[Audience]

---

## Decision Supported

[Decision]

---

## User Action

[Action]

---

## Supporting Signals

[Signals]

---

## Business Outcome

[Outcome]

---

## Success Outcome

[Outcome]

---

## Purpose

[Purpose]

---

## Primary Visual Candidate

[Visual]

---

# STORY 2 — DECISION READINESS

## Business Question

[Question]

---

## Business Objective

[Objective]

---

## Audience

[Audience]

---

## Decision Supported

[Decision]

---

## User Action

[Action]

---

## Supporting Signals

[Signals]

---

## Business Outcome

[Outcome]

---

## Success Outcome

[Outcome]

---

## Purpose

[Purpose]

---

## Primary Visual Candidate

[Visual]

---

# STORY 3 — DECISION BOARD

## Business Question

[Question]

---

## Business Objective

[Objective]

---

## Audience

[Audience]

---

## Decision Supported

[Decision]

---

## User Action

[Action]

---

## Supporting Signals

[Signals]

---

## Business Outcome

[Outcome]

---

## Success Outcome

[Outcome]

---

## Purpose

[Purpose]

---

## Primary Visual Candidate

[Visual]

---

# STORY 4 — ANALYSIS

## Business Question

[Question]

---

## Business Objective

[Objective]

---

## Audience

[Audience]

---

## Decision Supported

[Decision]

---

## User Action

[Action]

---

## Supporting Signals

[Signals]

---

## Business Outcome

[Outcome]

---

## Success Outcome

[Outcome]

---

## Purpose

[Purpose]

---

## Primary Visual Candidate

[Visual]

---

# STORY 5 — DATA TRUST

## Business Question

[Question]

---

## Business Objective

[Objective]

---

## Audience

[Audience]

---

## Decision Supported

[Decision]

---

## User Action

[Action]

---

## Supporting Signals

[Signals]

---

## Business Outcome

[Outcome]

---

## Success Outcome

[Outcome]

---

## Purpose

[Purpose]

---

## Primary Visual Candidate

[Visual]

---

# STORY 6 — REGIONAL MONITORING

## Business Question

[Question]

---

## Business Objective

[Objective]

---

## Audience

[Audience]

---

## Decision Supported

[Decision]

---

## User Action

[Action]

---

## Supporting Signals

[Signals]

---

## Business Outcome

[Outcome]

---

## Success Outcome

[Outcome]

---

## Purpose

[Purpose]

---

## Primary Visual Candidate

[Visual]

---

# STORY 7 — OPERATIONAL BRIEFING

## Business Question

[Question]

---

## Business Objective

[Objective]

---

## Audience

[Audience]

---

## Decision Supported

[Decision]

---

## User Action

[Action]

---

## Supporting Signals

[Signals]

---

## Business Outcome

[Outcome]

---

## Success Outcome

[Outcome]

---

## Purpose

[Purpose]

---

## Primary Visual Candidate

[Visual]

---

## STORY VALIDATION

Minimum:

```text
8 Stories Required
```

Every Story Must Define:

☐ Business Question

☐ Business Objective

☐ Audience

☐ Decision Supported

☐ User Action

☐ Supporting Signals

☐ Business Outcome

☐ Success Outcome

☐ Purpose

☐ Primary Visual Candidate

---

Every Story Must Answer:

```text
What is happening?

Why is it important?

What decision is supported?

What action should occur?

What successful outcome is expected?
```

---

Every Story Must Support:

```text
At Least One Decision

At Least One Action

At Least One Business Outcome
```

---

# STEP 10 — PAGE ARCHETYPE

## Purpose

Define the report design pattern most appropriate for supporting the primary decision.

Archetypes should be selected based on:

- Business Purpose
- Decision Requirements
- User Needs
- Operational Context

Not:

- Personal Preference
- Previous Report Designs
- Visual Preferences

---

## Primary Archetype

[Primary Archetype]

Purpose:

[Purpose]

Core User:

[User]

Decision Supported:

[Decision]

Business Outcome Supported:

[Outcome]

---

## Secondary Archetype

[Secondary Archetype]

Purpose:

[Purpose]

Core User:

[User]

Decision Supported:

[Decision]

Business Outcome Supported:

[Outcome]

---

## Supporting Archetype

[Supporting Archetype]

Purpose:

[Purpose]

Core User:

[User]

Decision Supported:

[Decision]

Business Outcome Supported:

[Outcome]

---

## Archetype Validation

Every Archetype Must:

☐ Support The Primary Decision

☐ Support Story Flow

☐ Support User Action

☐ Support Business Outcomes

☐ Support Traceability

---

# STEP 11 — LAYOUT BLUEPRINT

## Required Reading Order

```text
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
```

---

## Layout Design Objective

The layout should guide users through:

```text
Context
↓
Attention
↓
Decision
↓
Evidence
↓
Trust
↓
Action
↓
Business Outcome
```

---

## Information Priority Model

### Level 01 — Immediate Attention

Examples:

- Critical Risks
- Escalations
- Action Required
- Operational Exceptions

---

### Level 02 — Decision Support

Examples:

- Recommendations
- Prioritization
- Readiness
- Performance Status

---

### Level 03 — Analysis

Examples:

- Trends
- Root Causes
- Variance Analysis
- Performance Drivers

---

### Level 04 — Trust

Examples:

- Data Quality
- Freshness
- Validation Status
- Governance Metrics

---

## Layout Validation

The layout must support:

☐ Business Understanding

☐ Decision Making

☐ Risk Identification

☐ Business Trust

☐ Business Action

☐ Outcome Achievement

without requiring additional explanation.

---

# STEP 12 — VISUAL RECOMMENDATIONS

## Purpose

Describe how business information should be communicated visually.

Visuals exist to support:

```text
Business Problem
↓
Decision
↓
Question
↓
Signal
↓
Action
↓
Business Outcome
```

Visuals do not exist for presentation purposes alone.

Every visual should justify its existence through business value.

---

## Visual Selection Principles

Visual selection should prioritize:

- Decision Support
- Actionability
- Clarity
- Interpretability
- Cognitive Simplicity
- Business Outcomes

Avoid visual selection based on:

- Popularity
- Personal Preference
- Previous Report Design
- Visual Complexity

---

## Visual Recommendation Template

| Field | Recommendation |
|---------|---------|
| Story | [Story] |
| Question Supported | [Question] |
| Decision Supported | [Decision] |
| Action Supported | [Action] |
| Business Outcome Supported | [Outcome] |
| Visual Type | [Visual] |
| Reason | [Reason] |
| Data Source | [Signals] |
| Interaction | [Interaction] |

---

## Story 0 Visual Recommendation

Story:

Executive Context

Question Supported:

[Question]

Decision Supported:

[Decision]

Business Outcome Supported:

[Outcome]

Visual Type:

[Visual]

Reason:

[Reason]

---

## Story 1 Visual Recommendation

Story:

Action Required

Question Supported:

[Question]

Decision Supported:

[Decision]

Business Outcome Supported:

[Outcome]

Visual Type:

[Visual]

Reason:

[Reason]

---

## Story 2 Visual Recommendation

Story:

Decision Readiness

Question Supported:

[Question]

Decision Supported:

[Decision]

Business Outcome Supported:

[Outcome]

Visual Type:

[Visual]

Reason:

[Reason]

---

## Story 3 Visual Recommendation

Story:

Decision Board

Question Supported:

[Question]

Decision Supported:

[Decision]

Business Outcome Supported:

[Outcome]

Visual Type:

[Visual]

Reason:

[Reason]

---

## Story 4 Visual Recommendation

Story:

Analysis

Question Supported:

[Question]

Decision Supported:

[Decision]

Business Outcome Supported:

[Outcome]

Visual Type:

[Visual]

Reason:

[Reason]

---

## Story 5 Visual Recommendation

Story:

Data Trust

Question Supported:

[Question]

Decision Supported:

[Decision]

Business Outcome Supported:

[Outcome]

Visual Type:

[Visual]

Reason:

[Reason]

---

## Story 6 Visual Recommendation

Story:

Regional Monitoring

Question Supported:

[Question]

Decision Supported:

[Decision]

Business Outcome Supported:

[Outcome]

Visual Type:

[Visual]

Reason:

[Reason]

---

## Story 7 Visual Recommendation

Story:

Operational Briefing

Question Supported:

[Question]

Decision Supported:

[Decision]

Business Outcome Supported:

[Outcome]

Visual Type:

[Visual]

Reason:

[Reason]

---

## Visual Validation

Every Visual Must Support:

☐ A Business Question

☐ A Decision

☐ A Signal

☐ An Action

☐ A Business Outcome

☐ Story Objectives

---

## Visual Governance Rule

Visual selection should follow:

```text
Decision
↓
Question
↓
Signal
↓
Action
↓
Business Outcome
↓
Visual
```

Never:

```text
Visual
↓
Dashboard
↓
Decision
```

---

# STEP 13 — MARKDOWN WIREFRAME

## Purpose

Create a high-level layout blueprint before detailed mockup design begins.

The wireframe exists to validate:

- Story Sequencing
- Information Hierarchy
- User Attention Flow
- Decision Flow

before visual design occurs.

---

## Draft Reading Order

```text
Story 0 — Executive Context

Story 1 — Action Required

Story 2 — Decision Readiness

Story 3 — Decision Board

Story 4 — Analysis

Story 5 — Data Trust

Story 6 — Regional Monitoring

Story 7 — Operational Briefing
```

---

## User Journey

The expected user journey should follow:

```text
Situation
↓
Risk
↓
Decision
↓
Evidence
↓
Trust
↓
Action
↓
Outcome
```

---

## Wireframe Structure

### Section 01

Executive Context

Purpose:

Establish current business conditions.

---

### Section 02

Action Required

Purpose:

Surface immediate risks and required interventions.

---

### Section 03

Decision Readiness

Purpose:

Assess whether sufficient conditions exist to proceed.

---

### Section 04

Decision Board

Purpose:

Present available options and prioritization guidance.

---

### Section 05

Analysis

Purpose:

Provide supporting evidence and insights.

---

### Section 06

Data Trust

Purpose:

Validate confidence in information being consumed.

---

### Section 07

Regional Monitoring

Purpose:

Highlight location-based variances and risk concentrations.

---

### Section 08

Operational Briefing

Purpose:

Summarize recommended actions and operational priorities.

---

## Wireframe Validation

The wireframe should support:

☐ Context Understanding

☐ Risk Identification

☐ Decision Making

☐ Trust Validation

☐ Action Taking

☐ Outcome Achievement

without requiring additional explanation.

---

## Outcome Validation

Users should be able to:

```text
Understand The Situation
↓
Identify The Risk
↓
Evaluate The Options
↓
Make A Decision
↓
Take Action
↓
Improve The Business Outcome
```

---

# STEP 14 — SUCCESS CRITERIA

## Purpose

Define how matrix success will be evaluated before promotion.

Success criteria should describe measurable business outcomes.

---

## Business Success

✅ [Business Success Criterion]

✅ [Business Success Criterion]

✅ [Business Success Criterion]

✅ [Business Success Criterion]

---

## Decision Success

✅ [Decision Success Criterion]

✅ [Decision Success Criterion]

✅ [Decision Success Criterion]

✅ [Decision Success Criterion]

---

## Operational Success

✅ [Operational Success Criterion]

✅ [Operational Success Criterion]

✅ [Operational Success Criterion]

✅ [Operational Success Criterion]

---

## Governance Success

✅ Traceability Preserved

✅ Decision Coverage Complete

✅ Signal Coverage Complete

✅ Action Coverage Complete

✅ Outcome Coverage Complete

---

## User Success

Users should be able to:

- Understand the Situation
- Identify Important Risks
- Understand Available Options
- Trust the Information
- Make Decisions
- Take Action

within:

[Target Time]

---

## Outcome Success

The solution should improve:

- Decision Quality
- Response Speed
- Operational Effectiveness
- Risk Visibility
- Business Outcomes

---

## Success Validation

Verify:

☐ Business Success Criteria Defined

☐ Decision Success Criteria Defined

☐ Operational Success Criteria Defined

☐ User Success Criteria Defined

☐ Outcome Success Criteria Defined

---

# STEP 14A — HANDOFF READINESS

## Purpose

Validate that the Decision Story Matrix contains sufficient information to support downstream design activities.

Downstream agents should not need to perform:

```text
Business Rediscovery
```

to understand:

- Decision Intent
- Business Logic
- Signal Design
- Action Requirements
- Story Design Direction

---

## Mockup Readiness

The Mockup Agent should understand:

☐ Primary Decision

☐ Secondary Decisions

☐ Story Priorities

☐ User Actions

☐ Information Hierarchy

☐ Business Outcomes

☐ Visual Direction

☐ User Attention Requirements

Status:

READY / NOT READY

---

## TRD Readiness

The TRD Agent should understand:

☐ Business Logic

☐ Decision Logic

☐ Signal Definitions

☐ Threshold Logic

☐ Action Logic

☐ Data Expectations

☐ Business Rules

☐ Constraints

Status:

READY / NOT READY

---

## Semantic Design Readiness

The Semantic Design Agent should understand:

☐ Questions

☐ Signals

☐ Thresholds

☐ Required Metrics

☐ Business Definitions

☐ Outcome Expectations

☐ Traceability Requirements

Status:

READY / NOT READY

---

## Report Build Readiness

The Report Build Agent should understand:

☐ Stories

☐ Reading Order

☐ Layout Intent

☐ Visual Recommendations

☐ User Actions

☐ Desired Outcomes

Status:

READY / NOT READY

---

## Handoff Validation

Verify:

☐ Business Context Complete

☐ Decision Context Complete

☐ Question Coverage Complete

☐ Signal Coverage Complete

☐ Action Coverage Complete

☐ Story Coverage Complete

☐ Outcome Coverage Complete

☐ Traceability Complete

---

## Overall Handoff Result

READY FOR DSC DEVELOPMENT

or

RETURN FOR REVISION

---

# STEP 15 — VALIDATION CHECKLIST

## Purpose

Perform final quality validation before Matrix approval.

This checklist should serve as the final governance review before promotion.

---

## Foundation Validation

☐ Business Problem Defined

☐ Capability Defined

☐ Business Outcome Defined

☐ Decision Impact Defined

☐ Assumptions Documented

☐ Foundation Risks Documented

---

## Decision Validation

☐ Primary Decision Defined

☐ Decision Owner Defined

☐ Decision Authority Defined

☐ Decision Success Criteria Defined

☐ Business Outcomes Defined

☐ Secondary Decisions Defined

☐ Outcome Alignment Verified

---

## Human Authority Validation

☐ Decision Owner Identified

☐ Approval Authority Identified

☐ Human Accountability Assigned

☐ Governance Ownership Defined

☐ AI Recommendations Distinguished From Human Decisions

---

## Coverage Validation

☐ Operational Coverage

☐ Capacity Coverage

☐ Risk Coverage

☐ Governance Coverage

☐ Data Quality Coverage

☐ Regional Coverage

☐ Executive Coverage

☐ Coverage Gaps Reviewed

---

## Question Validation

☐ Questions Defined

☐ Questions Support Decisions

☐ Questions Support Signals

☐ Questions Support Actions

☐ Questions Support Business Outcomes

---

## Signal Validation

☐ Signals Defined

☐ Signal Contracts Defined

☐ Signals Support Questions

☐ Signals Support Decisions

☐ Signals Support Actions

☐ Signals Support Business Outcomes

---

## Threshold Validation

☐ Thresholds Defined

☐ Business Meaning Defined

☐ Actions Defined

☐ Outcomes Defined

---

## Action Validation

☐ Actions Defined

☐ Responsible Roles Defined

☐ Business Impacts Defined

☐ Expected Outcomes Defined

☐ Escalation Paths Defined

---

## Traceability Validation

☐ Business Problem Traceability

☐ Decision Traceability

☐ Question Traceability

☐ Signal Traceability

☐ Threshold Traceability

☐ Action Traceability

☐ Story Traceability

☐ Visual Traceability

☐ Outcome Traceability

☐ No Orphan Elements

---

## Risk Validation

☐ Risks Defined

☐ Mitigation Strategies Defined

☐ Failure Modes Evaluated

☐ Assumption Risks Evaluated

☐ Regression Risks Evaluated

---

## Story Validation

☐ Story 0 Complete

☐ Story 1 Complete

☐ Story 2 Complete

☐ Story 3 Complete

☐ Story 4 Complete

☐ Story 5 Complete

☐ Story 6 Complete

☐ Story 7 Complete

☐ Story Objectives Defined

☐ Story Outcomes Defined

☐ Visual Candidates Identified

---

## Design Validation

☐ Archetypes Defined

☐ Layout Defined

☐ Visual Recommendations Defined

☐ User Journey Defined

☐ Business Outcomes Supported

---

## Handoff Validation

☐ Mockup Ready

☐ TRD Ready

☐ Semantic Ready

☐ Report Build Ready

---

## Governance Validation

☐ Standards Compliant

☐ Traceability Complete

☐ Decision-First Compliant

☐ Human Authority Preserved

☐ Governance Requirements Met

---

# APPROVAL CHECKPOINT

## Decision Approval

☐ Decision Model Approved

☐ Business Outcomes Approved

☐ Decision Ownership Approved

---

## Business Approval

☐ Business Questions Approved

☐ Signal Design Approved

☐ Threshold Design Approved

☐ Action Design Approved

---

## Story Approval

☐ Story Planning Approved

☐ Story Coverage Approved

☐ Outcome Coverage Approved

---

## Governance Approval

☐ Traceability Approved

☐ Validation Passed

☐ Standards Compliance Confirmed

☐ Handoff Readiness Confirmed

---

## Human Approval Requirement

AI may:

```text
Analyze

Validate

Recommend
```

AI may not:

```text
Approve

Authorize

Promote
```

Final approval requires:

```text
Human Review
↓
Human Approval
↓
Promotion Decision
```

---

## Approval Result

APPROVED

or

RETURN FOR REVISION

---

# MATRIX PROMOTION DECISION

## Promotion Review

The Decision Story Matrix may only be promoted after:

```text
Decision Validation Complete
↓
Coverage Validation Complete
↓
Signal Validation Complete
↓
Threshold Validation Complete
↓
Action Validation Complete
↓
Risk Review Complete
↓
Story Planning Complete
↓
Traceability Complete
↓
Handoff Readiness Complete
↓
Approval Complete
```

---

## Promotion Checklist

☐ Foundation Review Complete

☐ Decision Model Complete

☐ Business Outcomes Defined

☐ Coverage Discovery Complete

☐ Questions Approved

☐ Signals Approved

☐ Signal Contracts Approved

☐ Threshold Design Approved

☐ Action Design Approved

☐ Risk Review Approved

☐ Regression Risk Review Complete

☐ Story Planning Approved

☐ Archetypes Approved

☐ Layout Blueprint Approved

☐ Visual Recommendations Approved

☐ Success Criteria Approved

☐ Traceability Complete

☐ Handoff Readiness Complete

☐ Validation Checklist Passed

☐ Approval Checkpoint Passed

---

## Promotion Authority

The following roles may participate in review:

- Product Owner
- Business Owner
- Decision Owner
- Data Owner
- Solution Architect
- Governance Reviewer

Promotion authority remains with designated human approvers.

---

## Promotion Result

Status:

```text
APPROVED

or

REJECTED
```

---

## Promotion Notes

Document:

- Outstanding Risks
- Outstanding Assumptions
- Approved Exceptions
- Follow-Up Actions

[Promotion Notes]

---

# MATRIX QUALITY SCORECARD

## Purpose

Provide a standardized quality assessment before promotion.

---

## Scoring Categories

### Foundation Quality

Score:

[0-10]

Criteria:

- Problem Defined
- Outcomes Defined
- Assumptions Reviewed
- Risks Identified

---

### Decision Quality

Score:

[0-10]

Criteria:

- Decision Clarity
- Ownership Clarity
- Outcome Alignment
- Business Value

---

### Coverage Quality

Score:

[0-10]

Criteria:

- Domain Coverage
- Question Coverage
- Signal Coverage
- Action Coverage

---

### Story Quality

Score:

[0-10]

Criteria:

- Story Completeness
- Story Relevance
- User Action Support
- Outcome Support

---

### Traceability Quality

Score:

[0-10]

Criteria:

- End-To-End Mapping
- No Orphan Elements
- Business Alignment
- Governance Alignment

---

### Handoff Quality

Score:

[0-10]

Criteria:

- Mockup Readiness
- TRD Readiness
- Semantic Readiness
- Build Readiness

---

## Overall Score

| Category | Score |
|----------|----------|
| Foundation Quality | [Score] |
| Decision Quality | [Score] |
| Coverage Quality | [Score] |
| Story Quality | [Score] |
| Traceability Quality | [Score] |
| Handoff Quality | [Score] |

---

### Total Score

[Score]

out of

60

---

### Overall Assessment

50 - 60

```text
Production Ready
```

---

40 - 49

```text
Ready With Minor Revisions
```

---

30 - 39

```text
Requires Significant Revision
```

---

Below 30

```text
Return To Discovery
```

---

# HUMAN AUTHORITY CERTIFICATION

## Governance Rule

AI may:

- Analyze
- Discover
- Validate
- Recommend
- Generate

AI may not:

- Approve Decisions
- Approve Governance
- Approve Promotion
- Approve Business Outcomes

---

## Human Certification

Decision Owner:

[Name]

Approval Status:

APPROVED / REJECTED

Date:

[Date]

---

Business Owner:

[Name]

Approval Status:

APPROVED / REJECTED

Date:

[Date]

---

Governance Reviewer:

[Name]

Approval Status:

APPROVED / REJECTED

Date:

[Date]

---

# MATRIX SUCCESS STATEMENT

A Decision Story Matrix succeeds when:

Every Business Problem

supports a Decision

Every Decision

supports Questions

Every Question

supports Signals

Every Signal

supports Thresholds

Every Threshold

supports Actions

Every Action

supports Stories

Every Story

supports Visual Direction

Every Visual

supports Business Outcomes

while maintaining complete:

```text
Business Problem
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
↓
Business Outcome
```

traceability.

The Matrix serves as the official:

```text
Decision Validation Contract
```

for creation of the:

```text
REPORT_STORY

(Decision Story Contract)
```

---

# HANDOFF RESULT

Upon approval the Matrix becomes eligible for progression to:

```text
REPORT_STORY_TEMPLATE_v7.1
```

and serves as the governing input for creation of the:

```text
Decision Story Contract (DSC)
```

---

# PLATFORM ALIGNMENT VERIFICATION

This template aligns with:

✅ PLATFORM_COACH_STANDARD_v1.1

✅ FRAMEWORK_README_v1.2

✅ DECISION_DRIVEN_BI_ARCHITECTURE_v3.2

✅ DECISION_STORY_HANDOFF_CONTRACT_v1.0

✅ Decision-First Operating System

✅ RDLC Governance Operating System

✅ Human Authority Principle

✅ Traceability Model

✅ Regression Protection Model

---

# PROMOTION CRITERIA

The Matrix may be promoted when:

☐ Foundation Review Complete

☐ Decision Readiness Complete

☐ Business Outcomes Defined

☐ Coverage Discovery Complete

☐ Question Coverage Approved

☐ Signal Design Approved

☐ Signal Contracts Approved

☐ Threshold Design Approved

☐ Action Design Approved

☐ Business Risk Review Complete

☐ Regression Risk Review Complete

☐ Story Planning Approved

☐ Traceability Complete

☐ Visual Planning Complete

☐ Handoff Readiness Complete

☐ Validation Checklist Passed

☐ Approval Checkpoint Passed

☐ Human Approval Received

☐ Quality Score Meets Minimum Threshold

---

## Promotion Status

```text
APPROVED

or

REJECTED
```

---

# DOCUMENT STATUS

Document:

REPORT_STORY_MATRIX_TEMPLATE_v7.1

Status:

APPROVED

Template Type:

Decision Validation Contract

Lifecycle Position:

```text
Business Discovery
↓
Decision Validation
↓
Business Design
```

Purpose:

```text
Validate Decision Thinking

Before Business Design Begins
```

Next Artifact:

```text
REPORT_STORY_TEMPLATE_v7.1
```