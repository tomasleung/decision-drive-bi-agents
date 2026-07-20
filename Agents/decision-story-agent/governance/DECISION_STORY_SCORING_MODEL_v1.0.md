# DECISION_STORY_SCORING_MODEL_v1.0

## Purpose

Define the official scoring model used by the:

```text
Decision Story Review Agent

Decision Story Governance Process

Promotion Gates

Template Evolution Process
```

to evaluate:

```text
REPORT_STORY_MATRIX

REPORT_STORY
```

against:

```text
DECISION_STORY_GOLD_OUTPUT_SPEC_v1.0

DECISION_STORY_REVIEW_CRITERIA_v1.0
```

---

# Scoring Philosophy

The score is intended to measure:

```text
Decision Quality

Business Coverage

Traceability

Storytelling Effectiveness

Actionability

Governance Readiness
```

The objective is NOT to reward:

```text
Length

Complexity

Technical Detail
```

The objective IS to reward:

```text
Decision Support

Business Clarity

Traceability

User Action
```

---

# Total Score

```text
100 Points
```

---

# DOMAIN 01
# DECISION MODEL

Weight:

```text
10 Points
```

---

## Criteria

### Primary Decision Defined

```text
2 Points
```

---

### Secondary Decisions Defined

```text
2 Points
```

---

### Decision Owner Defined

```text
1 Point
```

---

### Decision Frequency Defined

```text
1 Point
```

---

### Governing Business Rule Defined

```text
2 Points
```

---

### Success Criteria Defined

```text
2 Points
```

---

# DOMAIN 02
# BUSINESS QUESTION COVERAGE

Weight:

```text
15 Points
```

---

## Criteria

### Question Count

Minimum:

```text
10 Questions
```

Score:

```text
5 Points
```

---

### Question Categories Present

Required:

```text
Placement

Operations

Data Quality

Governance

Regional Monitoring
```

Score:

```text
5 Points
```

---

### Questions Support Decisions

Score:

```text
5 Points
```

---

# DOMAIN 03
# SIGNAL DESIGN

Weight:

```text
10 Points
```

---

## Criteria

### Signal Groups Defined

Score:

```text
3 Points
```

---

### Signal Coverage Complete

Score:

```text
4 Points
```

---

### Signals Support Questions

Score:

```text
3 Points
```

---

# DOMAIN 04
# SIGNAL CONTRACTS

Weight:

```text
15 Points
```

---

## Criteria

### Business Purpose Defined

```text
2 Points
```

---

### Business Definition Defined

```text
2 Points
```

---

### Unit Defined

```text
2 Points
```

---

### Source Defined

```text
2 Points
```

---

### Question Supported Defined

```text
3 Points
```

---

### Decision Supported Defined

```text
2 Points
```

---

### Validation Rule Defined

```text
2 Points
```

---

# DOMAIN 05
# THRESHOLD DESIGN

Weight:

```text
10 Points
```

---

## Criteria

### Threshold Defined

```text
2 Points
```

---

### Status Defined

```text
2 Points
```

---

### Action Defined

```text
2 Points
```

---

### Business Meaning Defined

```text
4 Points
```

---

# DOMAIN 06
# DECISION TRACEABILITY

Weight:

```text
10 Points
```

---

## Criteria

### Traceability Matrix Present

```text
2 Points
```

---

### Question → Signal Mapping

```text
3 Points
```

---

### Signal → Threshold Mapping

```text
2 Points
```

---

### Threshold → Action Mapping

```text
3 Points
```

---

# DOMAIN 07
# ACTION MATRIX

Weight:

```text
5 Points
```

---

## Criteria

### Conditions Defined

```text
2 Points
```

---

### Actions Defined

```text
1 Point
```

---

### Responsible Roles Defined

```text
2 Points
```

---

# DOMAIN 08
# STORY COVERAGE

Weight:

```text
15 Points
```

---

## Criteria

### Minimum Eight Stories

Required:

```text
Story 0

Story 1

Story 2

Story 3

Story 4

Story 5

Story 6

Story 7
```

Score:

```text
5 Points
```

---

### Story Flow Complete

Required:

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

Score:

```text
5 Points
```

---

### Story Purpose Clearly Defined

