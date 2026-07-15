# DECISION_STORY_GUIDELINES_v1.0
## Decision-Driven BI Decision Story Guidelines

---

# Document Metadata

Document Name

```text
DECISION_STORY_GUIDELINES
```

Version

```text
1.0
```

Owner

```text
Decision-Driven BI Framework
```

Status

```text
Approved Guideline
```

Purpose

```text
Provide implementation guidance for creating
Decision Story artifacts within the
Decision-Driven BI Framework.
```

These guidelines complement:

```text
REPORT_DESIGN_STANDARDS_v1.0
```

and define:

```text
How To Discover Decisions

How To Design Questions

How To Design Signals

How To Create Stories

How To Create Layout Blueprints

How To Create Visual Recommendations

How To Validate Outputs

How To Handoff Outputs
```

---

# SECTION 01 — GUIDING PHILOSOPHY

## Decision First

The report exists to support decisions.

Always begin with:

```text
Decision

↓

Business Question

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
```

Never begin with:

```text
Visual

↓

Layout

↓

Dashboard

↓

Decision
```

---

## Action Before Reporting

The purpose of reporting is not information.

The purpose of reporting is:

```text
Action
```

Every report section should improve a decision.

---

## Story Before Visuals

The story must be approved before visual selection begins.

Correct:

```text
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
```

Incorrect:

```text
Data

↓

Visual

↓

Dashboard
```

---

## Traceability First

Every artifact must support traceability:

```text
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
```

No orphan content is allowed.

---

# SECTION 02 — INPUT USAGE GUIDELINES

## Required Inputs

Always use:

```text
INPUT_BRD_vX.X.md
```

---

## Required Information

The BRD should provide:

```text
Business Problem

Business Goals

Business Decisions

Business Questions

Stakeholders

Success Criteria
```

---

## Reference Inputs

Use when available:

```text
Existing Reports

Existing Dashboards

Business Process Documents

Operational Procedures
```

---

## Input Priority

```text
1. Approved BRD

2. Business Owner Direction

3. Operational Documentation

4. Existing Reports

5. Existing Dashboards
```

Business intent remains the authoritative source.

---

# SECTION 03 — DECISION MODELING GUIDELINES

## Purpose

The Decision Model defines why the report exists.

---

## Required Documentation

Document:

```text
Primary Decision

Secondary Decisions

Decision Owner

Decision Frequency

Decision Success Criteria
```

---

## Validation Rule

Every report must contain:

```text
One Clearly Defined Primary Decision
```

---

## Avoid

Avoid:

```text
Technical Decisions

Visual Decisions

Layout Decisions
```

before the business decision is understood.

---

# SECTION 04 — BUSINESS QUESTION GUIDELINES

## Purpose

Questions translate decisions into information needs.

---

## Question Structure

Questions should be:

```text
Business Focused

Action Oriented

Decision Aligned
```

---

## Validation Rule

Every Question Must Support:

```text
A Decision
```

---

## Avoid

Avoid:

```text
Interesting Questions

Curiosity Questions

Questions With No Action
```

---

# SECTION 05 — SIGNAL DESIGN GUIDELINES

## Purpose

Signals tell users what they should monitor.

---

## Signal Requirements

Signals should:

```text
Support Questions

Support Decisions

Support Actions
```

---

## Validation Rule

Every Signal Must Support:

```text
Question

↓

Decision
```

---

## Avoid

Do not create:

```text
Orphan Signals
```

---

# SECTION 06 — THRESHOLD GUIDELINES

## Purpose

Thresholds translate signals into action.

---

## Preferred Pattern

```text
Signal

↓

Threshold

↓

Status

↓

Action

↓

Decision
```

---

## Required Documentation

Document:

```text
Healthy State

Warning State

Critical State

Recommended Action
```

---

## Avoid

Avoid thresholds without actions.

---

# SECTION 07 — ACTION DESIGN GUIDELINES

## Purpose

Actions define why reporting exists.

---

## Action Requirements

Actions should be:

```text
Specific

Practical

Operational

Observable
```

---

## Validation Rule

Every Action Must Support:

```text
A Decision
```

---

## Avoid

