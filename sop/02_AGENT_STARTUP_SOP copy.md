# 02_AGENT_STARTUP_SOP

## Decision-Driven BI Agent Platform

Version: 1.0

Status: Approved

Type: Agent Startup Procedure

Purpose:

Establish complete understanding of a platform agent before execution begins.

This SOP serves as the official initialization procedure for all platform agents.

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

Before executing an agent, establish understanding of:

- Agent Purpose
- Agent Responsibilities
- Agent Lifecycle
- Inputs
- Outputs
- Validation Rules
- Governance Rules
- Promotion Rules
- Handoff Rules
- Knowledge Ecosystem

Execution should not begin until agent context has been established.

---

# PREREQUISITE

The following must already be complete:

```text
01_PLATFORM_STARTUP_SOP
```

Required Outcome:

```text
Platform Context Established
```

If Platform Context has not been established:

```text
STOP EXECUTION
```

Complete Platform Startup first.

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
│   └── decision-story-agent/
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

Do not rely on hardcoded versions.

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

Capabilities:

- Navigate folders
- Resolve artifacts
- Load files
- Review repository contents

Execution should proceed normally.

---

## Mode 02 — Chat Context Mode

Examples:

- M365 Copilot Chat
- ChatGPT Chat
- Gemini Chat
- Claude Chat

Capabilities:

- Limited repository visibility
- No direct folder navigation
- Requires uploaded artifacts

If required artifacts cannot be located:

```text
STOP DISCOVERY
```

Request required artifacts from the user.

Uploaded artifacts become the execution context.

---

# HUMAN-IN-THE-LOOP RULE

If a required artifact cannot be located:

Do Not:

- Invent content
- Assume content
- Create replacement standards
- Guess responsibilities
- Infer governance
- Infer lifecycle behavior

Instead:

Request the missing artifact.

---

## Missing Artifact Report

When requesting an artifact provide:

Artifact Name

Expected Location

Purpose

Why It Is Required

Example:

```text
Missing Artifact:

AGENT_README

Expected Location:

agents/decision-story-agent/

Purpose:

Agent Responsibilities

Required For:

Agent Understanding
```

Execution may continue after required artifacts are supplied.

---

# AGENT STARTUP SEQUENCE

Complete all phases in order.

Do not skip phases.

---

# PHASE 01

## Establish Agent Mission

Resolve:

```text
PROJECT_INIT
```

Location:

```text
agents/decision-story-agent/
```

Purpose:

Understand:

- Agent Mission
- Agent Scope
- Lifecycle Position
- Business Purpose
- Success Criteria

Expected Outcome:

```text
Agent Mission Understood
```

Completion Status:

```text
PASS
FAIL
```

---

# PHASE 02

## Establish Agent Responsibilities

Resolve:

```text
AGENT_README
```

Location:

```text
agents/decision-story-agent/
```

Purpose:

Understand:

- Responsibilities
- Non-Responsibilities
- Inputs
- Outputs
- Validation Model
- Approval Model
- Handoff Model

Expected Outcome:

```text
Agent Responsibilities Understood
```

Completion Status:

```text
PASS
FAIL
```

---

# PHASE 03

## Establish Agent Operation

Resolve:

```text
SKILL_BLUEPRINT
```

Location:

```text
agents/decision-story-agent/
```

Purpose:

Understand:

- Lifecycle
- Discovery Process
- Validation Process
- Reasoning Process
- Generation Process
- Promotion Rules
- Failure Conditions

Expected Outcome:

```text
Agent Operation Understood
```

Completion Status:

```text
PASS
FAIL
```

---

# AGENT KNOWLEDGE ECOSYSTEM

The Decision Story Agent operates using multiple knowledge layers.

Agent Startup establishes awareness of these layers.

Execution of these layers occurs later during:

```text
03_DECISION_STORY_EXECUTION_SOP
```

Startup should not execute these artifacts.

Startup should only understand their purpose and location.

---

## Standards Layer

Expected Location:

```text
agents/decision-story-agent/standards/
```

Purpose:

Define:

- What Good Looks Like
- Design Standards
- Quality Standards
- Governance Expectations

Startup Outcome:

Understand Standards Exist.

Do Not Execute Standards.

---

## Guidelines Layer

Expected Location:

```text
agents/decision-story-agent/guidelines/
```

Purpose:

Define:

