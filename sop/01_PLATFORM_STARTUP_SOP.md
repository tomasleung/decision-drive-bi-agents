# 01_PLATFORM_STARTUP_SOP

## Decision-Driven BI Agent Platform

Version: 1.0

Status: Approved

Type: Platform Startup Procedure

Purpose:

Establish complete platform understanding before any repository, agent, skill, contract, automation, or implementation activity begins.

This SOP serves as the official entry point into the Decision-Driven BI Agent Platform.

Applicable To:

- Developers
- Architects
- Analysts
- Contributors
- M365 Copilot
- ChatGPT
- Claude
- Gemini
- GitHub Copilot
- Codex
- Future AI Agents

---

# OBJECTIVE

Before performing any platform work, establish understanding of:

- Platform Thinking
- Platform Governance
- Platform Architecture
- Repository Standards
- Skill Standards
- Agent Ecosystem
- Contract Ecosystem

Execution should not begin until platform context has been established.

---

# REPOSITORY ASSUMPTION

Assume execution begins at the repository root.

Example:

```text
/
│
├── framework/
│
├── agents/
│
├── contracts/
│
├── examples/
│
├── sop/
│
└── changelog/
```

Folder names are considered stable.

Files inside folders may evolve through versioning.

---

# ARTIFACT RESOLUTION RULE

Do not rely on hardcoded file versions.

Resolve artifacts using:

Purpose
↓
Compatibility
↓
Version

Selection Rule:

Highest Compatible Version

Ignore artifacts explicitly marked:

- Draft
- Experimental
- Deprecated
- Archived

unless explicitly requested.

---

# EXECUTION MODES

The platform supports two execution modes.

---

## Mode 01 — Repository Access Mode

Examples:

- Codex
- Claude Code
- GitHub Copilot Agent
- Future Code Agents

In this mode the agent can:

- Navigate folders
- Resolve artifacts
- Read repository files

The startup process should proceed normally.

---

## Mode 02 — Chat Context Mode

Examples:

- M365 Copilot Chat
- ChatGPT Chat
- Gemini Chat
- Claude Chat

In this mode the participant may not have direct access to the repository.

If required artifacts cannot be located:

STOP DISCOVERY

Request the required artifacts from the user.

The user becomes the repository access provider.

Uploaded artifacts become the execution context.

---

# HUMAN-IN-THE-LOOP RULE

If a required artifact cannot be located:

Do Not:

- Invent content
- Assume content
- Create replacement standards
- Guess missing governance

Instead:

Request the missing artifacts.

Examples:

- PLATFORM_COACH_STANDARD
- PROJECT_INIT
- FRAMEWORK_README
- DECISION_DRIVEN_BI_ARCHITECTURE

Execution may continue after artifacts are supplied.

---

# SUCCESS RULE

Repository access is optional.

Artifact access is mandatory.

Artifacts may be obtained through:

- Repository Navigation
- File Upload
- Shared Documents
- Approved Execution Context

The source of the artifact does not matter.

Availability of the artifact does.


---


# PLATFORM STARTUP SEQUENCE

Complete all phases in order.

Do not skip phases.

---

# PHASE 01

## Establish Platform Thinking

Resolve:

```text
PLATFORM_COACH_STANDARD
```

Location:

```text
framework/
```

Purpose:

Understand:

- Problem Framing
- Foundation Analysis
- Assumption Validation
- Failure Analysis
- Strategic Recommendation
- Regression Protection

Expected Outcome:

```text
Thinking Alignment Complete
```

---

# PHASE 02

## Establish Platform Mission

Resolve:

```text
PROJECT_INIT
```

Location:

```text
framework/
```

Purpose:

Understand:

- Platform Mission
- Platform Vision
- Platform Objectives
- Success Criteria
- Non-Goals

Expected Outcome:

```text
Mission Alignment Complete
```

---

# PHASE 03

## Establish Platform Governance

Resolve:

```text
FRAMEWORK_README
```

Location:

```text
framework/
```

Purpose:

Understand:

- Decision-First Framework
- Platform Governance
- Platform Principles
- Platform Lifecycle
- Human Authority Model

Expected Outcome:

```text
Governance Alignment Complete
```

---

# PHASE 04

## Establish Platform Architecture

Resolve:

```text
DECISION_DRIVEN_BI_ARCHITECTURE
```

Location:

```text
framework/
```

Purpose:

Understand:

- Platform Layers
- Agent Ecosystem
- Contract Ecosystem
- Execution Layer
- Governance Layer
- Traceability Model

Expected Outcome:

```text
Architecture Alignment Complete
```

---

# PHASE 05

## Establish Repository Understanding

Resolve:

```text
AGENT_REPOSITORY_STANDARD
```

Location:

```text
framework/
```

Purpose:

Understand:

- Repository Structure
- Folder Standards
- Required Files
- Read Order
- Repository Governance

Expected Outcome:

```text
Repository Understanding Complete
```

---

# PHASE 06

## Establish Skill Understanding

Resolve:

```text
SKILL_PACKAGE_STANDARD
```

Location:

```text
framework/
```

Purpose:

Understand:

- Skill Packaging
- Knowledge Layer
- Governance Layer
- Runtime Layer
- Skill Structure

Expected Outcome:

```text
Skill Package Understanding Complete
```

---

# PHASE 07

## Establish Skill Implementation Understanding

Resolve:

```text
SKILL_IMPLEMENTATION_STANDARD
```

Location:

```text
framework/
```

Purpose:

Understand:

- Skill Requirements
- Inputs
- Outputs
- Validation
- Promotion
- Failure Handling
- Runtime Expectations

Expected Outcome:

```text
Skill Implementation Understanding Complete
```

---

# PLATFORM UNDERSTANDING CHECK

Before continuing, verify understanding of:

## Platform Thinking

Can explain:

- Platform Coach purpose
- Problem framing approach
- Regression protection approach

---

## Platform Governance

Can explain:

- Decision-First principles
- Human Authority principle
- Traceability requirements

---

## Platform Architecture

Can explain:

- Platform layers
- Agent ecosystem
- Contract ecosystem

---

## Repository Architecture

Can explain:

- Repository structure
- Required files
- Read order

---

## Skill Architecture

Can explain:

- Blueprint responsibility
- Runtime responsibility
- Governance hierarchy

---

# PLATFORM OPERATING HIERARCHY

The platform operates through:

```text
Coach
↓
Framework
↓
Repository
↓
Skill Package
↓
Skill Implementation
↓
Agent
↓
Contract
↓
Execution
```

Thinking precedes implementation.

Governance precedes automation.

Decision context precedes artifact generation.

---

# COMPLETION RULE

Do not execute:

- Agents
- Skills
- Contracts
- Automation
- Generation Activities

until startup is complete.

---

# EXIT CRITERIA

Platform Context Established

Participant can explain:

- Platform Purpose
- Platform Hierarchy
- Governance Hierarchy
- Agent Ecosystem
- Contract Ecosystem
- Repository Standard
- Skill Standard
- Platform Operating Model

without further platform discovery.

---

# SUCCESS STATEMENT

This SOP succeeds when any human or AI participant can enter the repository and establish a consistent understanding of the Decision-Driven BI Platform before interacting with any agent repository.

The result is:

```text
Shared Platform Context
```

before:

```text
Agent Execution
```

begins.