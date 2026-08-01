# DECISION_STORY_GUIDELINES_v2.1

## Decision-Driven BI Decision Story Guidelines

---

# DOCUMENT METADATA

Document Name:

DECISION_STORY_GUIDELINES

Version:

2.1

Owner:

Decision-Driven BI Framework

Status:

Approved Guideline

Purpose:

Provide implementation guidance for converting a Business Requirements Document (BRD) into:

- REPORT_STORY_MATRIX
- REPORT_STORY (DSC)

These guidelines complement:

REPORT_DESIGN_STANDARDS_v2.1

The standards define:

What Good Looks Like

These guidelines define:

How To Apply Standards

---

# SECTION 01 — GUIDING PHILOSOPHY

## Outcome First

Every report exists to improve a business outcome.

Always begin with:

Business Problem
↓
Business Capability
↓
Business Outcome
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

Never begin with:

Visual
↓
Layout
↓
Dashboard
↓
Decision

---

## Decision First

Every report exists to support a business decision.

Decisions are the bridge between:

Business Outcomes

and

Business Actions

Without a decision, reporting has no business purpose.

---

## Action Before Reporting

The purpose of reporting is not information.

The purpose of reporting is:

Action

Every report section should improve a decision and enable a business response.

---

## Story Before Visuals

The decision story must be defined before visual selection begins.

Correct:

Business Outcome
↓
Decision
↓
Question
↓
Signal
↓
Action
↓
Story
↓
Visual

Incorrect:

Data
↓
Visual
↓
Dashboard

---

## Human Authority First

The framework is:

AI Assisted
↓
Human Governed

AI may:

- Discover
- Analyze
- Recommend
- Structure

AI may not:

- Approve Decisions
- Own Outcomes
- Assume Accountability

Final authority remains with designated business stakeholders.

---

## Traceability First

Every artifact must support:

Business Problem
↓
Business Capability
↓
Business Outcome
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

No orphan elements are allowed.

---

## Outcome Traceability Rule

Every recommendation should answer:

- What outcome improves?
- Which decision improves it?
- Which action influences the outcome?

If this chain cannot be explained:

The design requires review.

---

## Failure Awareness Principle

Discovery should evaluate:

- What could fail?
- What could be misunderstood?
- What could prevent success?
- What could reduce trust?

Failure analysis should occur before design completion.

---

## Handoff Philosophy

Decision Story outputs should become:

The Authoritative Business Design

for downstream teams.

Downstream teams should not need to re-discover business intent.

---

## Guiding Philosophy Success Statement

Decision Story Design succeeds when:

Business Problems

drive Capabilities

Capabilities

drive Outcomes

Outcomes

drive Decisions

Decisions

drive Questions

Questions

drive Signals

Signals

drive Actions

Actions

drive Stories

Stories

drive Visuals

while preserving:

- Accountability
- Traceability
- Outcome Alignment
- Human Governance

throughout the design process.

---

# SECTION 02 — INPUT USAGE GUIDELINES

## Required Input

Approved Business Requirements Document (BRD)

---

## Preferred Inputs

Priority Order:

### Priority 1

Approved BRD

Purpose:

Authoritative source of business intent.

---

### Priority 2

Business Owner Direction

Purpose:

Clarify goals, decisions, and priorities.

---

### Priority 3

Operational Documentation

Purpose:

Understand real-world processes and constraints.

---

### Priority 4

Existing Reports

Purpose:

Identify reusable logic and existing reporting patterns.

---

### Priority 5

Existing Dashboards

Purpose:

Discover current-state visualizations and stakeholder expectations.

---

## Foundation Discovery Inputs

When available, collect:

- Strategic Goals
- Business Objectives
- Capability Statements
- Operational Procedures
- Governance Documents
- Success Measures

These sources improve discovery quality.

---

## Input Analysis Rule

Do not copy BRD content directly into Decision Story artifacts.

Instead discover:

- Business Problems
- Business Capabilities
- Business Outcomes
- Decisions
- Questions
- Signals
- Thresholds
- Actions
- Stories

---

## Business Intent Priority Rule

When sources conflict:

Business Intent Wins

Priority:

Business Outcome
↓
Business Decision
↓
Business Process
↓
Existing Reports
↓
Current Visual Design

---

## Existing Artifact Review

When existing reports are available:

Review:

- Existing Decisions
- Existing Questions
- Existing Signals
- Existing Stories
- Existing Business Rules

before proposing changes.

---

## Regression Protection Review

When redesigning an existing report:

Identify:

- Approved Logic
- Existing KPIs
- Existing Decisions
- Existing Operational Actions
- Existing Story Elements

Preserve validated business knowledge whenever possible.

---

## Input Validation

Before beginning discovery verify:

- Business Context Available
- Business Problem Understood
- Stakeholders Identified
- Success Criteria Available

If major inputs are missing:

Create a discovery finding.

---

## Input Usage Success Statement

Input Usage succeeds when:

The agent understands:

- Why the report exists
- What capability should improve
- What outcome should improve
- Which decisions require support

before design activities begin.

---

# SECTION 03 — FOUNDATION DISCOVERY GUIDELINES

## Purpose

Foundation Discovery establishes the business context required before Decision Discovery begins.

The objective is to understand:

- Why the report exists
- What capability requires improvement
- What business outcomes are expected
- What risks may affect success

Foundation Discovery prevents teams from designing reports that solve the wrong problem.

---

## Discovery Sequence

Always begin with:

Business Problem
↓
Business Capability
↓
Business Outcome
↓
Decision

Do not begin with:

Decision
↓
Question
↓
Signal

until the foundation has been established.

---

## Foundation Discovery Process

### Step 01

Discover The Business Problem

---

### Step 02

Discover The Business Capability

---

### Step 03

Discover Expected Business Outcomes

---

### Step 04

Discover Strategic Alignment

---

### Step 05

Discover Assumptions

---

### Step 06

Discover Constraints

---

### Step 07

Discover Risks

---

## Business Problem Discovery

### Purpose

Identify the operational, tactical, or strategic issue requiring improvement.

---

### Discovery Questions

Ask:

- What pain point exists today?
- What business friction exists?
- What problem requires attention?
- What decision is difficult today?
- What business impact occurs if nothing changes?

---

### Identify

- Operational Pain Points
- Decision Delays
- Manual Activities
- Data Challenges
- Governance Challenges
- Visibility Gaps

---

## Business Capability Discovery

### Purpose

Identify the business capability that requires support or improvement.

---

### Discovery Questions

Ask:

- What business function is affected?
- What capability requires improvement?
- What operational process is being supported?
- What organizational outcome depends on this capability?

---

### Examples

Capabilities may include:

- Animal Placement
- Capacity Management
- Volunteer Coordination
- Fundraising
- Case Management
- Operational Planning
- Resource Allocation

---

## Capability Validation

A capability should answer:

```text
What does the business need to do better?
```

---

## Business Outcome Discovery

### Purpose

Identify the measurable result expected from the initiative.

Outcomes define success.

---

### Discovery Questions

Ask:

- What should improve?
- What should become faster?
- What should become easier?
- What should become more reliable?
- How will success be measured?

---

### Examples

Business Outcomes:

- Reduced Placement Time
- Improved Capacity Utilization
- Improved Data Trust
- Improved Decision Consistency
- Reduced Escalation Volume
- Improved Operational Efficiency

---

## Outcome Validation

Every outcome should be:

- Measurable
- Relevant
- Actionable
- Business Driven

---

## Strategic Alignment Discovery

### Purpose

Identify how the initiative supports broader goals.

---

### Discovery Questions

Ask:

- Which business objective does this support?
- Which department objective does this support?
- Which organizational goal does this support?
- Why should leadership care?

---

## Assumption Discovery

### Purpose

Identify assumptions that influence the design.

---

### Discovery Questions

Ask:

- What is assumed to be true?
- What conditions are required for success?
- What dependencies exist?

---

### Examples

- Required data is available
- Business processes remain stable
- Stakeholders participate in discovery
- Capacity information is reliable

---

## Constraint Discovery

### Purpose

Identify limitations affecting design.

---

### Discovery Questions

Ask:

- What limitations exist?
- What restrictions must be respected?
- What cannot change?

---

### Examples

- Budget Constraints
- Technology Constraints
- Staffing Constraints
- Governance Constraints
- Operational Constraints

---

## Risk Discovery

### Purpose

Identify conditions that may reduce success.

---

### Discovery Questions

Ask:

- What could go wrong?
- What could reduce trust?
- What could prevent adoption?
- What could reduce decision quality?

---

### Examples

- Poor Data Quality
- Unclear Ownership
- Missing Business Rules
- Stakeholder Misalignment
- Incomplete Requirements

---

## Foundation Summary Construction

Before Decision Discovery summarize:

### Business Problem

Why change is required.

---

### Business Capability

What capability requires improvement.

---

### Business Outcome

What improvement is expected.

---

### Strategic Alignment

Why the initiative matters.

---

### Risks

What could reduce success.

---

## Foundation Readiness Review

Before proceeding verify:

□ Business Problem Defined

□ Business Capability Defined

□ Business Outcomes Defined

□ Strategic Alignment Identified

□ Risks Identified

□ Assumptions Identified

□ Constraints Identified

---

## Validation Rule

If the following are not clearly understood:

- Business Problem
- Business Capability
- Business Outcome

STOP DISCOVERY

and continue business analysis.

Do not proceed to Decision Discovery.

---

## Foundation Discovery Success Statement

Foundation Discovery succeeds when:

Business Problems

identify Capabilities

Capabilities

identify Outcomes

Outcomes

justify Decisions

and the team understands:

- Why the report exists
- What capability should improve
- What outcome should improve
- What success looks like

before Decision Discovery begins.

---

# SECTION 04 — BUSINESS OUTCOME DISCOVERY GUIDELINES

## Purpose

Business Outcome Discovery identifies the measurable results that justify report creation.

Outcomes explain:

- Why the solution exists
- What success looks like
- How improvement is measured
- Which decisions matter most

Outcome Discovery should occur before Decision Discovery.

---

## Governing Rule

Every report must support at least one measurable Business Outcome.

Do not begin with:

Decision
↓
Question
↓
Signal

until the expected outcome is understood.

Always begin with:

Business Problem
↓
Business Capability
↓
Business Outcome

---

## Outcome Discovery Process

### Step 01

Identify Desired Improvement

---

### Step 02

Identify Success Measures

---

### Step 03

Identify Outcome Owner

---

### Step 04

Identify Success Targets

---

### Step 05

Identify Dependencies

---

### Step 06

Validate Outcome Alignment

---

## Desired Improvement Discovery

### Purpose

Identify what should improve if the report succeeds.

---

### Discovery Questions

Ask:

- What should become better?
- What should become faster?
- What should become easier?
- What should become more reliable?
- What should become more consistent?

---

### Examples

Desired Improvements:

- Faster Animal Placement
- Reduced Capacity Risk
- Improved Resource Utilization
- Improved Data Trust
- Reduced Escalation Volume
- Improved Operational Coordination

---

## Outcome Definition

### Purpose

Transform desired improvements into measurable outcomes.

---

### Outcome Structure

Every Business Outcome should define:

- Outcome Name
- Outcome Description
- Success Measure
- Success Target
- Outcome Owner

---

### Example

Outcome Name:

```text
Reduce Animal Placement Time
```

Success Measure:

```text
Average Placement Days
```

Success Target:

```text
Reduce From 18 Days To 12 Days
```

Outcome Owner:

```text
Animal Flow Leadership
```

---

## Outcome Ownership Discovery

### Purpose

Identify who is accountable for achieving the outcome.

---

### Discovery Questions

Ask:

- Who benefits from improvement?
- Who owns the business process?
- Who is accountable for results?
- Who reports success?

---

### Ownership Types

#### Outcome Owner

Accountable for business success.

---

#### Supporting Stakeholders

Influence success but are not accountable.

---

#### Data Contributors

Provide information supporting measurement.

---

## Success Measure Discovery

### Purpose

Identify how improvement will be evaluated.

---

### Discovery Questions

Ask:

- How is success measured today?
- What evidence proves improvement?
- What KPI reflects success?
- What threshold indicates success?

---

### Measure Examples

- Average Placement Time
- Utilization Rate
- Escalation Count
- SLA Compliance
- Data Trust Score
- Adoption Rate

---

## Success Target Discovery

### Purpose

Define the expected level of improvement.

---

### Discovery Questions

Ask:

- How much improvement is required?
- What target indicates success?
- What level justifies investment?

---

### Example Targets

```text
10% Improvement

25% Reduction

95% Compliance

90% Adoption Rate
```

Targets should be realistic and measurable.

---

## Outcome Dependency Discovery

### Purpose

Identify factors required for success.

---

### Discovery Questions

Ask:

- What conditions must exist?
- What business processes influence success?
- What external factors could affect outcomes?
- What resources are required?

---

### Dependency Examples

- Reliable Data
- Consistent Processes
- User Adoption
- Executive Support
- Training Availability

---

## Outcome Prioritization

Where multiple outcomes exist, classify:

### Primary Outcome

The main outcome the solution exists to improve.

---

### Secondary Outcomes

Supporting outcomes improved indirectly.

---

### Strategic Outcomes

Long-term organizational improvements.

---

## Outcome Validation

Every outcome should be:

### Measurable

Success can be quantified.

---

### Relevant

Supports the business problem.

---

### Achievable

Reasonably attainable.

---

### Actionable

Influenced by business decisions and actions.

---

### Governed

Has a clearly identified owner.

---

## Outcome Traceability Review

Verify:

Business Problem
↓
Business Capability
↓
Business Outcome

is clearly understood before Decision Discovery begins.

---

## Outcome Readiness Checklist

Before proceeding verify:

□ Business Outcome Defined

□ Outcome Owner Defined

□ Success Measure Defined

□ Success Target Defined

□ Dependencies Identified

□ Outcome Prioritized

---

## Validation Rule

If any of the following are unknown:

- Outcome
- Outcome Owner
- Success Measure

STOP DISCOVERY

and continue business analysis.

Do not proceed to Decision Discovery.

---

## Outcome Discovery Success Statement

Business Outcome Discovery succeeds when:

Business Problems

identify Capabilities

Capabilities

identify Outcomes

Outcomes

define Success

and stakeholders can clearly explain:

- What should improve?
- How improvement is measured?
- Who owns success?
- What target defines success?

before Decision Discovery begins.

---

# SECTION 05 — BRD ANALYSIS FRAMEWORK

## Purpose

Analyze the Business Requirements Document (BRD) before beginning Decision Story generation.

The objective is not to copy BRD content.

The objective is to discover:

- Business Problems
- Business Capabilities
- Business Outcomes
- Decisions
- Questions
- Signals
- Actions
- Stories
- Risks
- Accountability Requirements

A BRD should be treated as a discovery source rather than an output source.

---

## Governing Rule

Read the entire BRD before beginning design activities.

Do not begin:

- Decision Discovery
- Question Discovery
- Signal Discovery
- Story Design

until business context has been analyzed.

---

## BRD Analysis Sequence

### Step 01

Analyze Business Summary

---

### Step 02

Analyze Business Problem

---

### Step 03

Analyze Current State

---

### Step 04

Analyze Future State

---

### Step 05

Analyze Business Capabilities

---

### Step 06

Analyze Business Outcomes

---

### Step 07

Analyze Stakeholders

---

### Step 08

Analyze Risks

---

### Step 09

Analyze Success Criteria

---

### Step 10

Prepare Decision Discovery Inputs

---

## Analyze Business Summary

### Purpose

Understand the overall purpose of the initiative.

---

### Extract

- Business Goals
- Expected Benefits
- Success Drivers
- Strategic Objectives

---

### Discovery Questions

Ask:

