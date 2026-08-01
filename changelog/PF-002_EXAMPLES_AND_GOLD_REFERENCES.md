# PF-002

# Examples And Gold References

Status:

Proposed

Priority:

Medium

---

# Purpose

Evaluate introducing an examples layer to improve agent calibration and output consistency.

---

# Current State

Agent execution relies on:

- Governance
- Standards
- Guidelines
- Templates
- Inputs

No example repository exists.

---

# Problem

Templates define structure.

Governance defines quality.

Neither provides real implementation examples.

Future agents may produce technically compliant outputs with inconsistent depth, narrative quality, or traceability coverage.

---

# Proposed Solution

Create:

examples/

within agent repositories.

Examples provide:

- Reference Implementations
- Coverage Examples
- Narrative Examples
- Traceability Examples

Examples do not replace:

- Governance
- Standards
- Guidelines
- Templates

---

# Example Contents

examples/

ANIMALFLOW_REPORT_STORY_MATRIX_REFERENCE_v1.0.md

ANIMALFLOW_REPORT_STORY_REFERENCE_v1.0.md

---

# Usage Rules

Examples are optional.

Examples must never become execution dependencies.

Examples should be used for:

- Calibration
- Benchmarking
- Quality Comparison

Examples must not override:

- Governance
- Standards
- Guidelines
- Templates

---

# Benefits

- Improved Output Consistency
- Faster Agent Alignment
- Reduced Output Variability
- Better Cross-LLM Results
- Improved Quality Calibration

---

# Risks

Examples may be copied instead of learned from.

Business logic may become overfit to historical examples.

Agents may incorrectly treat examples as templates.

---

# Recommendation

Do not implement immediately.

First validate:

01_PLATFORM_STARTUP_SOP

02_AGENT_STARTUP_SOP

03_DECISION_STORY_EXECUTION_SOP

and complete multiple successful execution cycles.

Introduce examples only after multiple approved outputs exist.

---

# Success Criteria

A future AI can review approved examples and produce outputs that consistently align with expected coverage, quality, traceability, and narrative depth without copying business-specific content.