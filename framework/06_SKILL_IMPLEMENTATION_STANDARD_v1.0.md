# 06_SKILL_IMPLEMENTATION_STANDARD_v1.0.md

## Decision-Driven BI Agent Platform

Version: 1.0

Status: Approved

Maturity: Platform Standard

Purpose:

Define the minimum implementation requirements for all platform skills.

This standard ensures every platform skill:

- Looks consistent
- Behaves consistently
- Is portable across AI platforms
- Supports governance
- Supports traceability
- Supports long-term maintenance

---

# PURPOSE

The Skill Implementation Standard defines:

What must exist inside a production-quality skill.

This standard governs:

- Skill Design
- Skill Behavior
- Skill Documentation
- Skill Validation
- Skill Resources

across all platform agents.

---

# CORE PHILOSOPHY

A skill is not:

Prompt
+
LLM

A skill is:

Knowledge
+
Governance
+
Contracts
+
Examples
+
Execution Logic

The skill should contain the knowledge.

The AI should provide the reasoning.

---

# SKILL IMPLEMENTATION MODEL

Every platform skill should contain:

Metadata
↓
Triggers
↓
Inputs
↓
Outputs
↓
Workflow
↓
Validation
↓
Examples
↓
Edge Cases
↓
Resources

---

# REQUIRED METADATA

Every skill should define:

## Skill Name

Purpose:

Unique skill identity.

Example:

Decision Story Agent

---

## Skill Purpose

Purpose:

Business objective of the skill.

Example:

Convert approved Business Requirements into governed Decision Story artifacts.

---

## Version

Purpose:

Track skill evolution.

Example:

v3.0

---

## Status

Examples:

Draft

Review

Approved

Production Ready

---

## Owner

Purpose:

Identify responsible party.

---

# REQUIRED DESCRIPTION

Every skill should contain:

## Description

Must answer:

What does this skill do?

Why does it exist?

What problem does it solve?

Example:

The Decision Story Agent converts approved Business Requirements into REPORT_STORY_MATRIX and REPORT_STORY artifacts.

---

# REQUIRED TRIGGER MODEL

Every skill should define:

## When To Use

Describe:

Execution situations.

Example:

Use when:

- INPUT_BRD exists
- Decision Design is required
- REPORT_STORY generation is required

---

## When Not To Use

Describe:

Inappropriate execution situations.

Example:

Do not use:

- For semantic modeling
- For technical design
- For report building

---

## Prerequisites

Required conditions before execution.

Example:

- Approved INPUT_BRD
- Framework Understanding Complete

---

# REQUIRED INPUT CONTRACT

Every skill should define:

## Required Inputs

Examples:

INPUT_BRD

REPORT_STORY

TRD

---

## Optional Inputs

Examples:

Examples

Reference Artifacts

Supporting Documents

---

## Dependencies

Examples:

Standards

Guidelines

Templates

Contracts

---

# REQUIRED OUTPUT CONTRACT

Every skill should define:

## Deliverables

Examples:

REPORT_STORY_MATRIX

REPORT_STORY

---

## Success Criteria

Examples:

Traceability Preserved

Coverage Complete

Approval Gate Satisfied

---

# REQUIRED WORKFLOW

Every skill should explicitly define:

## Execution Lifecycle

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

---

## Stage Definitions

Each stage should define:

Purpose

Inputs

Outputs

Exit Criteria

---

# REQUIRED VALIDATION MODEL

Every skill should define:

## Validation Rules

Examples:

Question Coverage

Signal Coverage

Story Coverage

---

## Approval Gates

Define:

What approval means.

---

## Promotion Rules

Define:

When output can move downstream.

---

## Stop Conditions

Examples:

Missing Inputs

Failed Validation

Failed Governance Review

---

# REQUIRED AI BEHAVIOR RULES

Every skill should define:

## Resolution Rules

How artifacts are selected.

Examples:

Purpose Validation

Status Validation

Compatibility Validation

Version Resolution

---

## Governance Rules

Examples:

Standards Win

Guidelines Direct Execution

Templates Define Structure

Examples Demonstrate Usage

---

## Traceability Rules

Maintain:

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
Implementation

when applicable.

---

# REQUIRED EXAMPLES

Every skill should contain:

## Gold Standard Example

Purpose:

Demonstrate ideal execution.

---

## Expected Output Example

Purpose:

Demonstrate deliverable quality.

---

## Approved Reference Example

Purpose:

Establish quality benchmark.

---

# REQUIRED EDGE CASES

Every skill should define:

## Missing Input Handling

Example:

Incomplete BRD

---

## Low Readiness Handling

Example:

Business Discovery Incomplete

---

## Validation Failure Handling

Example:

Missing Traceability

---

## Governance Failure Handling

Example:

Approval Gate Failed

---

# RESOURCE MODEL

Optional resources should be organized consistently.

---

## references/

Purpose:

Additional documentation.

Examples:

decision-discovery.md

signal-design.md

story-design.md

semantic-design.md

The skill should load references only when required.

---

## scripts/

Purpose:

Deterministic execution.

Examples:

validate_traceability.py

validate_readiness.py

validate_contracts.py

Use scripts for repeatable validation.

---

## assets/

Purpose:

Reusable skill assets.

Examples:

Templates

Icons

Themes

SVG Components

Branding Assets

---

# RESOURCE USAGE RULE

Resources should support:

Consistency

Governance

Repeatability

Skill resources should not replace standards.

---

# IMPLEMENTATION CHECKLIST

Every production-ready skill should define:

✅ Metadata

✅ Description

✅ Triggers

✅ Inputs

✅ Outputs

✅ Workflow

✅ Validation

✅ Approval Gates

✅ Promotion Rules

✅ Examples

✅ Edge Cases

Optional:

⬜ references/

⬜ scripts/

⬜ assets/

---

# SUCCESS CRITERIA

The standard succeeds when every platform skill:

- Is understandable
- Is reusable
- Is governable
- Is portable
- Is testable
- Is maintainable

without requiring direct support from the skill author.

---

# SUCCESS STATEMENT

The Skill Implementation Standard succeeds when a developer or AI agent can:

1. Understand the skill purpose

2. Understand when to use the skill

3. Understand required inputs

4. Understand expected outputs

5. Execute the workflow

6. Validate results

7. Handle edge cases

without requiring direct guidance from the skill creator.

The result is:

Consistent

Governed

Portable

Production-Ready

AI Skill Implementations.

---

# PROMOTION STATUS

Version:

1.0

Status:

APPROVED

Maturity:

Platform Standard

Promotion:

Approved For All Current And Future Agent Repositories

Next Artifact:

README.md