- What is the organization trying to achieve?
- Why is this initiative important?
- What business result is expected?

---

## Analyze Business Problem

### Purpose

Understand why change is required.

---

### Extract

- Pain Points
- Bottlenecks
- Risks
- Operational Friction
- Decision Challenges
- Data Challenges

---

### Discovery Questions

Ask:

- What problem is occurring today?
- What is difficult today?
- What would happen if nothing changes?
- What consequences exist?

---

## Analyze Current State

### Purpose

Understand the existing environment.

---

### Extract

- Existing Processes
- Existing Reports
- Existing Decisions
- Existing Metrics
- Existing Constraints
- Existing Workarounds

---

### Discovery Questions

Ask:

- How is the work performed today?
- What reporting exists today?
- What manual effort exists?
- What causes frustration?

---

## Analyze Future State

### Purpose

Understand expected improvements.

---

### Extract

- Desired Capabilities
- Desired Outcomes
- Desired User Experience
- Desired Business Performance

---

### Discovery Questions

Ask:

- What should become easier?
- What should improve?
- What should be eliminated?
- What should become possible?

---

## Analyze Business Capabilities

### Purpose

Identify the business capabilities requiring support.

---

### Extract

- Core Business Processes
- Supported Functions
- Supported Services
- Operational Capabilities

---

### Discovery Questions

Ask:

- What capability is being improved?
- What capability should become more effective?
- Which business process depends on this capability?

---

### Examples

- Animal Placement
- Capacity Management
- Volunteer Management
- Fundraising
- Operational Planning

---

## Analyze Business Outcomes

### Purpose

Identify measurable outcomes expected from the initiative.

---

### Extract

- Desired Results
- Success Measures
- Business Targets
- Expected Improvements

---

### Discovery Questions

Ask:

- What business outcome should improve?
- How will success be measured?
- What target indicates success?
- Who owns the outcome?

---

## Analyze Stakeholders

### Purpose

Identify people impacted by decisions and outcomes.

---

### Extract

- Business Owners
- Operational Users
- Executive Stakeholders
- Data Owners
- Governance Participants

---

### Discovery Questions

Ask:

- Who makes decisions?
- Who acts on recommendations?
- Who owns success?
- Who owns approvals?

---

## Analyze Human Authority

### Purpose

Identify accountability and governance structures.

---

### Extract

- Decision Owners
- Approval Authorities
- Escalation Authorities
- Outcome Owners

---

### Discovery Questions

Ask:

- Who holds final authority?
- Who approves actions?
- Who owns outcomes?
- Who is accountable for success?

---

## Analyze Risks

### Purpose

Identify factors that may affect design quality or business success.

---

### Extract

- Operational Risks
- Data Risks
- Governance Risks
- Adoption Risks
- Outcome Risks

---

### Discovery Questions

Ask:

- What could fail?
- What could delay success?
- What could reduce trust?
- What could prevent adoption?

---

## Analyze Success Criteria

### Purpose

Identify how stakeholders will judge success.

---

### Extract

- Outcome Targets
- KPI Targets
- Adoption Targets
- Performance Targets

---

### Discovery Questions

Ask:

- What does success look like?
- What metric proves success?
- What business result is expected?

---

## Discovery Preparation Output

Before moving into Decision Discovery, prepare a summary containing:

### Business Problem

---

### Business Capability

---

### Business Outcomes

---

### Stakeholders

---

### Human Authority

---

### Risks

---

### Success Criteria

---

## BRD Completeness Assessment

Classify BRD quality as:

### Complete

Contains sufficient information for discovery.

---

### Partially Complete

Contains useful information but requires assumptions.

---

### Discovery Risk

Contains significant gaps requiring clarification.

---

## Regression Protection Review

When existing reports are referenced, identify:

- Existing Decisions
- Existing Questions
- Existing Signals
- Existing Actions
- Existing KPIs
- Existing Story Structures

to prevent accidental loss of business knowledge.

---

## BRD Analysis Readiness Checklist

Verify:

□ Business Problem Identified

□ Business Capability Identified

□ Business Outcomes Identified

□ Stakeholders Identified

□ Human Authority Identified

□ Risks Identified

□ Success Criteria Identified

□ Existing Logic Reviewed

---

## Validation Rule

If the BRD cannot answer:

- Why does this report exist?
- What outcome should improve?
- What capability is supported?

continue discovery before proceeding.

---

## BRD Analysis Success Statement

BRD Analysis succeeds when:

Business Intent

becomes Business Context

Business Context

reveals Capabilities

Capabilities

reveal Outcomes

Outcomes

enable Decision Discovery

and the team understands the business environment before beginning report design.

---

# SECTION 06 — DECISION DISCOVERY GUIDELINES

## Purpose

Decision Discovery defines why the report exists.

The objective is to identify the decisions that improve business outcomes.

Reports should never be designed before decision discovery is complete.

Decisions become the foundation for:

- Questions
- Signals
- Thresholds
- Actions
- Stories
- Visuals

---

## Governing Rule

Every decision must support a Business Outcome.

Every report must support at least one Primary Decision.

Always follow:

Business Problem
↓
Business Capability
↓
Business Outcome
↓
Decision

before proceeding to Question Discovery.

---

## Decision Discovery Process

### Step 01

Identify Primary Decision

---

### Step 02

Identify Secondary Decisions

---

### Step 03

Identify Decision Ownership

---

### Step 04

Identify Decision Authority

---

### Step 05

Identify Decision Frequency

---

### Step 06

Identify Success Criteria

---

### Step 07

Validate Outcome Alignment

---

### Step 08

Prioritize Decisions

---

## Primary Decision Discovery

### Purpose

Identify the single most important decision supported by the report.

The Primary Decision justifies the existence of the reporting solution.

---

### Discovery Questions

Ask:

- What decision becomes easier when the report is used?
- What decision is currently difficult?
- What decision produces the greatest business value?
- What decision most directly influences the outcome?

---

### Characteristics Of A Good Primary Decision

A Primary Decision should be:

- High Value
- Actionable
- Outcome Driven
- Measurable
- Operationally Relevant

---

### Examples

```text
Which centres should receive incoming animals?

Which cases should be prioritized first?

Which regions require intervention?

Which opportunities require immediate action?
```

---

## Secondary Decision Discovery

### Purpose

Identify supporting decisions that improve the Primary Decision.

---

### Discovery Questions

Ask:

- What supporting decisions occur before the primary decision?
- What supporting decisions occur after the primary decision?
- What decisions improve confidence?
- What decisions improve prioritization?

---

### Common Secondary Decisions

Examples:

- Escalation Decisions
- Readiness Decisions
- Capacity Decisions
- Prioritization Decisions
- Governance Decisions
- Resource Allocation Decisions

---

## Decision Ownership Discovery

### Purpose

Identify who owns the decision.

---

### Discovery Questions

Ask:

- Who makes the decision today?
- Who is accountable for the outcome?
- Who is responsible for execution?

---

### Required Discovery

Identify:

- Decision Owner
- Supporting Stakeholders
- Decision Consumers

---

## Decision Authority Discovery

### Purpose

Identify final approval authority.

---

### Discovery Questions

Ask:

- Who has final authority?
- Who may approve exceptions?
- Who may override recommendations?
- Who owns escalation decisions?

---

### Required Authority Roles

Identify where applicable:

- Decision Authority
- Approval Authority
- Escalation Authority
- Governance Authority

---

## Human Accountability Validation

Decision ownership and authority should never be assumed.

Every critical decision must identify:

- Owner
- Authority
- Accountability

---

## Decision Frequency Discovery

### Purpose

Understand how often decisions occur.

---

### Discovery Questions

Ask:

- How often is the decision made?
- How quickly must the decision occur?
- How long can decisions be delayed?

---

### Examples

- Real Time
- Hourly
- Daily
- Weekly
- Monthly
- Event Driven

---

## Decision Success Criteria Discovery

### Purpose

Define what successful decision support looks like.

---

### Discovery Questions

Ask:

- How will decision quality improve?
- How will decision speed improve?
- How will operational outcomes improve?

---

### Examples

- Faster Placement Decisions
- Reduced Escalations
- Improved Capacity Utilization
- Improved Data Trust
- Improved Resource Allocation

---

## Outcome Alignment Review

Every decision should support:

Business Outcome
↓
Decision

---

### Validation Questions

Ask:

- Which outcome improves because of this decision?
- What happens if this decision improves?
- What happens if this decision is ignored?

---

## Decision Prioritization

Classify decisions as:

### Primary

Core purpose of report.

---

### Critical Secondary

High impact supporting decisions.

---

### Supporting

Context and analysis decisions.

---

## Decision Readiness Assessment

Before proceeding verify:

□ Primary Decision Defined

□ Secondary Decisions Defined

□ Decision Owner Defined

□ Decision Authority Defined

□ Decision Frequency Defined

□ Success Criteria Defined

□ Outcome Alignment Confirmed

---

## Failure Mode Review

Evaluate:

### Missing Decision Risk

What happens if the decision is not identified?

---

### Ownership Risk

What happens if nobody owns the decision?

---

### Authority Risk

What happens if approval authority is unclear?

---

### Outcome Risk

What happens if the decision does not improve outcomes?

---

## Validation Rule

If a decision lacks:

- Outcome Alignment
- Decision Owner
- Decision Authority

the decision is incomplete.

Do not proceed to Question Discovery.

---

## Decision Discovery Success Statement

Decision Discovery succeeds when:

Business Outcomes

identify Decisions

Decisions

identify Accountability

Accountability

enables Action

and stakeholders can clearly explain:

- What decision must be made?
- Why it matters?
- Who owns it?
- Who approves it?
- Which outcome it improves?

before Question Discovery begins.

---

# SECTION 07 — HUMAN AUTHORITY DISCOVERY GUIDELINES

## Purpose

Human Authority Discovery ensures accountability remains clearly defined throughout the Decision Story.

The objective is to identify:

- Decision Ownership
- Approval Authority
- Escalation Authority
- Outcome Ownership
- Accountability Boundaries

before report design proceeds.

The framework is:

AI Assisted
↓
Human Governed

Human authority must always remain explicit.

---

## Governing Rule

Every critical Decision must identify:

- Decision Owner
- Decision Authority
- Action Owner
- Escalation Authority

Accountability may never be assumed.

Accountability must be discovered and documented.

---

## Human Authority Discovery Process

### Step 01

Identify Decision Owners

---

### Step 02

Identify Outcome Owners

---

### Step 03

Identify Approval Authorities

---

### Step 04

Identify Escalation Authorities

---

### Step 05

Identify Review Authorities

---

### Step 06

Validate Accountability

---

## Decision Owner Discovery

### Purpose

Identify who owns the business decision.

---

### Discovery Questions

Ask:

- Who makes the decision today?
- Who is responsible for determining next steps?
- Who is accountable if the decision is wrong?
- Who is expected to act on report recommendations?

---

### Examples

- Operations Manager
- Regional Director
- Animal Flow Team
- Executive Leadership
- Program Manager

---

## Outcome Owner Discovery

### Purpose

Identify who is accountable for business success.

---

### Discovery Questions

Ask:

- Who owns the business outcome?
- Who reports success?
- Who is measured against the outcome?
- Who benefits from improvement?

---

### Examples

- Director Of Operations
- Executive Leadership Team
- Regional Management
- Program Leadership

---

## Approval Authority Discovery

### Purpose

Identify who holds final approval authority.

---

### Discovery Questions

Ask:

- Who approves major actions?
- Who authorizes interventions?
- Who approves exceptions?
- Who can override recommendations?

---

### Examples

- Executive Director
- Regional Director
- Operations Leadership
- Governance Committee

---

## Escalation Authority Discovery

### Purpose

Identify who owns escalation decisions.

---

### Discovery Questions

Ask:

- Who handles critical conditions?
- Who receives escalations?
- Who approves emergency interventions?
- Who resolves unresolved conflicts?

---

### Examples

- Operations Leadership
- Executive Leadership
- Regional Management
- Governance Leads

---

## Review Authority Discovery

### Purpose

Identify who validates decisions and outcomes.

---

### Discovery Questions

Ask:

- Who reviews outcome performance?
- Who validates recommendations?
- Who reviews governance concerns?
- Who reviews exceptions?

---

### Examples

- Business Owner
- Product Owner
- Steering Committee
- Governance Team

---

## Accountability Mapping

For every critical decision document:

### Decision Owner

Who makes the decision?

---

### Action Owner

Who performs the action?

---

### Outcome Owner

Who owns success?

---

### Approval Authority

Who authorizes action?

---

### Escalation Authority

Who handles exceptions?

---

## Accountability Validation

Every critical decision should answer:

```text
Who makes the decision?

Who performs the action?

Who owns the outcome?

Who approves exceptions?

Who receives escalations?
```

---

## Human-In-The-Loop Identification

Identify where human intervention is required.

Examples:

### Approval Points

Human approval required.

---

### Exception Handling

Human review required.

---

### Escalation Review

Human assessment required.

---

### Governance Review

Human validation required.

---

## AI Boundary Discovery

### Purpose

Identify where AI recommendations stop.

---

### AI May Support

- Discovery
- Analysis
- Prioritization
- Recommendation
- Explanation

---

### AI May Not Own

- Decisions
- Outcomes
- Approvals
- Escalations
- Accountability

---

## Human Authority Risk Review

Evaluate:

### Ownership Risk

What happens if no owner exists?

---

### Approval Risk

What happens if approval authority is unclear?

---

### Escalation Risk

What happens if escalation paths are undefined?

---

### Accountability Risk

What happens if ownership is shared or unclear?

---

## Human Authority Readiness Checklist

Verify:

□ Decision Owner Identified

□ Outcome Owner Identified

□ Approval Authority Identified

□ Escalation Authority Identified

□ Review Authority Identified

□ Accountability Mapping Completed

---

## Validation Rule

If a critical decision does not identify:

- Decision Owner
- Outcome Owner
- Approval Authority

the design is incomplete.

Do not proceed to Question Discovery.

---

## Human Authority Discovery Success Statement

Human Authority Discovery succeeds when:

Every Decision

has an Owner

Every Action

has an Owner

Every Outcome

has an Owner

and stakeholders can clearly determine:

- Who decides?
- Who acts?
- Who approves?
- Who escalates?
- Who is accountable?

before decision-support design begins.

The result is:

- Clear Accountability
- Human Governance
- Reduced Ambiguity
- Stronger Decision Ownership
- 
---

# SECTION 08 — QUESTION DISCOVERY GUIDELINES

## Purpose

Questions translate Decisions into information requirements.

Question Discovery identifies what users must know before they can make an informed decision.

Questions act as the bridge between:

Business Outcome
↓
Decision
↓
Question
↓
Signal

Without the correct questions, decision support becomes incomplete.

---

## Governing Rule

Every Question must support:

- A Business Outcome
- A Decision
- A User Action

Questions that do not influence decisions should not be included.

---

## Question Discovery Process

### Step 01

Review Business Outcomes

---

### Step 02

Review Decisions

---

### Step 03

Identify Explicit Questions

---

### Step 04

Identify Implied Questions

---

### Step 05

Categorize Questions

---

### Step 06

Validate Coverage

---

### Step 07

Validate Outcome Alignment

---

### Step 08

Prepare Signal Discovery Inputs

---

## Explicit Question Discovery

### Purpose

Identify questions directly documented within source materials.

---

### Sources

Review:

- BRD Requirements
- Business Goals
- Success Criteria
- Stakeholder Requests
- Existing Reports

---

### Examples

```text
Which centres can receive additional animals?

Which regions are operating above capacity?

Which animals should be prioritized for placement?
```

---

## Implied Question Discovery

### Purpose

Identify important unanswered questions implied by business needs.

Often the most valuable questions are not explicitly written.

---

### Discovery Questions

