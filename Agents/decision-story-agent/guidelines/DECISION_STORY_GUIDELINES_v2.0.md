# DECISION_STORY_GUIDELINES_v2.0

## Decision-Driven BI Decision Story Guidelines

---

# DOCUMENT METADATA

Document Name:
DECISION_STORY_GUIDELINES

Version:
2.0

Owner:
Decision-Driven BI Framework

Status:
Approved Guideline

Purpose:

Provide implementation guidance for converting a Business Requirements Document (BRD) into:

- REPORT_STORY_MATRIX
- REPORT_STORY (DSC)

These guidelines complement:

REPORT_DESIGN_STANDARDS_v2.0

The standards define:

What Good Looks Like

These guidelines define:

How To Apply Standards

---

# SECTION 01 — GUIDING PHILOSOPHY

## Decision First

Every report exists to support a business decision.

Always begin with:

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

Never begin with:

Visual
↓
Layout
↓
Dashboard
↓
Decision

---

## Action Before Reporting

The purpose of reporting is not information.

The purpose of reporting is:

Action

Every report section should improve a decision.

---

## Story Before Visuals

The decision story must be defined before visual selection begins.

Correct:

Decision
↓
Question
↓
Signal
↓
Action
↓
Story
↓
Visual

Incorrect:

Data
↓
Visual
↓
Dashboard

---

## Traceability First

Every artifact must support:

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

No orphan elements are allowed.

---

# SECTION 02 — INPUT USAGE GUIDELINES

## Required Input

INPUT_BRD_TEMPLATE_v1.0

---

## Gold Input Example

INPUT_BRD_AnimalFlow_LiveCapacity_v3.0

Purpose:

Demonstrates the expected quality and completeness of a Decision Story Agent input.

---

## Input Priority

1. Approved BRD
2. Business Owner Direction
3. Operational Documentation
4. Existing Reports
5. Existing Dashboards

Business intent remains the authoritative source.

---

# SECTION 03 — BRD ANALYSIS FRAMEWORK

## Purpose

Analyze the BRD before beginning Decision Story generation.

The objective is not to copy BRD content.

The objective is to discover:

- Decisions
- Questions
- Signals
- Actions
- Stories

---

## Analyze Business Summary

Identify:

- Business Goals
- Expected Benefits
- Desired Outcomes

Ask:

What business improvement is being requested?

---

## Analyze Business Problem

Identify:

- Pain Points
- Risks
- Operational Friction
- Visibility Gaps

Ask:

Why does this report need to exist?

---

## Analyze Current State

Identify:

- Current Process
- Existing Limitations
- Manual Activities

Ask:

What should become easier?

---

## Analyze Future State

Identify:

- Desired Capabilities
- Desired Decisions
- Desired User Experience

Ask:

What should become possible?

---

# SECTION 04 — DECISION DISCOVERY GUIDELINES

## Purpose

Decision discovery defines why the report exists.

---

## Primary Decision Discovery

Identify:

The most important decision supported by the report.

Ask:

What decision becomes easier after using this report?

---

## Secondary Decision Discovery

Identify:

Additional decisions that support:

- Operations
- Risk
- Governance
- Monitoring
- Leadership

---

## Decision Validation

Every decision must define:

- Decision Owner
- Decision Frequency
- Business Purpose
- Success Criteria

---

## Validation Rule

Every report must contain:

One clearly defined Primary Decision.

---

# SECTION 05 — QUESTION DISCOVERY GUIDELINES

## Purpose

Questions translate decisions into information needs.

---

## Explicit Question Discovery

Extract questions directly documented in the BRD.

---

## Implied Question Discovery

Identify questions implied by:

- Business Goals
- Business Problems
- Success Criteria
- Actions
- Signals

---

## Question Categories

Evaluate coverage across:

- Operational
- Capacity
- Risk
- Governance
- Data Quality
- Regional
- Executive

---

## Question Validation

Every question must:

- Support a Decision
- Be Actionable
- Be Business Relevant
- Be Measurable

---

## Avoid

Avoid:

- Curiosity Questions
- Interesting Questions
- Questions With No Action
- Questions With No Decision

---

# SECTION 06 — SIGNAL DISCOVERY GUIDELINES

## Purpose

Signals provide evidence used for decision making.

---

## Signal Discovery Process

Question
↓
Potential Signals
↓
Decision Signals
↓
Critical Signals

---

## Signal Classification

Classify signals as:

- Operational
- Capacity
- Risk
- Governance
- Data Quality
- Regional
- Executive

---

## Signal Validation

Every signal must:

- Support a Question
- Support a Decision
- Support an Action
- Be Measurable
- Be Explainable

---

## Avoid

Do not create:

- Vanity Metrics
- Decorative KPIs
- Orphan Signals

---

# SECTION 07 — THRESHOLD DESIGN GUIDELINES

## Purpose

Thresholds convert signals into action.

---

## Preferred Structure

Signal
↓
Threshold
↓
Status
↓
Action
↓
Business Meaning

---

## Required States

Every critical signal should define:

- Healthy
- Warning
- Critical

where applicable.

---

## Threshold Validation

Every threshold must answer:

What Happened?

Why Does It Matter?

What Should Be Done?

---

# SECTION 08 — ACTION DISCOVERY GUIDELINES

## Purpose

Actions define the operational purpose of reporting.

---

## Action Discovery Process

Decision
↓
Business Response
↓
Operational Action
↓
Expected Outcome

---

## Action Requirements

Every action should define:

- Condition
- Recommended Action
- Responsible Role
- Expected Outcome
- Decision Supported

---

## Validation Rule

Every action must support:

- Human Decision
- Human Response
- Business Outcome

---

# SECTION 09 — STORY DESIGN GUIDELINES