Avoid actions that are:

```text
Vague

Unclear

Unmeasurable
```

---

# SECTION 08 — STORY DESIGN GUIDELINES

## Purpose

Convert business logic into a decision journey.

---

## Recommended Story Flow

```text
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
```

---

## Story Requirements

Every story section should answer:

```text
A Business Question
```

---

## Story Validation

A user should understand:

```text
What Is Happening

Why It Matters

What Requires Attention

What Decision Must Be Made

What Action Should Occur
```

---

# SECTION 09 — PAGE ARCHETYPE GUIDELINES

## Purpose

Select a design pattern aligned to business intent.

---

## Common Archetypes

```text
Operational Command Centre

Capacity Intelligence

Executive Monitoring

Exception Management

Regional Monitoring

Performance Monitoring

Data Quality Investigation
```

---

## Selection Rule

Choose archetypes based on:

```text
Business Decisions
```

not visual preferences.

---

# SECTION 10 — LAYOUT BLUEPRINT GUIDELINES

## Purpose

Define reading order.

---

## Preferred Layout Flow

```text
Context

↓

Analysis

↓

Decision

↓

Action
```

---

## Validation Rule

Users should not need to search for important content.

---

# SECTION 11 — VISUAL RECOMMENDATION GUIDELINES

## Purpose

Recommend visuals that support the story.

---

## Preferred Pattern

```text
Question

↓

Signal

↓

Visual
```

---

## Visual Selection Rule

Every visual must support:

```text
Decision

Question

Signal

Action
```

---

## Avoid

Avoid visuals that exist only because:

```text
They Look Good

They Are Popular

They Were Used Previously
```

---

# SECTION 12 — AI READINESS GUIDELINES

## Documentation Requirements

Every documented element should explain:

```text
Why It Exists

What It Supports

What Decision It Serves
```

---

## Decision Documentation

Document:

```text
Business Purpose

Owner

Success Criteria
```

---

## Question Documentation

Document:

```text
Business Purpose

Decision Supported
```

---

## Signal Documentation

Document:

```text
Business Purpose

Question Supported

Decision Supported
```

---

## AI Readiness Goal

An AI assistant should be able to explain:

```text
Why the report exists

Why a question exists

Why a signal exists

What action should occur
```

without reading additional documents.

---

# SECTION 13 — VALIDATION GUIDELINES

## Decision Validation

Verify:

```text
□ Primary Decision Defined

□ Secondary Decisions Defined

□ Decision Owner Defined

□ Success Criteria Defined
```

---

## Question Validation

Verify:

```text
□ Questions Defined

□ Questions Support Decisions

□ No Orphan Questions
```

---

## Signal Validation

Verify:

```text
□ Signals Defined

□ Signals Support Questions

□ No Orphan Signals
```

---

## Story Validation

Verify:

```text
□ Story Flow Defined

□ Questions Answered

□ Actions Defined

□ Business Journey Present
```

---

# SECTION 14 — HANDOFF GUIDELINES

## REPORT_STORY_MATRIX

Output:

```text
REPORT_STORY
```

---

## REPORT_STORY

Outputs To:

```text
Mockup Agent

TRD Agent
```

---

## Handoff Goal

Downstream agents should understand:

```text
Business Intent

Business Decisions

Questions

Signals

Actions

Story Flow
```

without revisiting the BRD.

---

# SECTION 15 — COMMON DESIGN MISTAKES

Avoid:

```text
Starting With Visuals

Starting With KPIs

Questions Without Decisions

Signals Without Questions

Thresholds Without Actions

Stories Without Decisions

Visuals Without Purpose

Reporting Without Action
```

---

# GUIDELINE SUCCESS STATEMENT

Decision Story Design succeeds when:

```text
Business Intent

↓

Decision Framework

↓

Question Design

↓

Signal Design

↓

Action Design

↓

Story Design
```

remains fully traceable.

The result is:

```text
Decision-Driven

Question-Driven

Action-Oriented

AI-Ready

Business Design Artifacts
```

that can be confidently handed to:

```text
Mockup Agent

TRD Agent

Semantic Design Agent

Report Build Agent
```