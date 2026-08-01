# 03_DECISION_STORY_EXECUTION_SOP

## Decision-Driven BI Agent Platform

Version: 1.0

Status: Approved

Type: Agent Execution Procedure

Purpose:

Execute the Decision Story Agent using approved governance, standards, guidelines, templates, and business inputs.

This SOP defines the deterministic execution workflow used to transform:

INPUT_BRD

into

REPORT_STORY_MATRIX

and

REPORT_STORY

through a governed and traceable process.

---

# OBJECTIVE

Generate:

REPORT_STORY_MATRIX

REPORT_STORY

using:

- Approved Input Contracts
- Approved Input Payloads
- Governance
- Standards
- Guidelines
- Templates

while preserving:

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

---

# PREREQUISITES

The following must already be complete:

```text
01_PLATFORM_STARTUP_SOP

02_AGENT_STARTUP_SOP
```

Required Outcomes:

```text
Platform Context Established

Agent Context Established
```

If either prerequisite is incomplete:

```text
STOP EXECUTION
```

---

# REPOSITORY ASSUMPTION

Assume execution begins at repository root.

```text
decision-story-agent/

├── inputs/
├── standards/
├── guidelines/
├── templates/
├── contracts/
├── governance/
├── test-run/
│
├── PROJECT_INIT.md
├── README.md
├── AGENT_README.md
├── SKILL_BLUEPRINT.md
└── skill.md
```

---

# ARTIFACT RESOLUTION RULE

Resolve artifacts using:

Purpose
↓
Compatibility
↓
Version

Selection Rule:

Highest Compatible Version

Ignore:

- Draft
- Experimental
- Deprecated
- Archived

unless explicitly requested.

---

# EXECUTION MODES

---

## Mode 01 — Repository Access

Examples:

- Codex
- Claude Code
- GitHub Copilot Agent

Agent may:

- Navigate Repository
- Resolve Artifacts
- Read Files
- Generate Outputs

---

## Mode 02 — Chat Context

Examples:

- M365 Copilot Chat
- ChatGPT Chat
- Gemini Chat
- Claude Chat

Agent may not have repository access.

If artifacts are unavailable:

```text
STOP EXECUTION
```

Request missing artifacts.

Do not infer missing content.

---

# HUMAN-IN-THE-LOOP RULE

If a required artifact is unavailable:

Do Not:

- Invent Governance
- Invent Standards
- Invent Templates
- Invent Inputs

Instead:

Request missing artifacts.

Execution may continue after artifacts are supplied.

---

# PHASE 01 — LOAD GOVERNANCE

Resolve:

```text
DECISION_STORY_GOLD_OUTPUT_SPEC

DECISION_STORY_REVIEW_CRITERIA

DECISION_STORY_SCORING_MODEL
```

Location:

```text
governance/
```

Purpose:

Understand:

- Output Quality Requirements
- Review Requirements
- Promotion Expectations
- Failure Conditions

Outcome:

```text
Governance Loaded
```

---

# PHASE 02 — LOAD STANDARDS

Resolve:

```text
REPORT_DESIGN_STANDARDS
```

Location:

```text
standards/
```

Purpose:

Understand:

- Decision Design
- Question Design
- Signal Design
- Threshold Design
- Action Design
- Story Design

Outcome:

```text
Standards Loaded
```

---

# PHASE 03 — LOAD GUIDELINES

Resolve:

```text
DECISION_STORY_GUIDELINES
```

Location:

```text
guidelines/
```

Purpose:

Understand:

- Discovery Methodology
- Design Guidance
- Validation Guidance
- Handoff Guidance

Outcome:

```text
Guidelines Loaded
```

---

# PHASE 04 — LOAD OUTPUT CONTRACTS

Resolve:

```text
01_REPORT_STORY_MATRIX_TEMPLATE

02_REPORT_STORY_TEMPLATE
```

Location:

```text
templates/
```

Purpose:

Understand:

- Matrix Structure
- DSC Structure
- Section Requirements
- Output Expectations

Outcome:

```text
Output Contracts Loaded
```

---

# PHASE 05 — LOAD INPUT CONTRACT

Resolve:

```text
INPUT_BRD_TEMPLATE
```

Location:

```text
inputs/
```

Purpose:

Understand:

- Required BRD Structure
- Readiness Rules
- Required Sections

Outcome:

```text
Input Contract Loaded
```

---

# PHASE 06 — LOAD INPUT PAYLOAD

Resolve:

```text
INPUT_BRD
```

Location:

```text
inputs/
```

Purpose:

Provide:

- Business Context
- Business Requirements
- Decision Context
- Stakeholders
- Business Outcomes