## Purpose

Convert business logic into a decision journey.

---

## Story Flow

Context
↓
Attention Required
↓
Decision Support
↓
Explanation
↓
Trust
↓
Action

---

## Story Validation

Every story should answer:

- What Is Happening?
- Why Is It Happening?
- What Requires Attention?
- What Decision Must Be Made?
- What Action Should Occur?

---

# SECTION 10 — STORY CONSTRUCTION FRAMEWORK

## Purpose

Provide a repeatable method for generating story sections.

---

## Story 0 — Executive Context

Purpose:

Provide high-level context.

Answer:

What is happening?

---

## Story 1 — Action Required

Purpose:

Highlight immediate concerns.

Answer:

What requires attention now?

---

## Story 2 — Decision Readiness

Purpose:

Determine whether action should occur.

Answer:

Are we ready to make a decision?

---

## Story 3 — Decision Board

Purpose:

Prioritize options.

Answer:

What should be prioritized?

---

## Story 4 — Analysis

Purpose:

Explain contributing factors.

Answer:

Why is this happening?

---

## Story 5 — Data Trust

Purpose:

Validate information quality.

Answer:

Can this information be trusted?

---

## Story 6 — Regional Monitoring

Purpose:

Identify geographic or organizational patterns.

Answer:

Where is pressure building?

---

## Story 7 — Operational Briefing

Purpose:

Summarize operational recommendations.

Answer:

What should happen next?

---

# SECTION 11 — PAGE ARCHETYPE GUIDELINES

## Purpose

Select an archetype aligned to business intent.

---

## Approved Archetypes

- Operational Command Centre
- Capacity Intelligence
- Executive Monitoring
- Exception Management
- Regional Monitoring
- Performance Monitoring
- Data Quality Investigation

---

## Selection Rule

Choose archetypes based on:

Business Decisions

not visual preferences.

---

# SECTION 12 — LAYOUT BLUEPRINT GUIDELINES

## Purpose

Define reading order.

---

## Preferred Flow

Context
↓
Analysis
↓
Decision
↓
Action

---

## Validation Rule

Users should not need to search for important content.

---

# SECTION 13 — VISUAL RECOMMENDATION GUIDELINES

## Purpose

Recommend visuals that support decisions.

---

## Preferred Selection Process

Decision
↓
Question
↓
Signal
↓
Action
↓
Visual

---

## Visual Validation

Every visual must support:

- Decision
- Question
- Signal
- Action

---

## Avoid

Avoid visuals that exist because:

- They Look Good
- They Are Popular
- They Were Used Previously

---

# SECTION 14 — TRACEABILITY GUIDELINES

## Purpose

Ensure full traceability across all artifacts.

---

## Required Mapping

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

- Decisions
- Questions
- Signals
- Thresholds
- Actions
- Stories
- Visuals

allowed.

---

# SECTION 15 — COVERAGE DISCOVERY GUIDELINES

## Purpose

Prevent blind spots during report design.

---

## Evaluate Coverage Across

- Operational
- Capacity
- Risk
- Governance
- Data Quality
- Regional
- Executive

---

## Validation Rule

If a category is relevant to the business problem but not represented in the design:

Create a review finding.

---

# SECTION 16 — AI READINESS GUIDELINES

## Documentation Requirements

Every documented element should explain:

- Why It Exists
- What It Supports
- What Decision It Serves

---

## AI Readiness Goal

An AI assistant should be able to explain:

- Why the report exists
- Why a question exists
- Why a signal exists
- Why an action exists

without reviewing additional documents.

---

# SECTION 17 — VALIDATION GUIDELINES

## Decision Validation

Verify:

□ Primary Decision Defined

□ Secondary Decisions Defined

□ Decision Owner Defined

□ Success Criteria Defined

---

## Question Validation

Verify:

□ Questions Defined

□ Questions Support Decisions

□ No Orphan Questions

---

## Signal Validation

Verify:

□ Signals Defined

□ Signals Support Questions

□ No Orphan Signals

---

## Action Validation

Verify:

□ Actions Defined

□ Actions Support Decisions

□ Responsible Roles Defined

---

## Story Validation

Verify:

□ Story Coverage Complete

□ Questions Answered

□ Actions Defined

□ Business Journey Present

---

## Traceability Validation

Verify:

□ Decision Traceability Complete

□ Question Traceability Complete

□ Signal Traceability Complete

□ Action Traceability Complete

---

# SECTION 18 — HANDOFF GUIDELINES

## REPORT_STORY_MATRIX

Output:

REPORT_STORY

---

## REPORT_STORY

Outputs To:

- Mockup Agent
- TRD Agent
- Semantic Design Agent

---

## Handoff Goal

Downstream agents should understand:

- Business Intent
- Decisions
- Questions
- Signals
- Actions
- Story Flow

without revisiting the BRD.

---

# SECTION 19 — COMMON DESIGN MISTAKES

Avoid:

- Starting With Visuals
- Starting With KPIs
- Questions Without Decisions
- Signals Without Questions
- Thresholds Without Actions
- Actions Without Decisions
- Stories Without Purpose
- Visuals Without Actionability
- Reporting Without Action

---

# GUIDELINE SUCCESS STATEMENT

Decision Story Design succeeds when:

Business Intent
↓
Decision Framework
↓
Question Design
↓
Signal Design
↓
Threshold Design
↓
Action Design
↓
Story Design
↓
Visual Design

remains fully traceable.

The result is:

- Decision Driven
- Question Driven
- Action Oriented
- Traceable
- Governed
- AI Ready

business design artifacts that can be confidently handed to:

- Mockup Agent
- TRD Agent
- Semantic Design Agent
- Report Build Agent