- Discovery Guidance
- Design Guidance
- Validation Guidance
- Handoff Guidance

Startup Outcome:

Understand Guidelines Exist.

Do Not Execute Guidelines.

---

## Templates Layer

Expected Location:

```text
agents/decision-story-agent/templates/
```

Purpose:

Define:

- REPORT_STORY_MATRIX Structure
- REPORT_STORY Structure

Startup Outcome:

Understand Templates Exist.

Do Not Populate Templates.

---

## Governance Layer

Expected Location:

```text
agents/decision-story-agent/governance/
```

Purpose:

Define:

- Gold Output Specifications
- Review Criteria
- Scoring Models
- Promotion Expectations

Startup Outcome:

Understand Governance Exists.

Do Not Apply Governance.

---

## Inputs Layer

Expected Location:

```text
agents/decision-story-agent/inputs/
```

Purpose:

Provide:

- Business Context
- Business Requirements
- Discovery Artifacts

Startup Outcome:

Understand Inputs Exist.

Do Not Analyze Inputs Yet.

---

## Outputs Layer

Expected Location:

```text
agents/decision-story-agent/outputs/
```

Purpose:

Store generated artifacts.

Expected Outputs:

```text
REPORT_STORY_MATRIX

REPORT_STORY
```

Startup Outcome:

Understand Output Destination Exists.

Do Not Generate Outputs Yet.

---

## Execution Layer

Execution of:

- Governance
- Standards
- Guidelines
- Templates
- Inputs

belongs to:

```text
03_DECISION_STORY_EXECUTION_SOP
```

and not Agent Startup.

---

# AGENT UNDERSTANDING CHECK

Before continuing verify understanding of:

---

## Agent Mission

Can explain:

- Why the agent exists
- What business problem it solves
- What lifecycle phases it owns

---

## Inputs

Can explain:

- Required Inputs
- Input Readiness Expectations
- Business Context Requirements

---

## Outputs

Can explain:

```text
REPORT_STORY_MATRIX

REPORT_STORY
```

and their purpose.

---

## Lifecycle

Can explain:

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

---

## Validation

Can explain:

- Decision Validation
- Coverage Validation
- Traceability Validation
- Handoff Validation

---

## Governance

Can explain:

- Human Authority Principle
- Approval Model
- Promotion Rules
- Failure Conditions

---

## Knowledge Ecosystem

Can explain:

- Standards Layer
- Guidelines Layer
- Templates Layer
- Governance Layer
- Inputs Layer
- Outputs Layer

---

# AGENT CONTEXT REPORT

Upon completion generate an Agent Startup Report.

---

## Agent

```text
Decision Story Agent
```

---

## Agent Purpose

Provide summary of mission.

---

## Lifecycle Ownership

Expected:

```text
Decision Validation

Business Design
```

---

## Inputs

Expected:

```text
INPUT_BRD
```

---

## Outputs

Expected:

```text
REPORT_STORY_MATRIX

REPORT_STORY
```

---

## Validation Model

Provide summary of:

- Decision Validation
- Coverage Validation
- Traceability Validation
- Handoff Validation

---

## Knowledge Ecosystem

Provide summary of:

- Standards
- Guidelines
- Templates
- Governance
- Inputs
- Outputs

---

## Handoff Model

Expected Consumers:

```text
Mockup Agent

TRD Agent

Semantic Design Agent

Semantic Build Agent

Report Build Agent
```

---

## Startup Status

```text
PASS
```

or

```text
FAIL
```

---

## Blocking Issues

List:

- Missing Artifacts
- Missing Context
- Startup Failures

---

# COMPLETION RULE

Do not execute:

- Skill Runtime
- REPORT_STORY_MATRIX Generation
- REPORT_STORY Generation

until Agent Startup is complete.

Execution belongs to:

```text
03_DECISION_STORY_EXECUTION_SOP
```

---

# EXIT CRITERIA

Agent Context Established

Participant can explain:

- Agent Mission
- Agent Responsibilities
- Inputs
- Outputs
- Lifecycle
- Validation Rules
- Governance Rules
- Knowledge Ecosystem
- Handoff Rules
- Promotion Rules

without additional agent discovery.

---

# SUCCESS STATEMENT

This SOP succeeds when any human or AI participant can establish a consistent understanding of the Decision Story Agent before execution begins.

The result is:

```text
Agent Context Established
```

before:

```text
Decision Story Execution
```

begins.