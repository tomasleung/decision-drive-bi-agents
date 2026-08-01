# Decision Story Agent

## Decision-Driven BI Agent Platform

Version: 1.1

Status: Approved

Repository Type: Platform Agent Repository

Purpose:

Provide the entry point, navigation guide, and repository overview for the Decision Story Agent.

This README explains:

- Why the repository exists
- What the agent does
- Repository contents
- How to navigate the repository
- Recommended read order
- How the agent fits into the platform lifecycle
- How outputs are generated and promoted

---

# Repository Purpose

The Decision Story Agent is the first operational agent within the Decision-Driven BI Agent Platform.

The agent transforms:

Business Requirements

into

Decision Design Artifacts

before technical implementation begins.

The agent is responsible for converting:

```text
INPUT_BRD
```

into:

```text
REPORT_STORY_MATRIX

REPORT_STORY
```

through a governed and traceable process.

---

# Agent Mission

The Decision Story Agent exists to answer:

```text
What decisions require support?

What questions must be answered?

What signals matter?

What actions should occur?

What story should the solution communicate?
```

before asking:

```text
What should the report look like?
```

---

# Repository Structure

```text
decision-story-agent/

├── inputs/
│
├── standards/
│
├── guidelines/
│
├── templates/
│
├── contracts/
│
├── governance/
│
├── outputs/
│
├── test-run/
│
├── PROJECT_INIT.md
│
├── README.md
│
├── AGENT_README.md
│
├── SKILL_BLUEPRINT.md
│
├── skill.md
│
└── CHANGELOG.md
```

---

# Repository Components

---

## PROJECT_INIT.md

Purpose:

Repository Constitution

Answers:

```text
Why does this repository exist?

What mission does it support?

What problem does it solve?
```

---

## README.md

Purpose:

Repository Navigation

Answers:

```text
What exists in this repository?

How should contributors navigate?

Where should execution begin?
```

---

## AGENT_README.md

Purpose:

Agent Overview

Answers:

```text
What is the Decision Story Agent?

What are its responsibilities?

What are its inputs and outputs?
```

---

## SKILL_BLUEPRINT.md

Purpose:

Agent Operating Specification

Answers:

```text
How does the agent operate?

What lifecycle stages exist?

What validations exist?

How does promotion occur?
```

---

## skill.md

Purpose:

Runtime Instructions

Answers:

```text
What should the AI execute?

What actions occur at runtime?
```

---

## inputs/

Purpose:

Input Contracts and Business Inputs

Contains:

```text
INPUT_BRD_TEMPLATE

INPUT_BRD_*
```

Answers:

```text
What information is required?

What business problem should be solved?
```

---

## standards/

Purpose:

Design Standards

Answers:

```text
What Good Looks Like?

What must be designed?
```

Examples:

```text
REPORT_DESIGN_STANDARDS
```

---

## guidelines/

Purpose:

Execution Guidance

Answers:

```text
How should standards be applied?

How should decisions be discovered?

How should stories be designed?
```

Examples:

```text
DECISION_STORY_GUIDELINES
```

---

## templates/

Purpose:

Output Contracts

Answers:

```text
How should outputs be structured?

Which sections are required?
```

Examples:

```text
01_REPORT_STORY_MATRIX_TEMPLATE

02_REPORT_STORY_TEMPLATE
```

---

## governance/

Purpose:

Quality Governance

Answers:

```text
What Good Looks Like?

How are outputs reviewed?

How are outputs scored?
```

Examples:

```text
DECISION_STORY_GOLD_OUTPUT_SPEC

DECISION_STORY_REVIEW_CRITERIA

DECISION_STORY_SCORING_MODEL
```

---

## test-run/

Purpose:

Execution Workspace

Answers:

```text
Where are generated outputs stored?

How are test runs isolated?

How are validation runs tracked?

How are outputs reviewed?
```

Each execution should create a dedicated test run folder.

Example:

