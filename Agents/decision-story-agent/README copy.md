# Decision Story Agent

## Decision-Driven BI Agent Platform

Version: 1.0

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

├── standards/

├── guidelines/

├── templates/

├── contracts/

├── governance/

├── examples/

├── outputs/

├── test-run/

├── PROJECT_INIT.md

├── README.md

├── AGENT_README.md

├── SKILL_BLUEPRINT.md

├── skill.md

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

Where should contributors start?
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
How does the agent work?

What lifecycle stages exist?

What validations exist?

What outputs are produced?
```

---

## skill.md

Purpose:

Runtime Instructions

Answers:

```text
What should the AI do right now?

How should execution occur?
```

---

# Agent Lifecycle Position

The Decision Story Agent is the first platform agent.

Platform flow:

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
Business Discovery Contracts

Platform Standards

Decision-First Framework

RDLC Governance Rules
```

---

# Outputs

Primary Outputs:

```text
REPORT_STORY_MATRIX

REPORT_STORY
```

The outputs become the governing business design artifacts used by downstream agents.

---

# Questions Answered

The Decision Story Agent answers:

```text
What business problem requires support?

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
- Action Discovery
- Story Discovery
- Coverage Validation
- Traceability Validation

The agent is not responsible for:

- UX Design
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

The agent is the first platform component responsible for formally establishing this traceability chain.

---

# Recommended Read Order

Before reviewing this repository:

Read:

```text
README.md

framework/README.md

framework/standards/README.md

agents/README.md
```

Then read this repository in the following order:

```text
PROJECT_INIT.md
↓
README.md
↓
AGENT_README.md
↓
SKILL_BLUEPRINT.md
↓
skill.md
```

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
- Missing Questions
- Missing Signals
- Missing Actions
- Broken Traceability

while preserving governance and decision intent.

---

# Next Artifact

After reviewing this repository:

Read:

```text
AGENT_README.md
```

to understand the Decision Story Agent's responsibilities, inputs, outputs, lifecycle, and operating model in detail.