Ask:

- What must be known before making the decision?
- What evidence would increase confidence?
- What conditions affect success?
- What conditions create risk?

---

### Examples

Business Request:

```text
Improve placement speed.
```

Implied Questions:

```text
Which centres have excess capacity?

Which animals have exceeded target placement time?

What operational factors slow placement?
```

---

## Outcome Alignment Discovery

### Purpose

Ensure questions support measurable outcomes.

---

### Discovery Questions

Ask:

- What outcome does this question support?
- How does answering this question improve the outcome?
- What decision becomes easier because this question is answered?

---

## Question Categories

Review coverage across the following areas.

### Operational Questions

Purpose:

Support day-to-day decisions.

Examples:

```text
What requires immediate attention?

Which workload should be prioritized?
```

---

### Capacity Questions

Purpose:

Support resource planning and utilization.

Examples:

```text
Where is capacity available?

Where are constraints emerging?
```

---

### Risk Questions

Purpose:

Support proactive intervention.

Examples:

```text
What conditions create risk?

What requires escalation?
```

---

### Governance Questions

Purpose:

Support compliance and oversight.

Examples:

```text
Are business rules being followed?

Are approvals required?
```

---

### Trust Questions

Purpose:

Support confidence in decision making.

Examples:

```text
Can the information be trusted?

Is the data complete?
```

---

### Regional Questions

Purpose:

Support geographic monitoring.

Examples:

```text
Which regions require intervention?

Where are pressures increasing?
```

---

### Executive Questions

Purpose:

Support strategic oversight.

Examples:

```text
Are business outcomes improving?

Where should leadership focus attention?
```

---

## Human Authority Alignment

Every Question should support:

Human Decision Making

not automated decision making.

---

### Review Questions

Ask:

- Who uses the answer?
- Which stakeholder benefits?
- Which decision owner depends on the answer?
- Which authority role requires visibility?

---

## Coverage Discovery

Verify:

### Decision Coverage

Every Decision has supporting questions.

---

### Outcome Coverage

Every Outcome has supporting questions.

---

### Risk Coverage

Major business risks are represented.

---

### Trust Coverage

Major data trust concerns are represented.

---

### Action Coverage

Questions support future actions.

---

## Failure-Aware Question Discovery

Evaluate:

### Missing Question Risk

What decision becomes harder if this question is omitted?

---

### Ambiguous Question Risk

Can business users interpret the question differently?

---

### Unanswerable Question Risk

Can available signals answer the question?

---

### Ownership Risk

Is there a responsible decision owner for the answer?

---

## Question Quality Standards

Good Questions are:

- Outcome Aligned
- Decision Relevant
- Actionable
- Measurable
- Explainable

---

Poor Questions are:

- Interesting But Irrelevant
- Data Curiosity Questions
- Questions Without Decisions
- Questions Without Actions

---

## Question Validation

Every Question must:

- Support A Business Outcome
- Support A Decision
- Support Human Action
- Be Measurable
- Be Explainable
- Be Traceable

---

## Question Readiness Checklist

Verify:

□ Outcome Supported

□ Decision Supported

□ Action Supported

□ Question Clearly Defined

□ Question Measurable

□ Coverage Reviewed

□ Traceability Preserved

---

## Validation Rule

If a Question does not support:

- A Business Outcome
- A Decision
- A Human Action

Remove It.

Do not proceed to Signal Discovery.

---

## Question Discovery Success Statement

Question Discovery succeeds when:

Business Outcomes

drive Decisions

Decisions

drive Questions

Questions

drive Signals

and stakeholders can clearly explain:

- What must be known?
- Why must it be known?
- Which decision depends on it?
- Which action becomes easier?

before Signal Discovery begins.

---

# SECTION 09 — SIGNAL DISCOVERY GUIDELINES

## Purpose

Signals provide evidence used to answer Business Questions and support Business Decisions.

Signals convert information needs into measurable business indicators.

Signal Discovery identifies:

- What should be measured
- What should be monitored
- What requires attention
- What supports decision making

Signals should provide trusted evidence for action.

---

## Governing Rule

Every Signal must support:

- A Business Outcome
- A Decision
- A Business Question
- A Human Action

Signals that do not influence decisions should not be included.

---

## Signal Discovery Process

### Step 01

Review Business Outcomes

---

### Step 02

Review Decisions

---

### Step 03

Review Business Questions

---

### Step 04

Identify Candidate Signals

---

### Step 05

Identify Decision Signals

---

### Step 06

Identify Critical Signals

---

### Step 07

Validate Signal Trust

---

### Step 08

Prepare Threshold Design Inputs

---

## Signal Discovery Framework

Apply:

Question
↓
Potential Signals
↓
Decision Signals
↓
Critical Signals

The objective is to discover the smallest set of signals necessary to support quality decisions.

---

## Candidate Signal Discovery

### Purpose

Identify all possible indicators capable of answering a question.

---

### Discovery Questions

Ask:

- What evidence would answer the question?
- What measurable indicator exists?
- What information would increase decision confidence?
- What condition should be monitored?

---

### Example

Question:

```text
Which centres can receive incoming animals?
```

Potential Signals:

```text
Available Capacity

Current Occupancy

Utilization Percentage

Open Kennels
```

---

## Decision Signal Identification

### Purpose

Identify signals that directly influence decisions.

---

### Discovery Questions

Ask:

- Which signal changes the decision?
- Which signal changes prioritization?
- Which signal affects action selection?
- Which signal affects escalation?

---

### Validation

If the signal does not influence a decision:

```text
Supporting Signal Only
```

or

```text
Remove Signal
```

---

## Critical Signal Identification

### Purpose

Identify signals that are essential to decision quality.

---

### Discovery Questions

Ask:

- What signal is absolutely required?
- What signal creates the greatest impact?
- What signal creates the greatest risk if missing?

---

### Classification

#### Critical

Decision quality significantly degrades without it.

---

#### Important

Improves confidence.

Decision still possible.

---

#### Supporting

Provides context and explanation.

---

## Signal Classification

Classify signals across one or more categories.

### Operational

Supports daily operations.

Examples:

- Active Cases
- Capacity Available
- Queue Length

---

### Capacity

Supports planning and utilization decisions.

Examples:

- Occupancy
- Open Capacity
- Resource Availability

---

### Risk

Supports early warning and intervention.

Examples:

- Escalation Count
- Capacity Pressure
- SLA Risk

---

### Governance

Supports compliance and policy validation.

Examples:

- Approval Status
- Policy Compliance

---

### Data Quality

Supports data trust.

Examples:

- Freshness Status
- Completeness Score
- Validation Status

---

### Regional

Supports geographic monitoring.

Examples:

- Regional Utilization
- Regional Demand

---

### Executive

Supports leadership oversight.

Examples:

- Strategic KPI Status
- Outcome Achievement

---

## Signal Trust Discovery

### Purpose

Determine whether business users can trust the signal.

---

### Discovery Questions

Ask:

- Is the signal consistently available?
- Is the signal understood by users?
- Is the signal governed?
- Is the signal explainable?

---

### Trust Indicators

Review:

- Source Quality
- Refresh Frequency
- Definition Clarity
- Calculation Stability

---

## Signal Ownership Discovery

### Purpose

Identify who owns the signal definition and business interpretation.

---

### Discovery Questions

Ask:

- Who defines the signal?
- Who validates the signal?
- Who relies on the signal?

---

### Examples

- Business Owner
- Operations Team
- Reporting Team
- Governance Team

---

## Outcome Alignment Review

Every Signal should support:

Business Outcome
↓
Decision
↓
Question
↓
Signal

---

### Validation Questions

Ask:

- What outcome does this signal support?
- What decision depends on it?
- What question does it answer?

---

## Human Authority Alignment

Signals are evidence.

Humans remain decision makers.

---

### Ask

- Which decision owner uses this signal?
- Which stakeholder relies on it?
- Which authority role requires visibility?

---

## Failure-Aware Signal Discovery

Evaluate:

### Missing Signal Risk

What happens if the signal is unavailable?

---

### Incorrect Signal Risk

What happens if the signal is wrong?

---

### Stale Signal Risk

What happens if the signal is outdated?

---

### Misinterpretation Risk

Could business users interpret the signal differently?

---

### Trust Risk

Could low-quality data reduce confidence?

---

## Signal Quality Standards

Good Signals are:

- Outcome Aligned
- Decision Relevant
- Measurable
- Explainable
- Actionable
- Trusted

---

Poor Signals are:

- Vanity Metrics
- Decorative KPIs
- Orphan Signals
- Unused Measures
- Metrics With No Decision Value

---

## Signal Readiness Checklist

Verify:

□ Business Outcome Supported

□ Decision Supported

□ Question Supported

□ Signal Defined

□ Signal Measurable

□ Signal Explainable

□ Signal Trust Reviewed

□ Signal Priority Assigned

---

## Validation Rule

If a Signal does not support:

- A Business Outcome
- A Decision
- A Question

Remove It.

Do not proceed to Threshold Design.

---

## Signal Discovery Success Statement

Signal Discovery succeeds when:

Business Outcomes

drive Decisions

Decisions

drive Questions

Questions

drive Signals

and stakeholders can clearly explain:

- What is being measured?
- Why is it being measured?
- Which decision depends on it?
- Which outcome improves because of it?

before Threshold Design begins.

---

# SECTION 10 — THRESHOLD DESIGN GUIDELINES

## Purpose

Thresholds convert Signals into business meaning and action.

Signals tell users what is happening.

Thresholds tell users:

- Why it matters
- How serious it is
- What should happen next

Thresholds transform information into decision guidance.

---

## Governing Rule

Every critical Signal should have a Threshold.

Every Threshold should support:

- A Business Outcome
- A Decision
- A Human Action

Thresholds that do not influence action should not be created.

---

## Threshold Design Process

### Step 01

Review Business Outcomes

---

### Step 02

Review Decisions

---

### Step 03

Review Signals

---

### Step 04

Identify Business Interpretation

---

### Step 05

Define Status States

---

### Step 06

Define Action Triggers

---

### Step 07

Define Escalation Logic

---

### Step 08

Validate Threshold Effectiveness

---

## Threshold Discovery Framework

Apply:

Signal
↓
Threshold
↓
Status
↓
Action
↓
Business Meaning

Every threshold should improve decision speed and consistency.

---

## Business Interpretation Discovery

### Purpose

Define the business meaning behind signal values.

---

### Discovery Questions

Ask:

- What does a good result look like?
- What indicates risk?
- What indicates intervention is required?
- What business condition is represented?

---

### Example

Signal:

```text
Capacity Utilization
```

Interpretation:

```text
Low Utilization
= Underused Capacity

Target Utilization
= Healthy Operations

High Utilization
= Capacity Risk
```

---

## Status Design

### Purpose

Standardize interpretation.

---

### Healthy

Condition is acceptable.

Typical Actions:

```text
Monitor

Continue

Maintain
```

---

### Warning

Condition requires attention.

Typical Actions:

```text
Review

Investigate

Prepare Response
```

---

### Critical

Condition requires intervention.

Typical Actions:

```text
Escalate

Intervene

Take Immediate Action
```

---

### Exception

Condition falls outside standard business rules.

Typical Actions:

```text
Special Review

Manual Approval

Governance Assessment
```

---

## Threshold Definition Discovery

### Discovery Questions

Ask:

- At what point should concern begin?
- At what point should action occur?
- At what point should escalation occur?
- What level creates business risk?

---

### Sources

Use:

- Business Rules
- Operational Procedures
- SME Knowledge
- Existing Governance Rules
- Existing Reporting Logic

where available.

---

## Action Trigger Discovery

### Purpose

Define the behavior expected when a threshold is reached.

---

### Discovery Questions

Ask:

- What should happen next?
- Who should respond?
- Is escalation required?
- Is approval required?

---

### Examples

Healthy:

```text
Continue Monitoring
```

---

Warning:

```text
Perform Review
```

---

Critical:

```text
Escalate To Leadership
```

---

Exception:

```text
Manual Intervention Required
```

---

## Escalation Discovery

### Purpose

Identify when additional authority is required.

---

### Discovery Questions

Ask:

- When does leadership need visibility?
- When is operational intervention required?
- When should governance become involved?

---

### Escalation Levels

Level 1

```text
Awareness
```

---

Level 2

```text
Operational Review
```

---

Level 3

```text
Management Escalation
```

---

Level 4

```text
Critical Intervention
```

---

## Human Authority Alignment

Thresholds should identify:

- Action Owner
- Escalation Owner
- Decision Authority

where applicable.

---

### Discovery Questions

Ask:

- Who responds to warnings?
- Who responds to critical conditions?
- Who approves major actions?

---

## Outcome Alignment Review

Every threshold should support:

Business Outcome
↓
Decision
↓
Signal
↓
Threshold

---

### Validation Questions

Ask:

- What outcome does the threshold protect?
- What decision does it influence?
- What action becomes easier?

---

## Failure-Aware Threshold Design

Evaluate:

### False Positive Risk

Could the threshold trigger unnecessary action?

---

### False Negative Risk

Could the threshold fail to identify risk?

---

### Stale Signal Risk

Could outdated data invalidate the threshold?

---

### Rule Change Risk

Could business rule changes invalidate the threshold?

---

### Escalation Failure Risk

Could critical conditions go unnoticed?

---

## Threshold Quality Standards

Good Thresholds are:

- Actionable
- Explainable
- Governed
- Outcome Aligned
- Consistent
- Easy To Interpret

---

Poor Thresholds are:

- Arbitrary
- Unexplained
- Unused
- Unsupported By Business Rules
- Difficult To Interpret

---

## Threshold Readiness Checklist

Verify:

□ Business Outcome Supported

□ Decision Supported

□ Signal Supported

□ Status Logic Defined

□ Action Triggers Defined

□ Escalations Defined

□ Business Meaning Defined

---

## Validation Rule

If a Threshold cannot answer:

```text
What Happened?

Why Does It Matter?

What Should Be Done?
```

the Threshold is incomplete.

Do not proceed to Action Discovery.

---

## Threshold Design Success Statement

Threshold Design succeeds when:

Business Outcomes

drive Decisions

Decisions

drive Signals

Signals

drive Thresholds

Thresholds

drive Actions

and stakeholders can immediately determine:

- What happened?
- Why it matters?
- What should occur next?
- Who should respond?

before Action Discovery begins.

---

# SECTION 11 — ACTION DISCOVERY GUIDELINES

## Purpose

Actions define the operational purpose of reporting.

Reports exist to improve decisions.

Decisions exist to improve actions.

Action Discovery identifies:

- What should happen next
- Who should respond
- Who is accountable
- How outcomes improve

A report without actions provides information but does not create business value.

---

## Governing Rule

Every Decision must support at least one Action.

Every Action must support at least one Business Outcome.

Actions that do not improve outcomes should be removed.

---

## Action Discovery Process

### Step 01

Review Business Outcomes

---

### Step 02

Review Decisions

---

### Step 03

Review Questions

---

### Step 04

Review Signals

---

### Step 05

Review Thresholds

---

### Step 06

Identify Business Responses

---

### Step 07

Identify Action Owners

---

### Step 08

Validate Outcome Alignment

---

## Action Discovery Framework

Apply:

Business Outcome
↓
Decision
↓
Signal
↓
Threshold
↓
Action

Actions should represent the operational response to business conditions.

---

## Business Response Discovery

### Purpose

Identify what business users should do when conditions occur.

---

### Discovery Questions

Ask:

- What should happen if conditions are healthy?
- What should happen if conditions worsen?
- What should happen if intervention is required?
- What should happen if escalation is required?

---

### Example

Threshold:

```text
Capacity Utilization > 95%
```

Potential Responses:

```text
Pause Intake

Review Capacity

Escalate To Leadership

Reallocate Resources
```