```text
test-run/

└── Test_Run_01_AnimalFlow/
```

Expected Contents:

```text
REPORT_STORY_MATRIX

REPORT_STORY
```

Additional artifacts may include:

```text
Execution Notes

Validation Findings

Review Notes
```

Test runs should never overwrite previous executions.

---

## outputs/

Purpose:

Promoted Deliverables

Answers:

```text
Which outputs have been reviewed?

Which outputs have been approved?

Which outputs are available for downstream agents?
```

Expected Contents:

```text
REPORT_STORY_MATRIX

REPORT_STORY
```

Outputs should only be placed here after review and approval.

---

# Agent Lifecycle Position

The Decision Story Agent is the first operational platform agent.

Platform Flow:

```text
INPUT_BRD
↓
Decision Story Agent
↓
REPORT_STORY_MATRIX
↓
REPORT_STORY
↓
Mockup Agent
↓
TRD Agent
↓
Semantic Design Agent
↓
Semantic Build Agent
↓
Report Build Agent
```

---

# Inputs

Primary Inputs:

```text
INPUT_BRD
```

Supporting Inputs:

```text
INPUT_BRD_TEMPLATE

Platform Standards

Platform Guidelines

Governance Artifacts

Output Templates
```

---

# Outputs

Primary Outputs:

```text
REPORT_STORY_MATRIX

REPORT_STORY
```

The outputs become governing business design artifacts used by downstream agents.

---

# Output Promotion Model

Generated outputs follow:

```text
Generate
↓
test-run/
↓
Review
↓
Approval
↓
outputs/
```

Outputs remain working artifacts until promotion.

Downstream agents should consume promoted artifacts whenever possible.

---

# Questions Answered

The Decision Story Agent answers:

```text
What business problem requires support?

What business capability is being improved?

What business outcomes matter?

What decisions must be made?

Who owns the decision?

What business questions exist?

What signals matter?

What thresholds matter?

What actions should occur?

What story should be communicated?
```

---

# Agent Responsibilities

The agent is responsible for:

- Decision Discovery
- Question Discovery
- Signal Discovery
- Threshold Design
- Action Design
- Story Design
- Coverage Validation
- Traceability Validation

The agent is not responsible for:

- UX Design
- Visual Mockups
- Technical Design
- Data Modeling
- Semantic Design
- Report Construction

These responsibilities belong to downstream agents.

---

# Governance Model

The Decision Story Agent operates under:

```text
Platform Coach Standard
↓
Framework
↓
Architecture
↓
Repository Standard
↓
Skill Package Standard
↓
Skill Implementation Standard
↓
Decision Story Agent
↓
Runtime Execution
```

Governance always overrides execution.

---

# Traceability Standard

The agent must preserve:

```text
Business Problem
↓
Business Capability
↓
Business Outcome
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

The agent is the first platform component responsible for establishing and preserving the traceability chain.

---

# Recommended Read Order

Before reviewing this repository:

Read:

```text
01_PLATFORM_STARTUP_SOP
```

After Platform Context has been established:

Read this repository in the following order:

```text
PROJECT_INIT.md
↓
README.md
↓
AGENT_README.md
↓
SKILL_BLUEPRINT.md
```

Execution begins only after:

```text
02_AGENT_STARTUP_SOP
```

is complete.

---

# Success Criteria

The repository succeeds when:

A complete and approved:

```text
INPUT_BRD
```

can be transformed into:

```text
REPORT_STORY_MATRIX

REPORT_STORY
```

without:

- Business Rediscovery
- Missing Decisions
- Missing Outcomes
- Missing Questions
- Missing Signals
- Missing Actions
- Broken Traceability

while preserving governance, business intent, and decision context.

---

# Next Artifact

After reviewing this repository:

Read:

```text
AGENT_README.md
```

to understand the Decision Story Agent's responsibilities, inputs, outputs, lifecycle ownership, governance model, and operating model in detail.