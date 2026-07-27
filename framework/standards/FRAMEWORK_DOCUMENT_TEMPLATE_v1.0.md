# FRAMEWORK_DOCUMENT_TEMPLATE_v1.0

## Purpose

This document defines the standard structure for all Decision-Driven BI Framework artifacts.

The objective is to ensure:

- Consistency
- Maintainability
- Traceability
- Readability
- AI Portability

across all framework documents.

---

# Document Classification

Framework documents belong to one of three categories:

## Category 01 — Repository Documents

Examples:

- FRAMEWORK_README
- ARCHITECTURE
- INPUTS README
- STANDARDS README
- GUIDELINES README
- TEMPLATES README

Purpose:

Explain framework components.

---

## Category 02 — Agent Documents

Examples:

- DECISION_STORY_AGENT_README
- REVIEW_AGENT_README
- MOCKUP_AGENT_README

Purpose:

Define agent responsibilities and framework relationships.

---

## Category 03 — Execution Artifacts

Examples:

- REPORT_STORY_MATRIX
- REPORT_STORY (DSC)
- MOCKUP
- TRD
- SEMANTIC_DESIGN

Purpose:

Execute framework methodology.

---

# Standard Metadata Block

Every major document should begin with:

## Document Metadata

Document Type

Version

Status

Owner

Purpose

Audience

Related Artifacts

Dependencies

---

# Repository Document Structure

Use for:

- README
- Architecture Documents
- Standards Documents
- Guidelines Documents

Structure:

# Document Title

## Purpose

## Scope

## Position In Framework

## Responsibilities

## Relationships

## Inputs

## Outputs

## Dependencies

## Governance

## Success Criteria

## Success Statement

## Promotion Status

---

# Agent Document Structure

Use for:

- Agent READMEs

Structure:

# Agent Name

## Purpose

## Mission

## Agent Position In Framework

## Repository Structure

## Folder Responsibilities

## Agent Responsibilities

## Core Philosophy

## Framework Dependencies

## Agent Read Order

## Framework Layers

## Inputs

## Input Readiness Validation

## Stop Conditions

## Discovery Process

## Outputs

## Validation Rules

## Traceability Standard

## Approval Gates

## Downstream Agent Relationships

## Success Criteria

## Success Statement

## Promotion Status

---

# Skill Blueprint Structure

Use for:

- Skill Blueprints

Structure:

# Skill Blueprint Name

## Metadata

## Purpose

## Mission

## Operating Model

## Governance Boundary

## Agent Lifecycle

## Framework Read Order

## Input Validation Engine

## Discovery Engine

## Validation Engine

## Output Engine

## Traceability Engine

## Failure Modes

## Approval Gates

## Human Approval Boundary

## Success Criteria

## Promotion Status

## Next Artifact

---

# Execution Artifact Structure

Use for:

- REPORT_STORY_MATRIX
- REPORT_STORY
- MOCKUP
- TRD

Structure:

## Document Metadata

## Decision Model

## Business Questions

## Signal Definitions

## Threshold Definitions

## Action Matrix

## Traceability Model

## Story Design

## Layout Blueprint

## Visual Recommendations

## Validation Checklist

## Approval Gate

## Success Statement

## Next Step

---

# Formatting Rules

Rule 01

Use hierarchical headings:

# Level 1

## Level 2

### Level 3

---

Rule 02

Use Purpose sections before implementation sections.

Explain:

Why

before

How

---

Rule 03

Place governance before execution.

Readers should understand:

Rules

before

Behavior

---

Rule 04

Every artifact should include:

Purpose

Success Criteria

Success Statement

Promotion Status

---

Rule 05

Every framework artifact should answer:

Why does this exist?

What does it produce?

How is success measured?

What happens next?

---

# Writing Style Rules

Use:

- Business language first
- Technical language second
- Active voice
- Short sections
- Explicit responsibilities

Avoid:

- Ambiguous language
- Technology-first explanations
- Long paragraphs
- Hidden assumptions

---

# Traceability Requirement

All framework documents should support:

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

whenever applicable.

---

# Governance Requirement

No artifact is considered complete until:

Purpose Defined

Responsibilities Defined

Success Criteria Defined

Success Statement Defined

Promotion Status Defined

---

# Success Statement

This template succeeds when all framework artifacts:

Appear consistent

Follow predictable structure

Remain maintainable

Remain AI portable

Remain traceable

and can be understood by:

Humans

AI Agents

Future Contributors

without additional explanation.

---

# Promotion Status

Version:
1.0

Status:
APPROVED

Maturity:
Framework Standard

Promotion:
Approved For All Future Documentation