---

## Action Definition Structure

Every Action should define:

- Condition
- Recommended Action
- Responsible Role
- Expected Outcome
- Decision Supported

---

### Condition

The event that triggers action.

Examples:

```text
Capacity Exceeded

Escalation Required

Data Trust Failed

SLA At Risk
```

---

### Recommended Action

The business response.

Examples:

```text
Perform Review

Escalate Issue

Pause Intake

Allocate Resources
```

---

### Responsible Role

The individual or team responsible for execution.

Examples:

```text
Operations Team

Regional Manager

Executive Leadership

Data Steward
```

---

### Expected Outcome

The business result expected after action occurs.

Examples:

```text
Reduced Risk

Improved Capacity

Improved Trust

Improved Service Delivery
```

---

### Decision Supported

The decision improved by the action.

Examples:

```text
Resource Allocation

Capacity Planning

Operational Prioritization

Governance Review
```

---

## Action Ownership Discovery

### Purpose

Identify who owns execution.

---

### Discovery Questions

Ask:

- Who performs the action?
- Who monitors completion?
- Who owns the operational response?
- Who is accountable for execution?

---

### Required Ownership

Identify:

- Action Owner
- Execution Team
- Accountability Owner

---

## Outcome Alignment Discovery

### Purpose

Ensure actions improve outcomes.

---

### Discovery Questions

Ask:

- What outcome improves if this action occurs?
- What outcome worsens if the action is ignored?
- How does the action support business goals?

---

### Validation

Every Action should support:

Business Outcome
↓
Decision
↓
Action

---

## Escalation Ownership Discovery

### Purpose

Identify who responds when normal actions are insufficient.

---

### Discovery Questions

Ask:

- Who receives escalations?
- Who approves interventions?
- Who resolves conflicts?
- Who owns critical incidents?

---

### Examples

- Operations Manager
- Regional Director
- Executive Leadership
- Governance Committee

---

## Action Effectiveness Discovery

### Purpose

Evaluate whether actions create meaningful business value.

---

### Discovery Questions

Ask:

- Does the action reduce risk?
- Does the action improve efficiency?
- Does the action improve decision quality?
- Does the action improve outcomes?

---

### Effectiveness Indicators

Examples:

```text
Reduced Escalations

Reduced Delays

Improved Capacity

Improved Compliance
```

---

## Human Authority Alignment

Every Action should identify:

### Action Owner

Who performs the action?

---

### Decision Authority

Who approves the action?

---

### Escalation Authority

Who handles critical situations?

---

### Outcome Owner

Who owns business success?

---

## Failure Recovery Discovery

### Purpose

Identify responses to common failures.

---

### Discovery Questions

Ask:

- What happens if the action fails?
- What happens if execution is delayed?
- What happens if nobody responds?
- What recovery action exists?

---

### Recovery Examples

```text
Escalation

Manual Review

Secondary Approval

Emergency Intervention
```

---

## Failure-Aware Action Discovery

Evaluate:

### Execution Risk

Could the action fail?

---

### Ownership Risk

Could ownership be unclear?

---

### Delay Risk

Could action timing affect outcomes?

---

### Outcome Risk

Could actions fail to improve outcomes?

---

### Escalation Risk

Could critical situations remain unresolved?

---

## Action Quality Standards

Good Actions are:

- Outcome Aligned
- Decision Driven
- Human Executable
- Measurable
- Governed
- Accountable

---

Poor Actions are:

- Vague
- Unowned
- Unmeasurable
- Unnecessary
- Disconnected From Outcomes

---

## Action Readiness Checklist

Verify:

□ Business Outcome Supported

□ Decision Supported

□ Threshold Supported

□ Action Defined

□ Action Owner Defined

□ Accountability Defined

□ Outcome Alignment Confirmed

□ Escalation Ownership Confirmed

---

## Validation Rule

If an Action lacks:

- An Owner
- A Business Outcome
- A Supported Decision

the Action is incomplete.

Do not proceed to Story Design.

---

## Action Discovery Success Statement

Action Discovery succeeds when:

Business Outcomes

drive Decisions

Decisions

drive Actions

Actions

improve Outcomes

and stakeholders can clearly explain:

- What should happen?
- Who should do it?
- Why should it happen?
- What outcome improves?

before Story Design begins.

# SECTION 12 — STORY DESIGN GUIDELINES

## Purpose

Story Design converts business logic into a decision journey.

The objective is not to present information.

The objective is to help users:

- Understand Business Conditions
- Evaluate Risks
- Assess Readiness
- Make Decisions
- Take Action

Stories transform business logic into business understanding.

---

## Governing Rule

Every Story must support:

- A Business Outcome
- A Decision
- A User Action

Stories that do not improve decision quality should not be included.

---

## Story Design Process

### Step 01

Review Business Outcomes

---

### Step 02

Review Decisions

---

### Step 03

Review Questions

---

### Step 04

Review Signals

---

### Step 05

Review Actions

---

### Step 06

Identify Story Purpose

---

### Step 07

Define Story Sequence

---

### Step 08

Validate Story Coverage

---

## Story Design Framework

Apply:

Business Outcome
↓
Decision
↓
Question
↓
Signal
↓
Action
↓
Story

Stories communicate the decision journey.

Stories do not replace the decision journey.

---

## Story Purpose Discovery

### Purpose

Identify why the story section exists.

---

### Discovery Questions

Ask:

- What should users understand?
- What decision should become easier?
- What action should become clearer?
- What outcome should improve?

---

### Validation

Every Story should justify its existence through:

```text
Outcome

Decision

Action
```

alignment.

---

## Outcome-Aligned Story Design

### Purpose

Ensure every Story supports measurable business improvement.

---

### Discovery Questions

Ask:

- Which Business Outcome does this Story support?
- Which Decision does this Story support?
- Which Action becomes easier because of this Story?

---

### Validation

Every Story should support:

Business Outcome
↓
Decision
↓
Story

---

## Story Narrative Structure

Story sections should generally progress through:

Context
↓
Attention Required
↓
Decision Readiness
↓
Decision Prioritization
↓
Analysis
↓
Trust Validation
↓
Operational Awareness
↓
Action

The story should feel natural and intentional.

---

## Story Audience Discovery

### Purpose

Identify who consumes the story.

---

### Discovery Questions

Ask:

- Who makes decisions?
- Who acts on recommendations?
- Who needs visibility?
- Who owns outcomes?

---

### Common Audiences

- Operations Teams
- Supervisors
- Leadership Teams
- Regional Management
- Executive Stakeholders
- Governance Teams

---

## Human Authority Visibility

Stories should clearly communicate:

- Decision Ownership
- Action Ownership
- Escalation Ownership
- Approval Responsibilities

where relevant.

---

### Discovery Questions

Ask:

- Who owns the decision?
- Who owns the action?
- Who approves exceptions?
- Who handles escalation?

---

## Story Sequencing Guidelines

Story sections should answer questions in this order:

### Context

```text
What is happening?
```

---

### Attention

```text
What requires attention?
```

---

### Readiness

```text
Can we act?
```

---

### Prioritization

```text
What should happen first?
```

---

### Explanation

```text
Why is this happening?
```

---

### Trust

```text
Can we trust the information?
```

---

### Awareness

```text
Where are risks and opportunities?
```

---

### Action

```text
What should happen next?
```

---

## Failure Mode Story Coverage

### Purpose

Ensure stories communicate business risks.

---

### Discovery Questions

Ask:

- What could prevent success?
- What could reduce trust?
- What could delay action?
- What could create poor decisions?

---

### Story Coverage Examples

- Capacity Risks
- Governance Issues
- Escalation Conditions
- Trust Concerns
- Outcome Risks

---

## Story Coverage Validation

Review:

### Outcome Coverage

Is every business outcome represented?

---

### Decision Coverage

Is every critical decision represented?

---

### Action Coverage

Is every critical action represented?

---

### Risk Coverage

Are business risks represented?

---

### Trust Coverage

Are trust concerns represented?

---

## Story Quality Standards

Good Stories are:

- Outcome Aligned
- Decision Focused
- Action Oriented
- Explainable
- Governed
- Traceable

---

Poor Stories are:

- Data Dumps
- Visual Collections
- Unstructured Analysis
- Information Without Purpose
- Content Without Decisions

---

## Story Traceability Review

Verify:

Business Outcome
↓
Decision
↓
Question
↓
Signal
↓
Action
↓
Story

remains intact.

---

## Story Readiness Checklist

Verify:

□ Business Outcome Supported

□ Decision Supported

□ Action Supported

□ Story Purpose Defined

□ Story Sequence Defined

□ Audience Defined

□ Human Authority Visible

□ Risk Coverage Reviewed

---

## Validation Rule

If a Story does not support:

- A Business Outcome
- A Decision
- A User Action

remove or redesign the Story.

Do not proceed to Story Construction.

---

## Story Design Success Statement

Story Design succeeds when:

Business Outcomes

drive Decisions

Decisions

drive Actions

Actions

drive Stories

and stakeholders can clearly understand:

- What is happening?
- Why it matters?
- What decision must be made?
- What action should occur?
- Who is accountable?

before Story Construction begins.

---

# SECTION 13 — STORY CONSTRUCTION FRAMEWORK

## Purpose

Provide a repeatable methodology for constructing Story sections from approved business design.

Story Construction transforms:

Business Outcomes
↓
Decisions
↓
Questions
↓
Signals
↓
Actions

into a structured user experience.

The goal is to communicate decision support consistently across all reporting solutions.

---

## Governing Rule

Every Story section must exist for a business purpose.

Every Story section must support:

- A Business Outcome
- A Decision
- A User Action

Story sections that do not improve decision quality should not be included.

---

## Story Construction Sequence

Construct Story sections in the following order:

### Story 0

Executive Context

↓

### Story 1

Action Required

↓

### Story 2

Decision Readiness

↓

### Story 3

Decision Prioritization

↓

### Story 4

Analysis And Explanation

↓

### Story 5

Data Trust

↓

### Story 6

Regional Monitoring

↓

### Story 7

Operational Briefing

---

## Story 0 — Executive Context

### Purpose

Provide organizational awareness and business context.

---

### Primary Questions

```text
What is happening?

Why should leadership care?
```

---

### Required Coverage

- Business Outcome Status
- Strategic Objectives
- Overall Health
- Major Trends
- High-Level Risks

---

### Human Authority Visibility

Identify:

- Outcome Owner
- Executive Sponsor
- Strategic Accountability

---

### Success Criteria

Leadership should understand the current situation within seconds.

---

## Story 1 — Action Required

### Purpose

Highlight immediate attention areas.

---

### Primary Questions

```text
What requires attention?

What requires intervention?
```

---

### Required Coverage

- Critical Exceptions
- Escalations
- Warning Conditions
- Urgent Risks

---

### Human Authority Visibility

Identify:

- Escalation Owner
- Decision Authority
- Responsible Teams

---

### Success Criteria

Users immediately identify priorities.

---

## Story 2 — Decision Readiness

### Purpose

Determine whether decisions can safely be made.

---

### Primary Questions

```text
Are we ready to act?

Are required conditions satisfied?
```

---

### Required Coverage

- Eligibility
- Readiness Conditions
- Required Inputs
- Approval Status

---

### Human Authority Visibility

Identify:

- Approval Authority
- Review Authority
- Governance Ownership

---

### Success Criteria

Users understand whether action may proceed.

---

## Story 3 — Decision Prioritization

### Purpose

Help users rank opportunities, responses, and actions.

---

### Primary Questions

```text
What should happen first?

What is most important?
```

---

### Required Coverage

- Priority Rankings
- Capacity Constraints
- Resource Allocation
- Action Recommendations

---

### Human Authority Visibility

Identify:

- Resource Owners
- Decision Owners
- Priority Approvers

---

### Success Criteria

Users can confidently determine priorities.

---

## Story 4 — Analysis And Explanation

### Purpose

Explain underlying business conditions.

---

### Primary Questions

```text
Why is this happening?
```

---

### Required Coverage

- Root Causes
- Trends
- Comparisons
- Contributing Factors

---

### Failure Mode Coverage

Include visibility into:

- Emerging Risks
- Process Failures
- Constraint Impacts
- Operational Failure Drivers

---

### Success Criteria

Users understand why conditions exist.

---

## Story 5 — Data Trust

### Purpose

Establish confidence in decision making.

---

### Primary Questions

```text
Can this information be trusted?
```

---

### Required Coverage

- Data Freshness
- Completeness
- Quality Indicators
- Governance Indicators

---

### Failure Mode Coverage

Include visibility into:

- Data Quality Risks
- Validation Failures
- Trust Concerns

---

### Success Criteria

Users understand confidence levels before acting.

---

## Story 6 — Regional Monitoring

### Purpose

Identify geographic or organizational patterns.

---

### Primary Questions

```text
Where are opportunities or risks emerging?
```

---

### Required Coverage

- Regional Comparisons
- Local Trends
- Resource Distribution
- Capacity Distribution

---

### Human Authority Visibility

Identify:

- Regional Ownership
- Regional Accountability
- Escalation Responsibilities

---

### Success Criteria

Users can determine where intervention is required.

---

## Story 7 — Operational Briefing

### Purpose

Convert findings into action.

---

### Primary Questions

```text
What should happen next?

Who should act?
```

---

### Required Coverage

- Recommended Actions
- Action Owners
- Escalations
- Follow-Up Activities

---

### Human Authority Visibility

Identify:

- Action Owner
- Decision Owner
- Escalation Authority

---

### Success Criteria

Users leave with a clear understanding of next steps.

---

## Outcome Coverage Validation

Collectively all Story sections should explain:

- Business Problem
- Business Capability
- Business Outcomes
- Decision Logic
- Recommended Actions

No outcome should be unsupported by Story coverage.

---

## Failure Mode Coverage Validation

Collectively all Story sections should address:

- Decision Risks
- Operational Risks
- Trust Risks
- Escalation Risks
- Outcome Risks

Major failure conditions should not remain hidden.

---

## Handoff Readiness Construction

The completed Story framework should provide sufficient detail for:

- Mockup Design
- TRD Development
- Semantic Design
- Report Build

without revisiting discovery activities.

---

## Story Construction Readiness Checklist

Verify:

□ Story 0 Defined

□ Story 1 Defined

□ Story 2 Defined

□ Story 3 Defined

□ Story 4 Defined

□ Story 5 Defined

□ Story 6 Defined

□ Story 7 Defined

□ Outcome Coverage Complete

□ Human Authority Visible

□ Failure Modes Covered

□ Handoff Readiness Achieved

---

## Validation Rule

If users cannot answer:

```text
What is happening?

Why is it happening?

What requires attention?

What decision is required?

What action should occur?
```

the Story framework is incomplete.

---

## Story Construction Success Statement

Story Construction succeeds when:

Business Outcomes

drive Decisions

Decisions

drive Actions

Actions

drive Stories

and users naturally progress from:

Context
↓
Attention
↓
Assessment
↓
Decision
↓
Action

while maintaining visibility into:

- Outcomes
- Accountability
- Risks
- Trust
- Priorities

throughout the experience.

---

# SECTION 14 — PAGE ARCHETYPE GUIDELINES

## Purpose

Page Archetypes represent proven decision-support patterns.

The purpose of archetype selection is to ensure report experiences are designed around:

Business Outcomes
↓
Decisions
↓
Actions

rather than:

Visual Preferences
↓
Dashboard Layouts
↓
Technology Constraints

Archetypes provide a consistent decision-support experience across all reporting solutions.

---

## Governing Rule

Select archetypes based on:

- Business Outcomes
- Decisions
- User Actions
- Operational Needs

Do not select archetypes because:

- A visual is preferred
- A layout is familiar
- A previous report used it
- A tool makes it easy

