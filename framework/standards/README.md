# Standards README

## Decision-Driven BI Agent Platform

Version: 1.0

Status: Approved

Purpose:

Provide the navigation, catalog, and governance guide for platform standards.

This README serves as the entry point into the standards folder and explains:

- What standards exist
- Why standards exist
- How standards interact
- When standards should be used
- Which standards have authority

---

# Purpose Of The Standards Folder

The standards folder contains the governing rules used throughout the platform.

Standards exist to ensure:

- Consistency
- Governance
- Portability
- Traceability
- Maintainability

across:

- Repositories
- Skills
- Contracts
- Agents
- Future Platform Extensions

---

# Standards Philosophy

Standards define:

What Good Looks Like

Standards are not:

Examples

Templates

Guidelines

Prompts

Standards provide rules.

Other artifacts implement those rules.

---

# Standards Authority Model

The platform follows:

```text
Platform Coach
↓
Standards
↓
Guidelines
↓
Templates
↓
Contracts
↓
Examples
↓
Agent Logic
↓
Runtime Execution
```

Rule:

Higher layers always override lower layers.

---

# Standards Catalog

The standards folder contains platform-wide standards.

---

## DOCUMENT_NAMING_STANDARD

Purpose:

Provide naming consistency across all platform artifacts.

Defines:

- File Naming
- Folder Naming
- Artifact Naming
- Version Naming

Answers:

```text
How should platform assets be named?
```

---

## VERSIONING_STANDARD

Purpose:

Provide platform version governance.

Defines:

- Major Versions
- Minor Versions
- Patch Versions
- Promotion Rules

Answers:

```text
How should platform versions be managed?
```

---

## GOVERNANCE_STANDARD

Purpose:

Define governance expectations across the platform.

Defines:

- Governance Principles
- Ownership Rules
- Approval Requirements
- Promotion Requirements

Answers:

```text
How is governance enforced?
```

---

## FRAMEWORK_DOCUMENT_TEMPLATE

Purpose:

Provide a consistent structure for framework documentation.

Defines:

- Required Sections
- Standard Formatting
- Metadata Requirements

Answers:

```text
How should framework documents be written?
```

---

# Relationship To Other Foundation Artifacts

Standards support the platform foundation.

---

## Platform Coach Standard

Provides:

```text
How To Think
```

---

## Standards

Provide:

```text
What Rules Exist
```

---

## Guidelines

Provide:

```text
How To Apply Rules
```

---

## Templates

Provide:

```text
How To Structure Outputs
```

---

## Agents

Provide:

```text
How Work Gets Done
```

---

# When To Read Standards

Standards should be reviewed when:

- Creating New Repositories
- Creating New Skills
- Creating New Contracts
- Creating New Agents
- Updating Existing Artifacts
- Performing Governance Reviews

---

# Recommended Read Order

Review standards in the following order.

---

## Step 01

DOCUMENT_NAMING_STANDARD

Purpose:

Understand naming conventions.

---

## Step 02

VERSIONING_STANDARD

Purpose:

Understand lifecycle management.

---

## Step 03

GOVERNANCE_STANDARD

Purpose:

Understand governance expectations.

---

## Step 04

FRAMEWORK_DOCUMENT_TEMPLATE

Purpose:

Understand framework documentation structure.

---

# Success Statement

The standards layer succeeds when:

Developers

Architects

Contributors

AI Agents

and Future Platforms

can consistently create:

- Repositories
- Skills
- Contracts
- Framework Documents

using the same governance rules and quality expectations.

The result is:

Consistency

Traceability

Governance

Portability

across the entire platform ecosystem.

---

# Next Location

After reviewing standards:

Navigate to:

```text
agents/README.md
```

to understand the platform's implementation ecosystem.