Score:

```text
5 Points
```

---

# DOMAIN 09
# STORY QUALITY

Weight:

```text
5 Points
```

---

## Criteria

Every Story Includes:

```text
Question

Output

Audience

Action

Supporting Signals

Decision Supported

Purpose
```

Score:

```text
5 Points
```

---

# DOMAIN 10
# PAGE ARCHETYPE

Weight:

```text
2 Points
```

---

## Criteria

### Archetypes Defined

Required:

```text
Primary

Secondary

Supporting
```

Score:

```text
2 Points
```

---

# DOMAIN 11
# LAYOUT BLUEPRINT

Weight:

```text
3 Points
```

---

## Criteria

### Reading Order Present

```text
1 Point
```

---

### Supports Context → Analysis → Decision → Action

```text
2 Points
```

---

# DOMAIN 12
# VISUAL RECOMMENDATIONS

Weight:

```text
8 Points
```

---

## Criteria

### Minimum Eight Visual Recommendations

```text
3 Points
```

---

### Visual Supports Story

```text
2 Points
```

---

### Reason Defined

```text
1 Point
```

---

### Data Source Defined

```text
1 Point
```

---

### Interaction Defined

```text
1 Point
```

---

# DOMAIN 13
# MARKDOWN WIREFRAME

Weight:

```text
1 Point
```

---

## Criteria

### Wireframe Present

```text
1 Point
```

---

# DOMAIN 14
# SUCCESS CRITERIA

Weight:

```text
1 Point
```

---

## Criteria

### Success Criteria Defined

```text
1 Point
```

---

# PROMOTION THRESHOLDS

## GOLD STANDARD

```text
95 – 100
```

Characteristics:

```text
Complete

Fully Traceable

Story Rich

Decision Driven

Promotion Ready
```

Recommendation:

```text
Promote Immediately
```

---

## APPROVED

```text
90 – 94
```

Characteristics:

```text
Minor Improvements Only

No Critical Gaps
```

Recommendation:

```text
Approve
```

---

## CONDITIONAL APPROVAL

```text
80 – 89
```

Characteristics:

```text
Good

Usable

Requires Minor Revision
```

Recommendation:

```text
Approve With Revisions
```

---

## REVISION REQUIRED

```text
70 – 79
```

Characteristics:

```text
Partial Coverage

Missing Sections

Weak Traceability
```

Recommendation:

```text
Revise Before Promotion
```

---

## REJECT

```text
Below 70
```

Characteristics:

```text
Major Gaps

Missing Coverage

Broken Story Design

Broken Traceability
```

Recommendation:

```text
Regenerate
```

---

# CRITICAL FAILURE RULES

The following conditions automatically prevent promotion regardless of score.

---

## Critical Failure 01

Missing Primary Decision

Result:

```text
Automatic Fail
```

---

## Critical Failure 02

Missing Decision Traceability

Result:

```text
Automatic Fail
```

---

## Critical Failure 03

Less Than Eight Stories

Result:

```text
Automatic Fail
```

---

## Critical Failure 04

Missing Signal Contracts

Result:

```text
Automatic Fail
```

---

## Critical Failure 05

No Action Matrix

Result:

```text
Automatic Fail
```

---

## Critical Failure 06

Missing Visual Recommendations

Result:

```text
Automatic Fail
```

---

# REVIEW OUTPUT FORMAT

The Review Agent will generate:

```text
Decision Model Score

Business Question Score

Signal Score

Signal Contract Score

Threshold Score

Traceability Score

Action Score

Story Coverage Score

Story Quality Score

Visual Score

Layout Score

Overall Score
```

---

# FINAL REVIEW OUTPUT

```text
Overall Score

Promotion Recommendation

Critical Findings

Major Findings

Minor Findings

Root Cause Analysis

Template Improvement Opportunities
```

---

# SCORING MODEL SUCCESS STATEMENT

The scoring model succeeds when it:

```text
Rewards Decision Quality

Rewards Business Coverage

Rewards Traceability

Rewards Storytelling

Rewards Actionability
```

while preventing promotion of artifacts that are:

```text
Incomplete

Non-Traceable

Weakly Structured

Not Decision Focused
```