Business purpose must always drive archetype choice.

---

## Archetype Selection Process

### Step 01

Review Business Outcomes

---

### Step 02

Review Primary Decision

---

### Step 03

Review User Actions

---

### Step 04

Review Story Structure

---

### Step 05

Select Archetype

---

### Step 06

Validate Decision Support

---

### Step 07

Validate Outcome Alignment

---

## Archetype Discovery Framework

Apply:

Business Outcome
↓
Decision
↓
Story
↓
Archetype

Archetypes should support how users make decisions.

---

## Operational Command Centre

### Purpose

Support rapid operational decision making.

---

### Best For

- Daily Operations
- Work Management
- Exception Handling
- Intake Decisions
- Assignment Decisions

---

### Typical Characteristics

- High Visibility
- Action Focused
- Prioritized Information
- Immediate Intervention Support

---

### Discovery Questions

Ask:

- Are rapid decisions required?
- Are operational teams the primary audience?
- Is real-time monitoring important?

---

## Capacity Intelligence

### Purpose

Support resource planning and utilization decisions.

---

### Best For

- Capacity Planning
- Supply And Demand
- Resource Allocation
- Utilization Monitoring

---

### Typical Characteristics

- Comparative Analysis
- Constraint Identification
- Availability Monitoring
- Planning Support

---

### Discovery Questions

Ask:

- Is capacity the primary concern?
- Does utilization influence decisions?
- Are allocation choices required?

---

## Executive Monitoring

### Purpose

Support leadership and strategic oversight.

---

### Best For

- Executive Review
- Strategic Planning
- Outcome Monitoring
- Organizational Performance

---

### Typical Characteristics

- Outcome Focused
- Aggregated Information
- Strategic Trends
- High-Level Risks

---

### Discovery Questions

Ask:

- Is strategic decision making the primary goal?
- Do leaders require visibility?
- Are business outcomes the focus?

---

## Exception Management

### Purpose

Highlight situations requiring intervention.

---

### Best For

- Escalations
- Operational Issues
- Governance Violations
- Critical Risks

---

### Typical Characteristics

- Risk Visibility
- Escalation Focus
- Prioritized Exceptions
- Action Orientation

---

### Discovery Questions

Ask:

- What requires immediate attention?
- Which conditions require intervention?
- Which risks require escalation?

---

## Regional Monitoring

### Purpose

Support geographic and organizational awareness.

---

### Best For

- Regional Performance
- Resource Distribution
- Capacity Distribution
- Risk Monitoring

---

### Typical Characteristics

- Comparative Analysis
- Regional Trends
- Distribution Monitoring
- Intervention Targeting

---

### Discovery Questions

Ask:

- Are regional comparisons important?
- Are organizational differences significant?
- Is location-based intervention required?

---

## Performance Monitoring

### Purpose

Track progress toward goals and outcomes.

---

### Best For

- KPI Monitoring
- Performance Management
- Outcome Tracking
- Target Achievement

---

### Typical Characteristics

- KPI Focused
- Trend Visibility
- Goal Tracking
- Progress Measurement

---

### Discovery Questions

Ask:

- Are outcomes being measured?
- Are performance targets important?
- Are KPI trends required?

---

## Data Quality Investigation

### Purpose

Support trust validation and governance review.

---

### Best For

- Data Quality Analysis
- Governance Monitoring
- Trust Validation
- Issue Resolution

---

### Typical Characteristics

- Trust Focused
- Validation Oriented
- Governance Visibility
- Root Cause Support

---

### Discovery Questions

Ask:

- Does data quality affect decisions?
- Are trust concerns significant?
- Is governance visibility required?

---

## Outcome Alignment Review

Every selected archetype should support:

Business Outcome
↓
Decision
↓
Action
↓
Archetype

---

### Validation Questions

Ask:

- Which outcome is improved?
- Which decision is supported?
- Which action becomes easier?

---

## Human Authority Visibility

Selected archetypes should make accountability visible.

Where appropriate ensure visibility of:

- Decision Owners
- Action Owners
- Approval Authorities
- Escalation Authorities

---

## Failure Mode Visibility

Selected archetypes should support visibility into:

- Operational Risks
- Capacity Risks
- Trust Risks
- Governance Risks
- Escalation Conditions

Important issues should never be hidden.

---

## Story Alignment Review

Every archetype should support the approved Story framework.

Validate alignment with:

- Executive Context
- Action Required
- Decision Readiness
- Prioritization
- Analysis
- Trust
- Regional Awareness
- Action

---

## Handoff Readiness Review

Archetype decisions should provide sufficient clarity for:

- Mockup Design
- TRD Development
- Semantic Design
- Report Build

without requiring re-discovery.

---

## Archetype Quality Standards

Good Archetypes are:

- Outcome Aligned
- Decision Focused
- Action Oriented
- Explainable
- Consistent
- Governed

---

Poor Archetypes are:

- Visual Driven
- Tool Driven
- Trend Driven
- Unrelated To Decisions
- Unrelated To Outcomes

---

## Archetype Readiness Checklist

Verify:

□ Business Outcome Supported

□ Decision Supported

□ Story Supported

□ User Action Supported

□ Human Authority Visible

□ Failure Visibility Considered

□ Handoff Ready

---

## Validation Rule

If an archetype cannot explain:

- What outcome it supports
- What decision it supports
- What action it enables

the archetype selection should be reconsidered.

---

## Page Archetype Success Statement

Page Archetype Discovery succeeds when:

Business Outcomes

drive Decisions

Decisions

drive Stories

Stories

drive Archetypes

and stakeholders can clearly explain:

- Why this archetype was selected
- What decision it supports
- What action it enables
- What outcome it improves

before Layout Design begins.

---

# SECTION 15 — LAYOUT BLUEPRINT GUIDELINES

## Purpose

Layout Design defines how the Decision Story is consumed.

The objective is not to arrange visuals.

The objective is to arrange information so users can:

- Understand Business Context
- Identify What Requires Attention
- Evaluate Decisions
- Understand Risks
- Take Action

Layout should guide users through the decision process naturally.

---

## Governing Rule

Layout must be derived from:

Business Outcome
↓
Decision
↓
Story
↓
Layout

Never derive layout from:

Visual
↓
Dashboard
↓
Decision

Story drives Layout.

Layout does not drive Story.

---

## Layout Design Process

### Step 01

Review Business Outcomes

---

### Step 02

Review Decisions

---

### Step 03

Review Approved Story Structure

---

### Step 04

Define Reading Order

---

### Step 05

Define Information Hierarchy

---

### Step 06

Define Escalation Visibility

---

### Step 07

Define Authority Visibility

---

### Step 08

Validate Layout Flow

---

## Layout Blueprint Framework

Apply:

Business Outcome
↓
Decision
↓
Story
↓
Layout
↓
Visual

The Layout should reinforce the Decision Story.

---

## Reading Order Design

### Purpose

Guide users through a defined decision journey.

---

### Preferred Reading Flow

Context
↓
Attention Required
↓
Decision Readiness
↓
Decision Prioritization
↓
Analysis
↓
Trust Validation
↓
Regional Awareness
↓
Action

---

### Validation Questions

Ask:

- What should users see first?
- What should users understand second?
- When should decisions appear?
- When should actions appear?

---

## Information Hierarchy Design

### Purpose

Ensure important information appears before supporting information.

---

### Priority 1

Immediate Decision Support

Examples:

- Critical Risks
- Escalations
- High Priority Decisions
- Outcome Status

---

### Priority 2

Decision Evaluation

Examples:

- Readiness Indicators
- Capacity Indicators
- Performance Status
- Priority Signals

---

### Priority 3

Explanation

Examples:

- Trends
- Comparisons
- Supporting Analysis

---

### Priority 4

Investigation

Examples:

- Detailed Breakdowns
- Supporting Metrics
- Historical Context

---

## Outcome Visibility Design

### Purpose

Keep Business Outcomes visible throughout the reporting experience.

---

### Discovery Questions

Ask:

- What outcome is affected?
- How is success measured?
- How is current performance progressing?

---

### Visibility Guidelines

Business Outcomes should not be hidden.

Users should always understand:

- What outcome matters
- How performance is progressing
- Why decisions matter

---

## Escalation Visibility Design

### Purpose

Ensure critical conditions are visible immediately.

---

### Priority Placement

Escalations should appear before:

- Detailed Analysis
- Historical Reporting
- Supporting Metrics

---

### Typical Escalation Content

- Critical Risks
- Capacity Failures
- Governance Issues
- Data Trust Failures
- Intervention Requirements

---

## Human Authority Visibility Design

### Purpose

Make accountability visible.

---

### Visibility Guidelines

Where applicable display:

- Decision Owner
- Action Owner
- Outcome Owner
- Escalation Authority

---

### Discovery Questions

Ask:

- Who is responsible?
- Who approves action?
- Who handles escalation?
- Who owns outcomes?

---

## Trust Visibility Design

### Purpose

Communicate confidence before action.

---

### Include When Relevant

- Data Freshness
- Data Quality
- Governance Status
- Validation Status

---

### Discovery Questions

Ask:

- Can users trust the information?
- Could quality concerns affect decisions?

---

## Failure Mode Visibility Design

### Purpose

Ensure business risks remain visible.

---

### Failure Conditions To Highlight

- Escalations
- Exceptions
- Capacity Risks
- Governance Risks
- Trust Risks
- Outcome Risks

---

### Guideline

Critical risks should never require extensive navigation to locate.

---

## Story-To-Layout Alignment Review

Verify:

Story 0
↓
Story 1
↓
Story 2
↓
Story 3
↓
Story 4
↓
Story 5
↓
Story 6
↓
Story 7

maps naturally to the intended layout flow.

---

## Handoff Readiness Design

Layout blueprints should provide sufficient detail for:

- Mockup Agents
- UX Designers
- TRD Authors
- Semantic Designers
- Report Developers

without requiring rediscovery.

---

## Layout Quality Standards

Good Layouts are:

- Outcome Focused
- Decision Oriented
- Action Focused
- Easy To Navigate
- Explainable
- Consistent

---

Poor Layouts are:

- Visual First
- Dashboard First
- Randomly Organized
- Analysis Before Decisions
- Action Hidden

---

## Layout Readiness Checklist

Verify:

□ Story Structure Applied

□ Reading Order Defined

□ Information Hierarchy Defined

□ Outcome Visibility Confirmed

□ Escalation Visibility Confirmed

□ Human Authority Visible

□ Trust Visibility Considered

□ Failure Visibility Considered

□ Handoff Ready

---

## Validation Rule

If users must:

- Search For Critical Conditions
- Reconstruct The Decision Process
- Determine Their Own Navigation Path

the layout requires redesign.

---

## Layout Blueprint Success Statement

Layout Design succeeds when:

Business Outcomes

drive Decisions

Decisions

drive Stories

Stories

drive Layout

and users naturally progress through:

Understanding
↓
Assessment
↓
Decision
↓
Action

without confusion, unnecessary navigation, or loss of accountability.

---

# SECTION 16 — VISUAL RECOMMENDATION GUIDELINES

## Purpose

Visual Recommendations define how approved decision-support information should be presented.

Visuals exist to support:

- Business Outcomes
- Decisions
- Questions
- Signals
- Actions

Visuals are the final expression of approved business design.

Visuals should never become the starting point for report design.

---

## Governing Rule

Visual selection must always follow:

Business Outcome
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

Never begin with:

Visual
↓
Dashboard
↓
Decision

Visuals are downstream artifacts.

---

## Visual Recommendation Process

### Step 01

Review Business Outcomes

---

### Step 02

Review Decisions

---

### Step 03

Review Questions

---

### Step 04

Review Signals

---

### Step 05

Review Actions

---

### Step 06

Review Story Requirements

---

### Step 07

Recommend Visuals

---

### Step 08

Validate Decision Support

---

## Visual Selection Framework

Apply:

Business Outcome
↓
Decision
↓
Question
↓
Signal
↓
Action
↓
Visual

Visuals should exist only when they improve decision quality.

---

## Visual Purpose Discovery

### Purpose

Determine why a visual is required.

---

### Discovery Questions

Ask:

- What decision becomes easier?
- What action becomes clearer?
- What condition becomes more visible?
- What outcome becomes easier to improve?

---

### Validation

Every visual should improve one or more of:

- Awareness
- Prioritization
- Comparison
- Explanation
- Action

---

## Awareness Visuals

### Purpose

Provide immediate understanding.

---

### Recommended Visuals

- KPI Cards
- Status Cards
- Scorecards
- Summary Panels

---

### Best For

- Executive Context
- Outcome Monitoring
- Decision Readiness

---

## Prioritization Visuals

### Purpose

Help users determine what should happen first.

---

### Recommended Visuals

- Priority Tables
- Ranked Lists
- Exception Boards
- Escalation Queues

---

### Best For

- Action Required
- Decision Prioritization
- Operational Briefing

---

## Comparison Visuals

### Purpose

Compare alternatives and options.

---

### Recommended Visuals

- Bar Charts
- Matrix Views
- Comparison Tables
- Benchmark Tables

---

### Best For

- Regional Monitoring
- Capacity Reviews
- Performance Reviews

---

## Explanation Visuals

### Purpose

Show causes and contributing factors.

---

### Recommended Visuals

- Trend Charts
- Breakdown Charts
- Driver Analysis
- Distribution Views

---

### Best For

- Analysis And Explanation
- Root Cause Reviews
- Performance Analysis

---

## Action Visuals

### Purpose

Convert findings into next steps.

---

### Recommended Visuals

- Recommendation Cards
- Operational Queues
- Action Tables
- Escalation Panels

---

### Best For

- Operational Briefing
- Action Required
- Escalation Management

---

## Visual Qualification Test

For every visual ask:

```text
What business action becomes easier because of this visual?
```

If no answer exists:

```text
Do Not Recommend The Visual
```

---

## Visual Recommendation Discovery

### Discovery Questions

Ask:

- What decision does this visual support?
- What question does this visual answer?
- What signal is being communicated?
- What action becomes easier?

---

## Outcome Alignment Review

Every visual should support:

Business Outcome
↓
Decision
↓
Action
↓
Visual

---

### Validation Questions

Ask:

- Which outcome improves?
- Which decision benefits?
- Which action becomes easier?

---

## Human Authority Support

Visuals should reinforce accountability.

Where appropriate provide visibility into:

- Decision Owners
- Action Owners
- Escalation Owners
- Outcome Owners

---

### Discovery Questions

Ask:

- Who uses this visual?
- Who acts because of this visual?
- Who owns the outcome?

---

## Trust Visibility Guidelines

Where decision confidence matters, visually communicate:

- Data Freshness
- Data Quality
- Completeness
- Validation Status
- Governance Status

---

### Validation Questions

Ask:

- Can users trust the information?
- Can trust concerns be identified?

---

## Failure Visibility Guidelines

Visuals should make critical conditions obvious.

---

### Examples

- Escalations
- Capacity Failures
- Governance Issues
- Data Quality Risks
- Outcome Risks

---

### Discovery Questions

Ask:

- What should never be missed?
- What condition requires immediate visibility?
- What condition requires intervention?

---

## Visual Consistency Guidelines

Use consistent:

- Labels
- Terminology
- Status Definitions
- Color Definitions

across all visual recommendations.

Consistency improves trust.

---

## Visual Anti-Patterns

Avoid visuals because:

- They Look Good
- They Are Popular
- They Were Used Previously
- The Tool Makes Them Easy

---

Avoid:

- Decorative Visuals
- Vanity Metrics
- Unused KPIs
- Visuals Without Actions
- Visuals Without Decisions

---

## Visual Traceability Review

Verify:

Business Outcome
↓
Decision
↓
Question
↓
Signal
↓
Action
↓
Visual

remains intact.

---