Outcome:

```text
Business Context Loaded
```

---

# PHASE 07 — INPUT READINESS VALIDATION

Validate INPUT_BRD against INPUT_BRD_TEMPLATE.

Verify:

- Business Capability Defined
- Business Outcomes Defined
- Outcome Owner Defined
- Primary Decision Defined
- Secondary Decisions Defined
- Business Questions Defined
- Signals Defined
- KPI Contracts Defined
- Actions Defined
- Risks Defined
- Data Sources Defined
- Stakeholders Defined

If critical readiness conditions fail:

```text
STOP EXECUTION
```

Return Readiness Findings.

Outcome:

```text
BRD Ready
```

---

# PHASE 08 — BUSINESS INTERPRETATION

Extract:

```text
Business Problem

Business Capability

Business Outcomes

Primary Decision

Secondary Decisions

Success Criteria

Stakeholders
```

Build:

```text
Capability
↓
Outcome
↓
Decision
```

model.

Outcome:

```text
Business Context Understood
```

---

# PHASE 09 — EXECUTE BLUEPRINT

Apply:

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

using:

- Governance
- Standards
- Guidelines

Outcome:

```text
Blueprint Execution Complete
```

---

# PHASE 10 — DESIGN DECISION CHAIN

Build:

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
↓
Visual
```

Traceability Model.

Verify:

No orphan:

- Decisions
- Questions
- Signals
- Thresholds
- Actions
- Stories
- Visuals

Outcome:

```text
Decision Chain Complete
```

---

# PHASE 11 — GENERATE REPORT_STORY_MATRIX

Populate:

```text
01_REPORT_STORY_MATRIX_TEMPLATE
```

Generate:

```text
REPORT_STORY_MATRIX
```

Verify:

- Question Coverage
- Signal Coverage
- Action Coverage
- Story Coverage
- Visual Coverage

Outcome:

```text
Matrix Generated
```

---

# PHASE 12 — VALIDATE REPORT_STORY_MATRIX

Validate against:

- Governance
- Standards
- Guidelines

Verify:

- Traceability Complete
- Coverage Complete
- Required Sections Complete

Outcome:

```text
Matrix Validated
```

---

# PHASE 13 — GENERATE REPORT_STORY

Populate:

```text
02_REPORT_STORY_TEMPLATE
```

Generate:

```text
REPORT_STORY
```

Outcome:

```text
DSC Generated
```

---

# PHASE 14 — VALIDATE REPORT_STORY

Validate against:

- Governance
- Standards
- Guidelines
- REPORT_STORY_MATRIX

Verify:

- Story Coverage
- Narrative Coverage
- Decision Coverage
- Traceability Coverage
- Visual Coverage

Outcome:

```text
DSC Validated
```

---

# PHASE 15 — CREATE TEST RUN

Create:

```text
test-run/

Test_Run_<ID>_<Scenario>/
```

Example:

```text
Test_Run_01_AnimalFlow/
```

Store:

```text
REPORT_STORY_MATRIX

REPORT_STORY
```

Do Not:

- Overwrite Previous Runs
- Modify Historical Test Runs

Outcome:

```text
Execution Stored
```

---

# PHASE 16 — EXECUTION REPORT

Generate:

Execution Report

Include:

---

## Dependencies

Artifacts Loaded

---

## Validation Results

Governance

Standards

Guidelines

Input Validation

Matrix Validation

DSC Validation

---

## Assumptions

Document assumptions used.

---

## Outputs

Generated:

```text
REPORT_STORY_MATRIX

REPORT_STORY
```

---

## Test Run Location

Example:

```text
Test_Run_01_AnimalFlow
```

---

## Recommendation

```text
Ready For Review

Ready With Findings

Not Ready
```

---

# FAILURE CONDITIONS

STOP EXECUTION if:

- Input Contract Missing
- Input Payload Missing
- Governance Missing
- Standards Missing
- Guidelines Missing
- Templates Missing
- BRD Readiness Fails
- Traceability Broken
- Matrix Validation Fails
- DSC Validation Fails

---

# EXIT CRITERIA

The execution succeeds when:

```text
REPORT_STORY_MATRIX
```

and

```text
REPORT_STORY
```

have been generated, validated, and stored within a test run folder.

---

# SUCCESS STATEMENT

This SOP succeeds when a valid:

INPUT_BRD

can be transformed into:

REPORT_STORY_MATRIX
↓
REPORT_STORY

through a deterministic, governed, traceable, and repeatable process without requiring significant business rediscovery.

The resulting outputs are ready for:

- Business Review
- Design Review
- Mockup Agent
- TRD Agent
- Semantic Design Agent
- Future Build Agents