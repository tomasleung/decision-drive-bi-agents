# Contracts

## Decision Story Agent

Version: 1.0

Status: Approved

Purpose:

The Contracts folder contains the governed handoff contracts used by the Decision Story Agent.

Contracts define:

- Required Information
- Approval Requirements
- Handoff Readiness
- Downstream Expectations

Contracts exist to ensure downstream agents can consume Decision Story outputs without requiring business rediscovery.

---

# Contract Philosophy

A template defines:

```text
Structure
```

A contract defines:

```text
Required Information
+
Governance
+
Approval
+
Readiness
```

Templates help create artifacts.

Contracts govern artifacts.

---

# Decision Story Contract Ecosystem

The Decision Story Agent currently defines the following contract.

---

## DECISION_STORY_HANDOFF_CONTRACT_v1.0

Purpose:

Govern the handoff of:

```text
REPORT_STORY
```

to downstream agents.

The contract defines:

- Required Sections
- Required Business Context
- Required Decision Logic
- Required Traceability
- Approval Requirements

before downstream consumption is allowed.

---

# Handoff Philosophy

The Decision Story Agent should eliminate:

```text
Business Rediscovery
```

Downstream agents should understand:

- Business Intent
- Decisions
- Questions
- Signals
- Thresholds
- Actions
- Story Logic

without returning to discovery sessions.

---

# Downstream Consumers

The contract supports:

```text
Mockup Agent

TRD Agent

Semantic Design Agent

Semantic Build Agent

Report Build Agent
```

---

# Contract Success Statement

The contracts layer succeeds when:

Decision Story outputs can move from:

```text
Decision Validation
```

to

```text
Business Design

Technical Design

Semantic Design

Implementation
```

without loss of business intent, governance, or traceability.