## Visual Readiness Checklist

Verify:

□ Business Outcome Supported

□ Decision Supported

□ Question Supported

□ Signal Supported

□ Action Supported

□ Human Authority Considered

□ Trust Visibility Considered

□ Failure Visibility Considered

□ Traceability Preserved

---

## Validation Rule

If a visual cannot answer:

```text
Why am I seeing this?

What action becomes easier?

What decision does this support?
```

the recommendation should be removed.

---

## Visual Recommendation Success Statement

Visual Recommendation succeeds when:

Business Outcomes

drive Decisions

Decisions

drive Questions

Questions

drive Signals

Signals

drive Actions

Actions

drive Visuals

and stakeholders can clearly explain:

- Why the visual exists
- What decision it supports
- What action it enables
- What outcome it improves

before implementation begins.

---

# SECTION 17 — TRACEABILITY GUIDELINES

## Purpose

Traceability preserves the relationship between business intent and report design.

The objective is to ensure every artifact can be explained, justified, reviewed, and governed.

Traceability prevents:

- Orphan Decisions
- Orphan Questions
- Orphan Signals
- Orphan Thresholds
- Orphan Actions
- Orphan Stories
- Orphan Visuals

Everything should exist for a documented business reason.

---

## Governing Rule

Every artifact must support:

Business Problem
↓
Business Capability
↓
Business Outcome
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

No break in the chain is permitted.

---

## Traceability Review Process

### Step 01

Validate Business Problem Alignment

---

### Step 02

Validate Business Capability Alignment

---

### Step 03

Validate Business Outcome Alignment

---

### Step 04

Validate Decision Alignment

---

### Step 05

Validate Question Alignment

---

### Step 06

Validate Signal Alignment

---

### Step 07

Validate Threshold Alignment

---

### Step 08

Validate Action Alignment

---

### Step 09

Validate Story Alignment

---

### Step 10

Validate Visual Alignment

---

## Business Problem Traceability

### Purpose

Ensure the report solves a defined business problem.

---

### Validation Questions

Ask:

- What problem does this report address?
- Why does the problem matter?
- What business impact exists?

---

### Traceability Chain

Business Problem
↓
Business Capability

---

## Business Capability Traceability

### Purpose

Ensure supported capabilities are explicitly identified.

---

### Validation Questions

Ask:

- What capability is improved?
- What business function benefits?
- Why is this capability important?

---

### Traceability Chain

Business Capability
↓
Business Outcome

---

## Business Outcome Traceability

### Purpose

Ensure measurable outcomes justify report design.

---

### Validation Questions

Ask:

- What business outcome improves?
- How is success measured?
- Who owns success?

---

### Traceability Chain

Business Outcome
↓
Decision

---

## Decision Traceability

### Purpose

Ensure every decision exists for a business reason.

---

### Validation Questions

Ask:

- Which outcome requires this decision?
- Who owns the decision?
- What action depends on it?

---

### Traceability Chain

Business Outcome
↓
Decision

---

## Question Traceability

### Purpose

Ensure every question supports decision making.

---

### Validation Questions

Ask:

- Which decision does this question support?
- What happens if this question is removed?
- Does the question improve decision quality?

---

### Traceability Chain

Decision
↓
Question

---

## Signal Traceability

### Purpose

Ensure every signal provides decision support.

---

### Validation Questions

Ask:

- Which question does this signal answer?
- Which decision depends on the signal?
- Which action becomes easier because of the signal?

---

### Traceability Chain

Question
↓
Signal

---

## Threshold Traceability

### Purpose

Ensure thresholds provide meaningful interpretation.

---

### Validation Questions

Ask:

- Why does this threshold exist?
- What action does it trigger?
- What business meaning does it provide?

---

### Traceability Chain

Signal
↓
Threshold

---

## Action Traceability

### Purpose

Ensure actions improve outcomes.

---

### Validation Questions

Ask:

- What outcome improves?
- What decision created the action?
- Who performs the action?

---

### Traceability Chain

Threshold
↓
Action

---

## Story Traceability

### Purpose

Ensure stories communicate decision logic.

---

### Validation Questions

Ask:

- Which decision is being communicated?
- Which action becomes clearer?
- Which outcome is being improved?

---

### Traceability Chain

Action
↓
Story

---

## Visual Traceability

### Purpose

Ensure visuals support decisions.

---

### Validation Questions

Ask:

- Why does this visual exist?
- What decision does it support?
- What action becomes easier?

---

### Traceability Chain

Story
↓
Visual

---

## Human Authority Traceability

### Purpose

Preserve accountability throughout the decision chain.

---

### Verify

Every critical design element identifies:

- Decision Owner
- Outcome Owner
- Action Owner
- Approval Authority
- Escalation Authority

---

### Validation Questions

Ask:

- Who owns this decision?
- Who owns this outcome?
- Who approves actions?
- Who receives escalations?

---

## Handoff Traceability

### Purpose

Ensure downstream artifacts inherit business intent.

---

### Verify

Mockup
↓
Story

TRD
↓
Decision Logic

Semantic Model
↓
Signals

Report Build
↓
Stories

---

### Validation Questions

Ask:

- Can downstream teams understand intent?
- Can traceability be preserved?
- Can work continue without revisiting discovery?

---

## Regression Protection Traceability

### Purpose

Prevent accidental loss of approved business design.

---

### Review

When previous artifacts exist compare:

- Decisions
- Questions
- Signals
- Thresholds
- Actions
- Stories
- Outcomes

---

### Validation Questions

Ask:

- What existing logic is being changed?
- What justification exists?
- What business impact could occur?

---

## Traceability Quality Standards

Good Traceability Is:

- Complete
- Explainable
- Auditable
- Outcome Aligned
- Governed

---

Poor Traceability Is:

- Assumed
- Incomplete
- Broken
- Unverifiable
- Ambiguous

---

## Traceability Readiness Checklist

Verify:

□ Business Problem Traceable

□ Business Capability Traceable

□ Business Outcome Traceable

□ Decision Traceable

□ Question Traceable

□ Signal Traceable

□ Threshold Traceable

□ Action Traceable

□ Story Traceable

□ Visual Traceable

□ Human Authority Traceable

□ Handoff Traceability Preserved

□ Regression Risks Reviewed

---

## Validation Rule

If any artifact cannot be traced back to:

Business Outcome

or

Decision

the artifact should be reviewed and potentially removed.

---

## Traceability Success Statement

Traceability succeeds when:

Business Problems

support Capabilities

Capabilities

support Outcomes

Outcomes

support Decisions

Decisions

support Questions

Questions

support Signals

Signals

support Thresholds

Thresholds

support Actions

Actions

support Stories

Stories

support Visuals

and every stakeholder can explain:

- Why the artifact exists
- Which outcome it supports
- Which decision it supports
- Which action it enables

without ambiguity.

---

# SECTION 18 — COVERAGE DISCOVERY GUIDELINES

## Purpose

Coverage Discovery ensures the Decision Story fully addresses the business problem.

The objective is to prevent blind spots, incomplete designs, and unsupported decisions.

Coverage analysis confirms that:

- Outcomes are covered
- Decisions are covered
- Actions are covered
- Risks are covered
- Authority is covered
- Stories are covered

before outputs are approved.

---

## Governing Rule

Every significant business requirement should be represented somewhere within the Decision Story.

Coverage should be evaluated across:

Business Problem
↓
Business Capability
↓
Business Outcome
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

No major business concern should remain uncovered.

---

## Coverage Discovery Process

### Step 01

Review Foundation Coverage

---

### Step 02

Review Outcome Coverage

---

### Step 03

Review Decision Coverage

---

### Step 04

Review Question Coverage

---

### Step 05

Review Signal Coverage

---

### Step 06

Review Action Coverage

---

### Step 07

Review Story Coverage

---

### Step 08

Review Governance Coverage

---

### Step 09

Review Handoff Coverage

---

## Foundation Coverage Review

### Purpose

Confirm that business context is fully represented.

---

### Verify Coverage For

- Business Problem
- Business Capability
- Business Outcomes
- Strategic Alignment
- Risks
- Constraints
- Assumptions

---

### Discovery Questions

Ask:

- Is the business problem represented?
- Is the capability represented?
- Are outcomes represented?
- Are risks represented?

---

## Business Outcome Coverage Review

### Purpose

Ensure outcomes remain visible throughout the design.

---

### Verify Coverage For

- Primary Outcomes
- Secondary Outcomes
- Strategic Outcomes
- Operational Outcomes

---

### Discovery Questions

Ask:

- Does every outcome appear in the design?
- Does every outcome have decision support?
- Does every outcome have measurable success criteria?

---

## Decision Coverage Review

### Purpose

Ensure all important decisions are represented.

---

### Verify Coverage For

- Primary Decisions
- Secondary Decisions
- Escalation Decisions
- Governance Decisions
- Prioritization Decisions

---

### Discovery Questions

Ask:

- Does every important decision appear?
- Are supporting decisions represented?
- Are escalation decisions represented?

---

## Question Coverage Review

### Purpose

Ensure information requirements are complete.

---

### Verify Coverage Across

- Operational
- Capacity
- Risk
- Governance
- Trust
- Regional
- Executive

---

### Discovery Questions

Ask:

- Can every decision be answered?
- Are major information gaps present?
- Are important questions missing?

---

## Signal Coverage Review

### Purpose

Ensure sufficient evidence exists for decisions.

---

### Verify Coverage Across

- Critical Signals
- Decision Signals
- Trust Signals
- Risk Signals
- Outcome Signals

---

### Discovery Questions

Ask:

- Does every question have supporting signals?
- Are critical signals identified?
- Are trust indicators included?

---

## Action Coverage Review

### Purpose

Ensure business responses exist.

---

### Verify Coverage Across

- Monitoring Actions
- Operational Actions
- Escalation Actions
- Intervention Actions
- Governance Actions

---

### Discovery Questions

Ask:

- Does every threshold lead to action?
- Are escalation actions defined?
- Are ownership responsibilities assigned?

---

## Human Authority Coverage Review

### Purpose

Ensure accountability is visible.

---

### Verify Coverage For

- Decision Owners
- Outcome Owners
- Action Owners
- Approval Authorities
- Escalation Authorities

---

### Discovery Questions

Ask:

- Is accountability visible?
- Is authority defined?
- Are approval responsibilities documented?

---

## Failure Mode Coverage Review

### Purpose

Ensure critical risks are represented.

---

### Verify Coverage For

- Decision Risks
- Signal Risks
- Data Trust Risks
- Operational Risks
- Outcome Risks

---

### Discovery Questions

Ask:

- What could fail?
- Where are major risks represented?
- Are mitigation approaches described?

---

## Story Coverage Review

### Purpose

Ensure the complete decision journey is represented.

---

### Verify Coverage For

Story 0

Executive Context

---

Story 1

Action Required

---

Story 2

Decision Readiness

---

Story 3

Decision Prioritization

---

Story 4

Analysis And Explanation

---

Story 5

Data Trust

---

Story 6

Regional Monitoring

---

Story 7

Operational Briefing

---

### Discovery Questions

Ask:

- Are all required stories represented?
- Are story objectives clear?
- Are stories aligned to outcomes?

---

## Governance Coverage Review

### Purpose

Ensure governance requirements are represented.

---

### Verify Coverage For

- Ownership
- Accountability
- Approvals
- Escalations
- Traceability

---

### Discovery Questions

Ask:

- Is governance visible?
- Are approvals identified?
- Are accountability paths documented?

---

## Handoff Coverage Review

### Purpose

Ensure downstream teams can proceed without rediscovery.

---

### Verify Coverage For

- Mockup Readiness
- TRD Readiness
- Semantic Readiness
- Build Readiness

---

### Discovery Questions

Ask:

- Can mockups be produced?
- Can semantic design begin?
- Can developers proceed?

---

## Regression Protection Coverage Review

### Purpose

Ensure proven business knowledge is preserved.

---

### Review Existing

- Decisions
- Questions
- Signals
- Thresholds
- Actions
- Stories
- Business Rules

---

### Discovery Questions

Ask:

- What previously approved logic exists?
- What is changing?
- What business impact may occur?

---

## Coverage Quality Standards

Good Coverage Is:

- Complete
- Balanced
- Outcome Aligned
- Decision Focused
- Governed
- Traceable

---

Poor Coverage Includes:

- Missing Decisions
- Missing Actions
- Missing Risks
- Missing Ownership
- Missing Outcomes
- Missing Trust Validation

---

## Coverage Readiness Checklist

Verify:

□ Foundation Coverage Complete

□ Outcome Coverage Complete

□ Decision Coverage Complete

□ Question Coverage Complete

□ Signal Coverage Complete

□ Action Coverage Complete

□ Human Authority Coverage Complete

□ Failure Mode Coverage Complete

□ Story Coverage Complete

□ Governance Coverage Complete

□ Handoff Coverage Complete

□ Regression Review Complete

---

## Validation Rule

If a critical business area is relevant but not represented:

Create a Coverage Finding

and evaluate whether design expansion is required.

---

## Coverage Discovery Success Statement

Coverage Discovery succeeds when:

Business Problems

are fully represented

Business Outcomes

are fully supported

Decisions

are fully answerable

Actions

are fully defined

and no major business concern remains unaddressed within the Decision Story design.

---

# SECTION 19 — FAILURE MODE DISCOVERY GUIDELINES

## Purpose

Failure Mode Discovery identifies conditions that may prevent the reporting solution from achieving its intended outcomes.

The objective is not to eliminate all risk.

The objective is to understand:

- What could fail
- Why failure could occur
- What impact failure may create
- What mitigation actions may be required

Failure Mode Discovery should occur before final validation.

---

## Governing Rule

Every critical outcome, decision, signal, and action should be evaluated for potential failure conditions.

Failure analysis should focus on:

Business Outcomes
↓
Decisions
↓
Signals
↓
Actions

and not solely on technical implementation.

---

## Failure Discovery Process

### Step 01

Review Business Outcomes

---

### Step 02

Review Critical Decisions

---

### Step 03

Review Critical Signals

---

### Step 04

Review Critical Thresholds

---

### Step 05

Review Critical Actions

---

### Step 06

Identify Failure Scenarios

---

### Step 07

Assess Business Impact

---

### Step 08

Identify Mitigation Approaches

---

## Failure Mode Categories

Evaluate failures across the following areas:

### Business Outcome Failures

### Decision Failures

### Signal Failures

### Threshold Failures

### Operational Failures

### Trust Failures

### Governance Failures

### Adoption Failures

---

## Business Outcome Failure Discovery

### Purpose

Identify conditions where intended business outcomes are not achieved.

---

### Discovery Questions

Ask:

- What could prevent success?
- What outcome could fail to improve?
- What dependencies could block progress?
- What assumptions could be incorrect?

---

### Examples

- Placement Times Do Not Improve
- Utilization Remains Unchanged
- Escalation Volume Increases
- User Adoption Remains Low

---

## Decision Failure Discovery

### Purpose

Identify conditions where poor decisions may occur.

---

### Discovery Questions

Ask:

- What could cause incorrect decisions?
- What information could be misunderstood?
- What important decision may be unsupported?
- What decision could be delayed?

---

### Examples

- Capacity Assigned Incorrectly
- Resources Allocated Improperly
- Escalations Missed
- Priorities Misidentified

---

## Signal Failure Discovery

### Purpose

Identify risks affecting signal quality.

---

### Discovery Questions

Ask:

- Could the signal be unavailable?
- Could the signal be inaccurate?
- Could the signal become outdated?
- Could the signal be misunderstood?

---

### Examples

- Missing Data
- Calculation Errors
- Stale Refreshes
- Conflicting Definitions

---

## Threshold Failure Discovery

### Purpose

Identify risks affecting business interpretation.

---

### Discovery Questions

