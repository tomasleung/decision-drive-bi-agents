# SKILL_BLUEPRINT.md

# Decision Story Agent Skill Blueprint

## Decision-Driven BI Agent Platform

Version: 1.0

Status: Approved

Blueprint Type: Agent Operating Specification

Agent:

Decision Story Agent

---

# PURPOSE

The Skill Blueprint defines how the Decision Story Agent operates.

The blueprint governs:

- Discovery
- Validation
- Reasoning
- Generation
- Approval Readiness
- Promotion

before runtime execution occurs.

The blueprint is the authoritative operating specification for the agent.

---

# AGENT MISSION

Transform:

```text
INPUT_BRD
```

into:

```text
REPORT_STORY_MATRIX

REPORT_STORY
```

through a governed decision-design process.

The agent exists to establish:

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
```

before implementation begins.

---

# GOVERNING AUTHORITIES

The agent operates under:

```text
Platform Coach Standard
↓
Decision-First Framework
↓
RDLC Governance
↓
Platform Architecture
↓
Repository Standards
↓
Skill Standards
↓
Decision Story Agent Blueprint
↓
Runtime Instructions
```

---

# AGENT LIFECYCLE

The Decision Story Agent follows:

```text
Discover
↓
Validate
↓
Reason
↓
Generate
↓
Validate
↓
Promote
```

No stage may be skipped.

---

# PHASE 01 — DISCOVER

## Purpose

Understand the business problem space.

---

## Inputs

```text
INPUT_BRD
```

---

## Activities

Identify:

- Business Problem
- Business Need
- Business Outcome
- Stakeholders
- Decisions
- Questions
- Signals
- Actions

---

## Output

```text
Discovery Assessment
```

---

# PHASE 02 — VALIDATE INPUT READINESS

## Purpose

Determine whether the BRD is sufficient.

---

## Readiness Checklist

Verify:

```text
Business Problem Defined

Decision Defined

Decision Owner Defined

Business Outcome Defined

Questions Defined

Stakeholders Defined

Success Criteria Defined
```

---

## Outcomes

Ready

or

Not Ready

---

## Failure Condition

If critical information is missing:

```text
STOP EXECUTION
```

Return readiness findings.

---

# PHASE 03 — DECISION DISCOVERY

## Purpose

Identify decision requirements.

---

## Deliverables

Identify:

```text
Primary Decision

Secondary Decisions

Decision Owners

Decision Outcomes
```

---

## Success Rule

Every decision must support:

```text
Business Outcome
```

---

# PHASE 04 — QUESTION DISCOVERY

## Purpose

Identify information requirements.

---

## Deliverables

Create:

```text
Decision
↓
Question
```

relationships.

---

## Validation Rule

Every question must support:

```text
A Decision
```

Questions without decision relevance are removed.

---

# PHASE 05 — SIGNAL DISCOVERY

## Purpose

Identify evidence requirements.

---

## Deliverables

Create:

```text
Question
↓
Signal
```

relationships.

---

## Validation Rule

Every signal must:

```text
Support A Question

Support A Decision
```

Signals without decision value are removed.

---

# PHASE 06 — THRESHOLD DISCOVERY

## Purpose

Identify action boundaries.

---

## Deliverables

Define:

```text
Signal
↓
Threshold
```

relationships.

---

## Validation Rule

Every threshold should support:

```text
Monitoring

Escalation

Intervention
```

---

# PHASE 07 — ACTION DISCOVERY

## Purpose

Identify operational responses.

---

## Deliverables

Define:

```text
Threshold
↓
Action
```

relationships.

---

## Validation Rule

Every action must support:

```text
Business Outcome
```

---

# PHASE 08 — STORY DISCOVERY

## Purpose

Translate decision logic into user-facing narrative.

---

## Deliverables

Define:

```text
Decision Story
```

including:

- Context
- Evidence
- Risks
- Opportunities
- Actions

---

## Validation Rule

Stories should support decision making.

Stories should not simply describe data.

---

# PHASE 09 — MATRIX GENERATION

## Purpose

Create the validation artifact.

---

## Output

```text
REPORT_STORY_MATRIX
```

---

## Matrix Coverage

Validate:

```text
Decision Coverage

Question Coverage

Signal Coverage

Threshold Coverage

Action Coverage

Story Coverage
```

---

## Key Question

```text
Do we fully understand the decision space?
```

---

# PHASE 10 — REPORT STORY GENERATION

## Purpose

Create the Decision Story Contract.

---

## Output

```text
REPORT_STORY
```

---

## Contract Contents

Include:

- Decision Logic
- Question Logic
- Signal Logic
- Threshold Logic
- Action Logic
- Story Logic
- Visual Direction

---

# VALIDATION MODEL

The agent performs four validation categories.

---

## Validation 01 — Decision Validation

Verify:

```text
All Required Decisions Identified
```

---

## Validation 02 — Coverage Validation

Verify:

```text
Decision Coverage

Question Coverage

Signal Coverage

Threshold Coverage

Action Coverage
```

---

## Validation 03 — Traceability Validation

Verify:

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
```

remains intact.

---

## Validation 04 — Handoff Validation

Verify downstream readiness.

Outputs should support:

```text
Mockup Agent

TRD Agent

Semantic Design Agent

Semantic Build Agent

Report Build Agent
```

without business rediscovery.

---

# PROMOTION RULES

REPORT_STORY_MATRIX may be promoted when:

```text
Coverage Complete

Validation Passed

Traceability Verified
```

---

REPORT_STORY may be promoted when:

```text
Decision Logic Approved

Story Logic Approved

Handoff Readiness Approved
```

---

# FAILURE CONDITIONS

Return findings without promotion when:

```text
Decision Missing

Decision Owner Missing

Business Outcome Missing

Question Coverage Incomplete

Signal Coverage Incomplete

Broken Traceability
```

---

# SUCCESS CRITERIA

The blueprint succeeds when:

```text
INPUT_BRD
```

can consistently produce:

```text
REPORT_STORY_MATRIX

REPORT_STORY
```

while preserving:

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
```

traceability.

---

# BLUEPRINT SUCCESS STATEMENT

The Decision Story Agent Skill Blueprint succeeds when a repeatable, governed lifecycle exists for transforming business requirements into decision-focused design artifacts before technical implementation begins.

The result is:

```text
Decision Products
```

not

```text
Reporting Products
```

---

# PROMOTION STATUS

Version:

1.0

Status:

APPROVED

Blueprint Type:

Agent Operating Specification

Lifecycle:

✅ Discover

✅ Validate

✅ Reason

✅ Generate

✅ Validate

✅ Promote

Outputs:

✅ REPORT_STORY_MATRIX

✅ REPORT_STORY

---

# NEXT ARTIFACT

skill.md

Purpose:

Define runtime execution instructions for AI platforms including:

- Copilot
- ChatGPT
- Claude
- Gemini
- Future Enterprise AI Platforms