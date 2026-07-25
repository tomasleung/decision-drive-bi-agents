# Guidelines

## Decision Story Agent

---

# Purpose

This folder contains the implementation guidelines used by the Decision Story Agent.

Guidelines define:

- How To Apply Standards
- How To Analyze Inputs
- How To Discover Decisions
- How To Discover Questions
- How To Discover Signals
- How To Discover Actions
- How To Design Stories
- How To Validate Outputs

The guidelines ensure Decision Story generation remains:

- Consistent
- Repeatable
- Traceable
- Business Driven
- Action Oriented

across all projects.

---

# Why Guidelines Exist

Standards define:

What Good Looks Like

Guidelines define:

How To Achieve It

Without guidelines, different analysts, developers, and AI models may interpret the same business requirements differently.

Guidelines provide a repeatable methodology for transforming:

Business Requirements
↓
Decision Framework
↓
Story Framework
↓
Decision Story Contract

---

# Current Guidelines

## DECISION_STORY_GUIDELINES_v2.0

Purpose:

Provide the official Decision Story discovery and design methodology.

The guideline defines:

- BRD Analysis
- Decision Discovery
- Question Discovery
- Signal Discovery
- Threshold Design
- Action Discovery
- Story Construction
- Coverage Discovery
- Traceability Validation
- Handoff Rules

The guideline defines:

How To Apply Standards

during execution.

---

# Guideline Coverage

## BRD Analysis

Defines:

- Business Goal Analysis
- Problem Analysis
- Current State Analysis
- Future State Analysis
- Stakeholder Analysis

Answers:

What is the business trying to achieve?

---

## Decision Discovery

Defines:

- Primary Decision Discovery
- Secondary Decision Discovery
- Decision Validation
- Decision Prioritization

Answers:

What decisions should be supported?

---

## Question Discovery

Defines:

- Explicit Question Discovery
- Implied Question Discovery
- Coverage Analysis
- Question Validation

Answers:

What information is required before making a decision?

---

## Signal Discovery

Defines:

- Signal Identification
- Signal Classification
- Signal Prioritization
- Signal Validation

Answers:

What evidence should support the decision?

---

## Threshold Design

Defines:

- Threshold Discovery
- Status Design
- Business Meaning Design
- Action Triggers

Answers:

When should users react?

---

## Action Discovery

Defines:

- Business Response Design
- Operational Actions
- Responsible Roles
- Expected Outcomes

Answers:

What should happen next?

---

## Story Construction

Defines:

- Story Purpose
- Story Sequencing
- Story Responsibilities
- Story Validation

Answers:

How should the decision journey be communicated?

---

## Coverage Discovery

Defines:

- Operational Coverage
- Capacity Coverage
- Risk Coverage
- Governance Coverage
- Data Quality Coverage
- Regional Coverage
- Executive Coverage

Answers:

Has the business problem been fully covered?

---

## Traceability

Defines:

- Decision Traceability
- Question Traceability
- Signal Traceability
- Action Traceability
- Story Traceability

Answers:

Can every design artifact be traced back to a decision?

---

## Validation

Defines:

- Decision Validation
- Question Validation
- Signal Validation
- Action Validation
- Story Validation
- Traceability Validation

Answers:

Is the design ready for promotion?

---

# Relationship To Other Framework Layers

The Decision Story Framework follows:

Input Contract
↓
Standards
↓
Guidelines
↓
Templates
↓
Agent
↓
Governance

---

## Inputs

Define:

What Information Is Required

---

## Standards

Define:

What Good Looks Like

---

## Guidelines

Define:

How To Apply Standards

---

## Templates

Define:

What Must Be Produced

---

## Agent

Defines:

How Framework Artifacts Are Executed

---

## Governance

Defines:

How Outputs Are Evaluated

---

# Relationship To Standards

Standards define:

- Design Principles
- Quality Expectations
- Governance Expectations

Guidelines define:

- Discovery Methods
- Design Methods
- Validation Methods
- Execution Methods

Relationship:

Standards
↓
Guidelines
↓
Templates
↓
Artifacts

Guidelines must never override standards.

---

# Discovery Chain

All design activities should follow:

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

This sequence should remain traceable throughout the design process.

---

# Governing Rule

The Guidelines folder is the:

Official Design Methodology

for the Decision Story Agent.

Agent logic should follow the guidelines.

Templates should assume the guidelines have been applied.

When conflicts exist:

Standards Win

Guidelines Direct Execution

---

# Usage

The Decision Story Agent must apply:

DECISION_STORY_GUIDELINES_v2.0

after reviewing:

REPORT_DESIGN_STANDARDS_v2.0

and before populating:

- REPORT_STORY_MATRIX
- REPORT_STORY

---

# Validation

Before generating outputs verify:

□ Business Problem Understood

□ Primary Decision Defined

□ Secondary Decisions Defined

□ Question Coverage Complete

□ Signal Coverage Complete

□ Threshold Logic Defined

□ Action Logic Defined

□ Story Coverage Complete

□ Traceability Preserved

---

# Success Statement

The Guidelines folder succeeds when:

Every Decision Story

follows the same discovery process,

uses the same design methodology,

maintains full traceability,

and consistently converts business requirements into decision-focused artifacts.

The result is:

- Consistent
- Governed
- Repeatable
- Traceable
- Action-Oriented
- Decision-Driven Design

across all future implementations.