Ask:

- Could thresholds trigger unnecessary action?
- Could thresholds miss critical conditions?
- Could business rules change?
- Could thresholds be interpreted inconsistently?

---

### Examples

- False Positive Alerts
- False Negative Alerts
- Misaligned Threshold Values
- Obsolete Business Rules

---

## Operational Failure Discovery

### Purpose

Identify failures in execution and response.

---

### Discovery Questions

Ask:

- Could actions be ignored?
- Could action ownership be unclear?
- Could escalation paths fail?
- Could response times be too slow?

---

### Examples

- No Owner Assigned
- Escalation Not Performed
- Delayed Response
- Incomplete Follow-Up

---

## Trust Failure Discovery

### Purpose

Identify conditions that reduce confidence in reporting.

---

### Discovery Questions

Ask:

- Could users lose confidence?
- Could data quality concerns appear?
- Could conflicting numbers exist?
- Could governance concerns arise?

---

### Examples

- Data Freshness Issues
- Data Quality Failures
- Inconsistent Definitions
- Missing Validation

---

## Governance Failure Discovery

### Purpose

Identify accountability and oversight risks.

---

### Discovery Questions

Ask:

- Is authority unclear?
- Are approvals undefined?
- Are accountabilities shared?
- Could governance processes fail?

---

### Examples

- Missing Decision Owner
- Missing Approval Authority
- Undefined Escalation Paths
- Governance Gaps

---

## Adoption Failure Discovery

### Purpose

Identify conditions that reduce solution usage.

---

### Discovery Questions

Ask:

- Could users avoid the report?
- Could the report be too complex?
- Could trust be insufficient?
- Could users prefer existing processes?

---

### Examples

- Low Adoption
- Workflow Bypass
- Shadow Reporting
- Excessive Complexity

---

## Failure Impact Assessment

Classify each failure mode.

### Critical

Failure significantly affects outcomes.

Immediate mitigation required.

---

### High

Failure impacts decisions or operations.

Mitigation strongly recommended.

---

### Medium

Failure creates inefficiency or confusion.

Mitigation beneficial.

---

### Low

Limited business impact.

Monitor and review.

---

## Mitigation Discovery

For each significant failure identify:

### Prevention

What reduces likelihood?

---

### Detection

How is failure identified?

---

### Response

What action occurs when detected?

---

### Recovery

How is business operation restored?

---

## Failure Mode Prioritization

Prioritize failures based on:

- Business Impact
- Decision Impact
- Outcome Impact
- User Impact
- Governance Impact

Highest-risk failures should receive the greatest visibility.

---

## Human Authority Review

For every critical failure identify:

- Decision Owner
- Outcome Owner
- Escalation Authority
- Response Owner

Accountability should remain explicit.

---

## Failure Coverage Checklist

Verify:

□ Outcome Failure Risks Reviewed

□ Decision Failure Risks Reviewed

□ Signal Failure Risks Reviewed

□ Threshold Failure Risks Reviewed

□ Operational Failure Risks Reviewed

□ Trust Failure Risks Reviewed

□ Governance Failure Risks Reviewed

□ Adoption Risks Reviewed

□ Mitigations Identified

---

## Validation Rule

If a critical outcome depends on:

- A Critical Decision
- A Critical Signal
- A Critical Action

and no failure analysis exists,

create a Failure Review Finding.

---

## Failure Mode Discovery Success Statement

Failure Mode Discovery succeeds when:

Business Outcomes

are protected by Decisions

Decisions

are protected by Signals

Signals

are protected by Validation

Actions

are protected by Ownership

and stakeholders can clearly explain:

- What could fail?
- Why it could fail?
- What impact could occur?
- How failure would be detected?
- How failure would be managed?

before final approval.

---

# SECTION 20 — AI READINESS GUIDELINES

## Purpose

AI Readiness ensures Decision Story artifacts can be understood, explained, validated, and reused by humans and future AI agents.

The objective is to create business design artifacts that are:

- Explainable
- Traceable
- Governed
- Reusable
- Transferable

without requiring additional discovery.

AI readiness improves long-term maintainability and framework scalability.

---

## Governing Rule

Every documented artifact should explain:

- Why It Exists
- What It Supports
- What Outcome It Improves
- What Decision It Enables
- What Action It Influences

Artifacts that cannot be explained are not AI Ready.

---

## AI Readiness Process

### Step 01

Review Business Outcomes

---

### Step 02

Review Decision Traceability

---

### Step 03

Review Human Authority

---

### Step 04

Review Story Explainability

---

### Step 05

Review Handoff Readiness

---

### Step 06

Review Documentation Completeness

---

### Step 07

Validate AI Readiness

---

## Outcome Explainability

### Purpose

Ensure business outcomes can be understood without reviewing source materials.

---

### Every Outcome Should Explain

- Why the outcome matters
- How success is measured
- Who owns success
- Which decisions influence success

---

### Validation Questions

Ask:

- Can a new stakeholder understand the outcome?
- Can an AI explain the outcome?
- Can the outcome be traced to decisions?

---

## Decision Explainability

### Purpose

Ensure every decision can be explained independently.

---

### Every Decision Should Explain

- Why the decision exists
- What outcome it supports
- Who owns it
- What action depends on it

---

### Validation Questions

Ask:

- Can the decision be explained without the BRD?
- Can the decision be justified?
- Can the decision be traced?

---

## Question Explainability

### Purpose

Ensure information requirements are self-explanatory.

---

### Every Question Should Explain

- What information is required
- Why it matters
- Which decision it supports
- Which outcome it influences

---

### Validation Questions

Ask:

- Can users understand the question immediately?
- Can an AI explain why the question exists?

---

## Signal Explainability

### Purpose

Ensure metrics and indicators remain understandable.

---

### Every Signal Should Explain

- What is being measured
- Why it is measured
- Which question it answers
- Which decision depends on it

---

### Validation Questions

Ask:

- Can business users interpret the signal?
- Can AI explain signal purpose?

---

## Action Explainability

### Purpose

Ensure recommended actions remain understandable.

---

### Every Action Should Explain

- What should happen
- Who should act
- Why the action matters
- What outcome improves

---

### Validation Questions

Ask:

- Can execution ownership be identified?
- Can AI explain the business rationale?

---

## Human Authority Explainability

### Purpose

Preserve accountability.

---

### Every Critical Element Should Identify

- Decision Owner
- Outcome Owner
- Action Owner
- Approval Authority
- Escalation Authority

---

### Validation Questions

Ask:

- Who owns the decision?
- Who owns the outcome?
- Who approves actions?
- Who manages escalations?

---

## Traceability Explainability

### Purpose

Ensure business logic remains discoverable.

---

### Every Artifact Should Trace To

Business Problem
↓
Business Capability
↓
Business Outcome
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

---

### Validation Questions

Ask:

- Can the chain be followed end-to-end?
- Can business intent be reconstructed?

---

## Handoff Readiness For AI

### Purpose

Support future agents and automation workflows.

---

### Artifacts Should Enable

- Mockup Generation
- TRD Generation
- Semantic Design
- Report Development
- Governance Review

without revisiting discovery.

---

### Validation Questions

Ask:

- Can another agent continue work?
- Can another analyst continue work?
- Can another team understand intent?

---

## Documentation Completeness Standard

Every major artifact should explain:

### Why

Why does it exist?

---

### What

What does it do?

---

### Who

Who owns it?

---

### Outcome

What outcome improves?

---

### Decision

What decision does it support?

---

## AI Interoperability Standard

Decision Story artifacts should be reusable across:

- Future Agents
- Future Framework Versions
- Future Teams
- Future Projects

without requiring redesign.

---

## AI Readiness Quality Standards

AI Ready Artifacts are:

- Explainable
- Traceable
- Governed
- Consistent
- Self-Contained
- Transferable

---

Not AI Ready:

- Assumed Knowledge
- Missing Ownership
- Missing Purpose
- Missing Traceability
- Ambiguous Business Logic

---

## AI Readiness Checklist

Verify:

□ Outcomes Explainable

□ Decisions Explainable

□ Questions Explainable

□ Signals Explainable

□ Actions Explainable

□ Ownership Documented

□ Traceability Preserved

□ Handoff Ready

□ Governance Visible

---

## Validation Rule

If an artifact cannot answer:

```text
Why do I exist?

What outcome do I support?

What decision do I support?

Who owns me?
```

the artifact is not AI Ready.

---

## AI Readiness Success Statement

AI Readiness succeeds when:

Business Problems

drive Capabilities

Capabilities

drive Outcomes

Outcomes

drive Decisions

Decisions

drive Actions

and future humans, teams, and AI agents can understand, explain, govern, and extend the design without revisiting discovery activities.

The result is:

- Explainable Design
- Reusable Design
- Governed Design
- Transferable Design
- AI-Ready Design

---

# SECTION 21 — VALIDATION GUIDELINES

## Purpose

Validation ensures the completed Decision Story design is:

- Complete
- Governed
- Traceable
- Outcome Aligned
- Action Oriented
- Human Governed
- Promotion Ready

Validation is the final discovery activity before handoff.

---

## Governing Rule

No Decision Story artifact should be approved until validation is complete.

Validation must confirm:

Business Problem
↓
Business Capability
↓
Business Outcome
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

remains intact.

---

## Validation Process

### Step 01

Validate Foundation

---

### Step 02

Validate Outcomes

---

### Step 03

Validate Decisions

---

### Step 04

Validate Questions

---

### Step 05

Validate Signals

---

### Step 06

Validate Thresholds

---

### Step 07

Validate Actions

---

### Step 08

Validate Stories

---

### Step 09

Validate Traceability

---

### Step 10

Validate Readiness

---

## Foundation Validation

### Purpose

Confirm business context is complete.

---

### Verify

□ Business Problem Defined

□ Business Capability Defined

□ Business Outcomes Defined

□ Strategic Alignment Defined

□ Risks Identified

□ Constraints Identified

□ Assumptions Identified

---

### Validation Questions

Ask:

- Why does this report exist?
- What capability is supported?
- What outcome should improve?

---

## Outcome Validation

### Purpose

Confirm business value exists.

---

### Verify

□ Primary Outcomes Defined

□ Outcome Owners Defined

□ Outcome Measures Defined

□ Success Targets Defined

□ Outcome Alignment Verified

---

### Validation Questions

Ask:

- What improves?
- How is success measured?
- Who owns success?

---

## Decision Validation

### Purpose

Confirm decision support is properly defined.

---

### Verify

□ Primary Decision Defined

□ Secondary Decisions Defined

□ Decision Owner Defined

□ Decision Authority Defined

□ Decision Frequency Defined

□ Success Criteria Defined

---

### Validation Questions

Ask:

- What decision is supported?
- Why does it matter?
- Who owns it?

---

## Question Validation

### Purpose

Confirm information requirements are complete.

---

### Verify

□ Questions Defined

□ Questions Support Decisions

□ Questions Support Outcomes

□ Questions Are Actionable

□ No Orphan Questions

---

### Validation Questions

Ask:

- What decision depends on this question?
- What outcome improves because of this question?

---

## Signal Validation

### Purpose

Confirm evidence supports decision making.

---

### Verify

□ Signals Defined

□ Signals Measurable

□ Signals Explainable

□ Signals Trusted

□ No Orphan Signals

---

### Validation Questions

Ask:

- What question does the signal answer?
- What decision depends on it?

---

## Threshold Validation

### Purpose

Confirm signals are actionable.

---

### Verify

□ Thresholds Defined

□ Status Logic Defined

□ Action Triggers Defined

□ Escalation Logic Defined

□ Business Meaning Defined

---

### Validation Questions

Ask:

- What happened?
- Why does it matter?
- What should happen next?

---

## Action Validation

### Purpose

Confirm actions improve outcomes.

---

### Verify

□ Actions Defined

□ Action Owners Defined

□ Outcome Alignment Confirmed

□ Escalation Owners Defined

□ Accountability Defined

---

### Validation Questions

Ask:

- What should happen?
- Who should act?
- What outcome improves?

---

## Story Validation

### Purpose

Confirm complete decision support exists.

---

### Verify

□ Story 0 Defined

□ Story 1 Defined

□ Story 2 Defined

□ Story 3 Defined

□ Story 4 Defined

□ Story 5 Defined

□ Story 6 Defined

□ Story 7 Defined

---

### Validation Questions

Ask:

- What is happening?
- Why is it happening?
- What requires attention?
- What decision is required?
- What action should occur?

---

## Human Authority Validation

### Purpose

Confirm accountability remains visible.

---

### Verify

□ Decision Owner Defined

□ Outcome Owner Defined

□ Action Owner Defined

□ Approval Authority Defined

□ Escalation Authority Defined

---

### Validation Questions

Ask:

- Who decides?
- Who approves?
- Who acts?
- Who owns the outcome?

---

## Failure Mode Validation

### Purpose

Confirm key risks have been reviewed.

---

### Verify

□ Outcome Risks Reviewed

□ Decision Risks Reviewed

□ Signal Risks Reviewed

□ Trust Risks Reviewed

□ Operational Risks Reviewed

□ Mitigation Approaches Identified

---

### Validation Questions

Ask:

- What could fail?
- What impact could occur?
- How would failure be detected?

---

## Traceability Validation

### Purpose

Confirm business logic remains explainable.

---

### Verify

□ Business Problem Traceable

□ Business Capability Traceable

□ Business Outcome Traceable

□ Decision Traceable

□ Question Traceable

□ Signal Traceable

□ Threshold Traceable

□ Action Traceable

□ Story Traceable

□ Visual Traceable

---

### Validation Questions

Ask:

- Can the chain be followed end-to-end?
- Can every artifact be justified?

---

## Handoff Readiness Validation

### Purpose

Confirm downstream teams can proceed.

---

### Verify

□ Mockup Ready

□ TRD Ready

□ Semantic Ready

□ Build Ready

□ Governance Ready

---

### Validation Questions

Ask:

- Can another team continue work?
- Can another agent continue work?
- Is rediscovery required?

---

## Regression Protection Validation

### Purpose

Protect approved business knowledge.

---

### Verify

□ Existing Decisions Reviewed

□ Existing Questions Reviewed

□ Existing Signals Reviewed

□ Existing Thresholds Reviewed

□ Existing Actions Reviewed

□ Existing Stories Reviewed

□ Existing Logic Preserved

---

### Validation Questions

Ask:

- What changed?
- Why did it change?
- What business impact exists?

---

## Promotion Readiness Assessment

### Not Ready

Characteristics:

```text
Critical Gaps

Missing Outcomes

Missing Decisions

Missing Ownership
```

Action:

```text
Return To Discovery
```

---

### Partially Ready

Characteristics:

```text
Minor Gaps

Limited Risks

Additional Validation Required
```

Action:

```text
Remediate Before Approval
```

---

### Ready

Characteristics:

```text
Traceability Complete

Governance Complete

Outcome Alignment Complete

Handoff Ready
```

Action:

```text
Proceed To Handoff
```

---

## Validation Quality Standards

Good Validation Is:

- Objective
- Repeatable
- Traceable
- Governed
- Outcome Focused

---

Poor Validation Is:

- Assumption Based
- Incomplete
- Unstructured
- Unverifiable

---

## Validation Readiness Checklist

Verify:

□ Foundation Complete

□ Outcomes Complete

□ Decisions Complete

□ Questions Complete

□ Signals Complete

□ Thresholds Complete

□ Actions Complete

□ Stories Complete

□ Human Authority Complete

□ Failure Review Complete

□ Traceability Complete

□ Handoff Ready

□ Regression Review Complete

---

## Validation Rule

If any critical area fails validation:

Create A Validation Finding

and return to the appropriate discovery activity.

Do not proceed to handoff.

---

## Validation Success Statement

Validation succeeds when:

