# DOCUMENT_NAMING_STANDARD_v1.0

## Decision-Driven BI Agent Platform

Version: 1.0

Status: Approved

Maturity: Platform Standard

Purpose:
Define a consistent naming convention for all platform repositories, framework artifacts, contracts, standards, templates, agents, and generated outputs.

---

# PURPOSE

This standard ensures:

- Consistent naming
- Predictable file discovery
- Easier AI navigation
- Easier repository maintenance
- Reduced ambiguity

across all platform artifacts.

---

# CORE PRINCIPLE

File names should answer:

What is this artifact?

before answering:

What version is it?

---

# STANDARD FORMAT

Use:

ARTIFACT_NAME_VERSION

Example:

REPORT_STORY_v1.0.md

SEMANTIC_MODEL_SPEC_v1.0.md

MEASURE_CONTRACT_v1.0.md

---

# CHARACTER RULES

Use:

- Uppercase Names
- Underscores
- Version Suffix

Example:

REPORT_STORY_v1.0.md

Avoid:

ReportStory.md

report-story.md

Report_Story.md

reportstory.md

---

# PLATFORM FOUNDATION DOCUMENTS

Purpose:

Platform Startup Sequence

Format:

01_NAME_vX.X.md

Examples:

01_TASK_BREAKDOWN_v1.0.md

02_PROJECT_INIT_v2.0.md

03_AGENT_REPOSITORY_STANDARD_v1.0.md

04_SKILL_PACKAGE_STANDARD_v1.0.md

---

# FRAMEWORK DOCUMENTS

Purpose:

Framework Knowledge

Format:

NAME_vX.X.md

Examples:

FRAMEWORK_README_v1.0.md

DECISION_DRIVEN_BI_ARCHITECTURE_v3.0.md

FRAMEWORK_DOCUMENT_TEMPLATE_v1.0.md

---

# STANDARDS

Format:

NAME_STANDARD_vX.X.md

Examples:

DOCUMENT_NAMING_STANDARD_v1.0.md

VERSIONING_STANDARD_v1.0.md

GOVERNANCE_STANDARD_v1.0.md

REPORT_DESIGN_STANDARD_v1.0.md

---

# GUIDELINES

Format:

NAME_GUIDELINES_vX.X.md

Examples:

DECISION_STORY_GUIDELINES_v1.0.md

SEMANTIC_DESIGN_GUIDELINES_v1.0.md

---

# TEMPLATES

Format:

NAME_TEMPLATE_vX.X.md

Examples:

REPORT_STORY_TEMPLATE_v1.0.md

TRD_TEMPLATE_v1.0.md

---

# CONTRACTS

Format:

NAME_CONTRACT_vX.X.md

Examples:

BRD_CONTRACT_v1.0.md

DSC_CONTRACT_v1.0.md

SEMANTIC_CONTRACT_v1.0.md

---

# GENERATED ARTIFACTS

Format:

NAME_vX.X.md

Examples:

REPORT_STORY_v1.0.md

REPORT_STORY_MATRIX_v1.0.md

TRD_v1.0.md

DATA_MODEL_MATRIX_v1.0.md

SEMANTIC_MODEL_SPEC_v1.0.md

MEASURE_CONTRACT_v1.0.md

---

# AGENT REPOSITORY FILES

Use fixed names.

No version numbers.

Examples:

README.md

PROJECT_INIT.md

AGENT_README.md

SKILL_BLUEPRINT.md

skill.md

CHANGELOG.md

---

# AGENT FOLDER NAMES

Use lowercase.

Use hyphens.

Examples:

decision-story-agent

mockup-agent

trd-agent

semantic-design-agent

semantic-build-agent

report-build-agent

---

# FOLDER NAMES

Use lowercase.

Use hyphens if needed.

Examples:

inputs

standards

guidelines

templates

contracts

governance

examples

outputs

test-run

---

# VERSION LOCATION RULE

The version always appears at the end.

Correct:

REPORT_STORY_v1.0.md

Incorrect:

v1.0_REPORT_STORY.md

---

# SUCCESS CRITERIA

The naming standard succeeds when:

- Files are easy to locate
- Files are easy to understand
- AI agents can identify artifacts consistently
- Repository structures remain predictable

---

# PROMOTION STATUS

Version:

1.0

Status:

APPROVED

Maturity:

Platform Standard