Business Problems

support Capabilities

Capabilities

support Outcomes

Outcomes

support Decisions

Decisions

support Actions

and every artifact is:

- Complete
- Explainable
- Traceable
- Governed
- Accountable
- Promotion Ready

before handoff begins.

---

# SECTION 22 — HANDOFF GUIDELINES

## Purpose

Handoff Guidelines ensure Decision Story outputs can be consumed by downstream teams, agents, and governance processes without requiring rediscovery.

The objective is to make the Decision Story artifacts the:

Authoritative Business Design

for all downstream activities.

---

## Governing Rule

Downstream consumers should not need to revisit the BRD to understand:

- Business Context
- Business Outcomes
- Decisions
- Questions
- Signals
- Thresholds
- Actions
- Stories
- Accountability

The Decision Story artifacts must provide sufficient business design information to continue implementation.

---

## Handoff Process

### Step 01

Validate Discovery Completeness

---

### Step 02

Validate Traceability

---

### Step 03

Validate Human Authority

---

### Step 04

Validate Story Completeness

---

### Step 05

Validate Handoff Readiness

---

### Step 06

Publish Outputs

---

## Handoff Principles

### Principle 1

Business Intent Must Be Preserved

---

### Principle 2

Decision Logic Must Be Preserved

---

### Principle 3

Outcome Alignment Must Be Preserved

---

### Principle 4

Human Accountability Must Be Preserved

---

### Principle 5

Traceability Must Be Preserved

---

## REPORT_STORY_MATRIX Handoff

### Purpose

Validate Decision Logic before detailed design begins.

---

### Primary Consumers

- Business Owners
- Product Owners
- Report Designers

---

### Required Understanding

Consumers should understand:

- Business Outcomes
- Decisions
- Questions
- Signals
- Thresholds
- Actions

without reviewing additional documents.

---

## REPORT_STORY Handoff

### Purpose

Provide complete business design guidance.

---

### Primary Consumers

- Mockup Agent
- TRD Agent
- Semantic Design Agent
- Report Build Agent

---

### Required Understanding

Consumers should understand:

- Why the solution exists
- What outcomes improve
- What decisions are supported
- What actions occur
- How the story should be communicated

---

## Mockup Readiness Review

### Purpose

Ensure visual and layout design can begin.

---

### Verify

- Story Structure Defined
- Archetypes Defined
- Layout Concepts Defined
- Visual Recommendations Defined

---

### Validation Questions

Ask:

- Can a mockup be produced?
- Is the decision journey clear?
- Is information hierarchy understood?

---

## TRD Readiness Review

### Purpose

Ensure technical design can begin.

---

### Verify

- Decisions Defined
- Signals Defined
- Thresholds Defined
- Actions Defined
- Business Logic Defined

---

### Validation Questions

Ask:

- Is business logic complete?
- Can requirements be translated into technical specifications?

---

## Semantic Readiness Review

### Purpose

Ensure semantic model design can begin.

---

### Verify

- Signals Defined
- KPI Definitions Defined
- Business Measures Defined
- Business Questions Defined

---

### Validation Questions

Ask:

- Can measures be designed?
- Can dimensions be identified?
- Can traceability be preserved?

---

## Report Build Readiness Review

### Purpose

Ensure implementation teams can proceed.

---

### Verify

- Story Complete
- Visual Guidance Complete
- Layout Complete
- Governance Complete

---

### Validation Questions

Ask:

- Can report development begin?
- Are business expectations clear?
- Is ambiguity minimized?

---

## Human Authority Handoff

### Purpose

Ensure accountability survives downstream implementation.

---

### Verify

- Decision Owners Included
- Outcome Owners Included
- Action Owners Included
- Approval Authorities Included
- Escalation Authorities Included

---

### Validation Questions

Ask:

- Is accountability clear?
- Can ownership be preserved during implementation?

---

## Handoff Package Requirements

Every handoff package should provide:

### Business Context

---

### Business Outcomes

---

### Decision Framework

---

### Signal Framework

---

### Action Framework

---

### Story Framework

---

### Accountability Framework

---

### Traceability Framework

---

## Handoff Quality Standards

Good Handoffs Are:

- Complete
- Traceable
- Explainable
- Outcome Aligned
- Governance Aware

---

Poor Handoffs Are:

- Ambiguous
- Incomplete
- Missing Ownership
- Missing Traceability
- Missing Business Context

---

## Handoff Readiness Checklist

Verify:

□ Outcomes Defined

□ Decisions Defined

□ Signals Defined

□ Thresholds Defined

□ Actions Defined

□ Stories Defined

□ Ownership Defined

□ Traceability Preserved

□ Mockup Ready

□ TRD Ready

□ Semantic Ready

□ Build Ready

---

## Validation Rule

If downstream consumers cannot understand:

- Why the report exists
- What outcome improves
- What decision is supported
- Who owns accountability

the handoff is incomplete.

---

## Handoff Success Statement

Handoff succeeds when:

Business Problems

support Outcomes

Outcomes

support Decisions

Decisions

support Actions

and downstream teams can continue design and implementation without revisiting discovery activities.

The result is:

- Faster Delivery
- Better Consistency
- Stronger Governance
- Reduced Rework
- Preserved Business Intent
 
---

# SECTION 23 — COMMON DESIGN MISTAKES

## Purpose

Common Design Mistakes identify recurring failures that reduce the effectiveness of Decision Story design.

The objective is to proactively prevent:

- Weak Decision Support
- Poor Traceability
- Missing Accountability
- Incomplete Coverage
- Poor Handoffs
- Reporting-Driven Design

These mistakes should be reviewed throughout the discovery and design process.

---

## Governing Rule

Whenever a design concern is identified:

Review whether one or more common design mistakes are present.

Correct the issue before approval.

---

## Mistake 01 — Starting With Visuals

### Problem

The design process begins with:

Visual
↓
Dashboard
↓
Decision

instead of:

Business Outcome
↓
Decision
↓
Story
↓
Visual

---

### Symptoms

- Dashboard First Thinking
- Visual Wish Lists
- Visual Selection Before Discovery
- Layout Discussions Before Decisions

---

### Correction

Return to:

- Business Outcomes
- Decisions
- Questions
- Signals
- Actions

before discussing visuals.

---

## Mistake 02 — Starting With KPIs

### Problem

KPIs are treated as the purpose of reporting.

---

### Symptoms

- KPI Inventories
- Measure Collections
- Metrics Without Decisions
- Metrics Without Actions

---

### Correction

Ask:

```text
What decision becomes easier?

What action becomes easier?
```

before approving a KPI.

---

## Mistake 03 — Missing Business Outcomes

### Problem

The report is justified through data visibility instead of measurable outcomes.

---

### Symptoms

- No Outcome Owner
- No Success Measure
- No Outcome Target
- Unclear Business Value

---

### Correction

Identify:

- Business Outcome
- Outcome Owner
- Success Measure
- Success Target

before continuing.

---

## Mistake 04 — Decisions Without Owners

### Problem

Decisions exist without accountability.

---

### Symptoms

- Unnamed Decision Owners
- Shared Ownership
- Undefined Authority

---

### Risks

- Slow Decisions
- Escalation Delays
- Lack Of Accountability

---

### Correction

Define:

- Decision Owner
- Approval Authority
- Escalation Authority

before approval.

---

## Mistake 05 — Questions Without Decisions

### Problem

Questions exist without supporting a business decision.

---

### Symptoms

- Curiosity Questions
- Interesting Questions
- Reporting Questions
- Questions With No Action

---

### Correction

Remove questions that do not support:

- Outcomes
- Decisions
- Actions

---

## Mistake 06 — Signals Without Questions

### Problem

Metrics exist without supporting information needs.

---

### Symptoms

- Unused Measures
- Extra KPIs
- Unexplained Metrics

---

### Correction

Verify:

Question
↓
Signal

exists before approval.

---

## Mistake 07 — Thresholds Without Actions

### Problem

Thresholds exist without consequences.

---

### Symptoms

- Status Colors Only
- Passive Monitoring
- No Action Definition

---

### Correction

Every threshold should answer:

```text
What should happen next?
```

---

## Mistake 08 — Actions Without Outcomes

### Problem

Actions are defined without business value.

---

### Symptoms

- Activity For Activity's Sake
- Operational Noise
- Undefined Success

---

### Correction

Verify:

Business Outcome
↓
Decision
↓
Action

alignment.

---

## Mistake 09 — Stories Without Purpose

### Problem

Story sections become information containers.

---

### Symptoms

- Data Dumps
- Generic Pages
- Unstructured Analysis

---

### Correction

Every Story should answer:

```text
What decision becomes easier?

What action becomes clearer?
```

---

## Mistake 10 — Missing Human Authority

### Problem

Ownership and accountability are unclear.

---

### Symptoms

- Undefined Action Owners
- Missing Approval Authority
- Missing Escalation Ownership

---

### Risks

- Delayed Action
- Governance Issues
- Poor Adoption

---

### Correction

Document:

- Decision Owner
- Outcome Owner
- Action Owner
- Escalation Authority

---

## Mistake 11 — Ignoring Failure Modes

### Problem

Risks are not evaluated.

---

### Symptoms

- No Failure Analysis
- Missing Trust Assessment
- Missing Escalation Review

---

### Risks

- Poor Decisions
- Missed Risks
- Reduced Trust

---

### Correction

Review:

- Decision Failures
- Signal Failures
- Trust Failures
- Outcome Failures

before approval.

---

## Mistake 12 — Broken Traceability

### Problem

Artifacts cannot be traced to outcomes.

---

### Symptoms

- Orphan Signals
- Orphan Actions
- Orphan Stories
- Orphan Visuals

---

### Correction

Verify:

Business Problem
↓
Business Capability
↓
Business Outcome
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

remains intact.

---

## Mistake 13 — Weak Handoffs

### Problem

Downstream teams must rediscover requirements.

---

### Symptoms

- Missing Business Context
- Missing Decisions
- Missing Story Logic
- Missing Ownership

---

### Correction

Validate:

- Mockup Readiness
- TRD Readiness
- Semantic Readiness
- Build Readiness

before handoff.

---

## Mistake 14 — Removing Existing Knowledge

### Problem

Existing approved business logic is discarded during redesign.

---

### Symptoms

- Existing Decisions Removed
- Existing Signals Removed
- Existing Actions Removed
- Existing Stories Removed

without justification.

---

### Correction

Perform:

Regression Protection Review

before approving changes.

---

## Mistake 15 — Reporting Without Action

### Problem

The report provides information but does not improve behavior.

---

### Symptoms

- Visibility Only
- Monitoring Only
- No Recommended Response
- No Ownership

---

### Correction

Ask:

```text
What should happen because of this report?
```

If no answer exists:

Re-evaluate the design.

---

## Anti-Pattern Review Checklist

Before approval verify:

□ Outcomes Defined

□ Decisions Defined

□ Ownership Defined

□ Questions Support Decisions

□ Signals Support Questions

□ Thresholds Support Actions

□ Actions Support Outcomes

□ Stories Support Decisions

□ Traceability Preserved

□ Handoff Readiness Confirmed

□ Failure Modes Reviewed

□ Regression Protection Reviewed

---

## Common Design Mistakes Success Statement

Common Design Mistake Review succeeds when:

The design avoids:

- Reporting Driven Thinking
- KPI Driven Thinking
- Visual Driven Thinking
- Technology Driven Thinking

and remains:

- Outcome Driven
- Decision Driven
- Action Focused
- Human Governed
- Fully Traceable

throughout the design lifecycle.

---

# GUIDELINE SUCCESS STATEMENT

## Purpose

The Decision Story Guidelines define the official methodology for applying the Decision-Driven BI Framework.

The guidelines ensure every implementation follows a consistent process for transforming:

Business Requirements
↓
Business Context
↓
Business Outcomes
↓
Decision Design
↓
Story Design
↓
Decision Story Contract

into governed business design artifacts.

---

## Governing Principle

The purpose of reporting is not information delivery.

The purpose of reporting is:

Better Outcomes
↓
Better Decisions
↓
Better Actions

through structured and governed decision support.

---

## Discovery Principle

All design activities should follow:

Business Problem
↓
Business Capability
↓
Business Outcome
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

Discovery should never begin with:

Visuals

KPIs

Dashboards

Layouts

Technology

---

## Outcome Principle

Every reporting initiative should improve at least one:

- Business Outcome
- Operational Outcome
- Strategic Outcome

Every outcome should:

- Be Measurable
- Have Ownership
- Have Success Criteria
- Support Decision Making

---

## Human Governance Principle

The framework is:

AI Assisted
↓
Human Governed

AI may:

- Discover
- Analyze
- Recommend
- Explain
- Structure

AI may not:

- Own Decisions
- Approve Outcomes
- Assume Accountability
- Replace Human Authority

Final responsibility always remains with designated business stakeholders.

---

## Accountability Principle

Every critical element should identify:

- Decision Owner
- Outcome Owner
- Action Owner
- Approval Authority
- Escalation Authority

Accountability should remain visible throughout the entire design lifecycle.

---

## Traceability Principle

Every artifact should support:

Business Problem
↓
Business Capability
↓
Business Outcome
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

No orphan artifacts are permitted.

Every element should be explainable.

---

## Failure Awareness Principle

Every design should evaluate:

- Outcome Failures
- Decision Failures
- Signal Failures
- Trust Failures
- Operational Failures
- Governance Failures

Critical risks should be discovered before implementation begins.

---

## Handoff Principle

The Decision Story outputs should become:

The Authoritative Business Design

for downstream activities.

Downstream teams should understand:

- Business Intent
- Business Outcomes
- Decisions
- Actions
- Accountability
- Story Logic

without revisiting discovery.

---

## AI Readiness Principle

Every major element should answer:

```text
Why do I exist?

What outcome do I support?

What decision do I support?

What action becomes easier?

Who owns me?
```

Decision Story artifacts should be:

- Explainable
- Reusable
- Governed
- Transferable
- AI Ready

for future agents and future framework versions.

---

## Regression Protection Principle

Framework evolution should preserve:

- Approved Decisions
- Approved Questions
- Approved Signals
- Approved Thresholds
- Approved Actions
- Approved Stories
- Approved Business Rules
- Approved Traceability

Enhancements should strengthen proven business design rather than replace it unnecessarily.

---

## Promotion Readiness Principle

Decision Story outputs are promotion ready when:

- Business Context Is Defined
- Outcomes Are Defined
- Decisions Are Defined
- Signals Are Defined
- Actions Are Defined
- Stories Are Defined
- Ownership Is Defined
- Traceability Is Complete
- Failure Review Is Complete
- Handoff Readiness Is Confirmed

---

## Framework Success Criteria

The guidelines succeed when:

Every Business Problem

supports a Business Capability

Every Business Capability

supports a Business Outcome

Every Business Outcome

supports a Decision

Every Decision

supports Business Questions

Every Business Question

supports Signals

Every Signal

supports Thresholds

Every Threshold

supports Actions

Every Action

supports Business Improvement

Every Story

supports User Decisions

Every Visual

supports Business Action

while preserving:

- Accountability
- Traceability
- Governance
- Human Authority
- Outcome Alignment

throughout the design process.

---

## Final Success Statement

The Decision Story Guidelines succeed when reporting solutions become:

Outcome Driven

Decision Driven

Question Driven

Action Oriented

Human Governed

Traceable

Governed

AI Ready

business design artifacts that can be confidently handed to:

- Mockup Agent
- TRD Agent
- Semantic Design Agent
- Report Build Agent
- Future AI Agents

without loss of business intent, accountability, or traceability.

The result is:

- Better Outcomes
- Better Decisions
- Better Actions
- Better Governance
- Better Handoffs
- Better Reuse
- Better Long-Term Sustainability

across all future implementations.

