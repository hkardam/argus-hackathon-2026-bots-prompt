You are acting as a senior product architect, solution analyst, data modeler, QA lead, and AI coding workflow designer.

I will provide one or more requirement documents / PRDs / BRDs / workflow documents / business rules documents.

Your job is to read them deeply and create a SINGLE, comprehensive, implementation-ready document that translates the requirements into a step-by-step coding prompt pack for an AI coding assistant (such as Antigravity / Cursor / Copilot / Claude / GPT coding mode).

This is not a summary task.
This is not a generic architecture task.
This is a faithful translation task.

Your output must preserve the source requirements as exactly as possible and convert them into a structured execution document so that a developer can start prompting and coding one by one with minimal further thinking.

PRIMARY GOAL
Create one complete document that:

1. Extracts all fields, workflows, validations, rules, roles, document types, statuses, calculations, constraints, templates, notifications, reports, and edge cases from the requirement documents.
2. Converts them into an implementation-ready system design.
3. Produces an ordered series of coding prompts to build the system step by step.
4. Clearly tells which prompts should use lighter/faster models and which should use stronger/reasoning-heavy models.
5. Includes testing prompts and exhaustive test coverage derived from the requirement itself.

CRITICAL BEHAVIOR RULES

- Be exhaustive.
- Do not omit business rules.
- Do not simplify away details.
- Do not replace exact requirement-defined fields with generic placeholders.
- Do not invent alternate workflows if the document already specifies them.
- If the source defines something ambiguously, mark it explicitly as “Ambiguity / Assumption Required”.
- If implementation-level constructs are not directly specified (for example DB tables), derive them faithfully from the requirements and clearly label them as “Derived Implementation Model”.
- Preserve numeric thresholds, percentages, tolerances, role restrictions, status transitions, checklists, mandatory fields, dependencies, and validation logic exactly.
- If multiple documents are provided, reconcile them carefully and call out conflicts.
- Keep the final document structured, dense, and execution-oriented.
- The final document must be usable directly by an engineering team in a hackathon or rapid-build setting.

WHAT TO PRODUCE

Create the final output as a SINGLE DOCUMENT with the following sections in this exact order:

SECTION 1 — Document Purpose and Usage

- Explain what this document is
- Explain how a developer should use it
- Explain that prompts should be executed one by one in order
- Mention where lighter vs stronger models should be used

SECTION 2 — Source Requirement Coverage Map
Create a traceability-style coverage section that lists:

- source modules / sections / features from the requirement docs
- whether each has been captured
- where it appears in this final document

SECTION 3 — Canonical Requirement Extraction
Extract the full requirement into structured form.

Include:
A. Business objective / product goal
B. User roles / actors
C. Role-wise permissions
D. Modules / features
E. End-to-end workflows
F. Statuses / state transitions
G. Entities / business objects
H. Field-level definitions
I. Required documents / attachments / evidence types
J. Eligibility rules / screening rules / business rules
K. Scoring rules / rubric / weights
L. Approval rules / reviewer rules / conflict rules
M. Financial rules / calculation rules / thresholds / tolerances
N. Reporting requirements
O. Compliance rules / exception rules
P. Notification / communication triggers
Q. Template / letter / agreement / export requirements
R. Search / filter / dashboard / analytics requirements
S. Audit log / security / RBAC requirements
T. Edge cases and special scenarios
U. Explicit ambiguities / missing information

For every rule, preserve:

- exact condition
- threshold / number / formula
- outcome
- whether it is hard validation, soft validation, warning, advisory AI check, or workflow block

SECTION 4 — Programme / Workflow / Module-wise Detailed Extraction
Break everything down feature by feature.

For each grant/programme/workflow/module defined in the requirement, include:

- purpose
- fields by section
- required document checklist
- validations
- dependencies
- derived UI components
- backend actions
- workflow states
- transitions
- notifications
- audit events
- reporting implications
- edge cases

If there are multiple programme types / application types / form types, create a separate subsection for each one.

SECTION 5 — Derived Implementation Data Model
Translate the requirements into an implementation-friendly system model.

Include:

- main entities
- relationships
- suggested tables / collections
- important enums
- status fields
- JSON-configurable structures where appropriate
- document storage model
- audit log model
- notification model
- reporting model
- review / approval / compliance model

Important:

- Clearly separate “directly specified in requirements” vs “derived for implementation”
- Keep field names explicit and implementation-friendly
- Include required indexes / ownership / references where relevant

SECTION 6 — Validation Matrix
Create a complete validation matrix.

For each validation include:

- validation ID
- module
- field(s)
- rule description
- validation type (frontend/backend/workflow/calculation/security)
- exact logic
- error/warning outcome
- blocking or non-blocking
- source basis from the requirement

SECTION 7 — Workflow and State Machine Matrix
For each main workflow:

- list all states
- allowed transitions
- transition conditions
- who can trigger the transition
- system actions triggered
- notifications triggered
- audit log events created
- invalid transitions that must be blocked

SECTION 8 — Security / Access / Audit Requirements
Include:

- role-based access matrix
- object ownership restrictions
- field-level visibility restrictions
- internal vs external notes/messages
- finance-sensitive fields / privacy-sensitive fields
- required audit events
- immutable or append-only items
- admin capabilities
- reviewer conflict restrictions
- approval segregation rules if present

SECTION 9 — Notifications / Documents / Generated Artefacts
Include:

- all notification events
- recipients
- trigger timing
- channel assumptions
- message purpose
- generated documents
- agreement/rejection/approval/report templates
- merge fields
- downloadable/exportable items

SECTION 10 — Recommended Tech Stack and Architecture for Rapid Build
Recommend a practical tech stack optimized for fast execution.

Include:

- frontend stack
- backend stack
- DB/storage/auth choice
- testing stack
- document/PDF/export choice
- AI integration strategy
- where deterministic logic must be used
- where LLM advisory logic may be used
- risk-reduction suggestions for hackathon delivery

SECTION 11 — Ordered Build Plan
Create a detailed implementation order.

This must be sequenced logically according to:

1. system setup
2. core data model
3. auth and RBAC
4. workflow order from intake to final closure
5. reporting/compliance
6. notifications/audit
7. hardening/testing/demo readiness

For each implementation step include:

- objective
- what to build
- dependencies
- expected output
- owner suggestion if a 4-person team is building
- estimated complexity (low / medium / high)

SECTION 12 — Model Strategy for Prompting
For each coding prompt later in the document, specify which model class to use:

- Flash / Lite / Fast model for simpler scaffolding, CRUD, layout, plumbing, boilerplate, basic tests
- Pro / Reasoning / Strong model for architecture, schema design, complex validation, workflow logic, AI prompt design, test design, integration fixes

Also explain:

- why a stronger model is needed
- how to avoid wasting stronger-model quota

SECTION 13 — Master Shared Context Block
Create one reusable shared context block to prepend to every coding prompt.

This block must contain:

- project name
- goal
- architecture rules
- quality rules
- role definitions
- implementation constraints
- AI usage constraints
- code quality expectations
- non-goals / scope boundaries

SECTION 14 — Ordered Coding Prompt Pack
This is the most important section.

Create a step-by-step series of prompts to be executed one by one in the correct order.

Requirements for this section:

- each prompt must be comprehensive
- each prompt must assume the requirement document has already been read
- each prompt must include enough detail so the coding model does not “generalize away” requirement specifics
- each prompt must be written in a way that a developer can directly copy-paste it into an AI coding tool
- prompts must mention the exact requirement-derived fields/rules/modules relevant to that step
- prompts must specify model recommendation: Flash or Pro
- prompts must specify expected output
- prompts must tell the model not to rewrite unrelated files
- prompts must favor compile-ready code
- prompts must keep code modular and implementation-friendly

The prompt pack must cover, in order:

1. architecture and repo blueprint
2. project scaffold
3. schema / migrations / seed data
4. auth / RBAC / route guards
5. public catalogue / discoverability / entry screens if relevant
6. applicant or primary intake flow
7. profile / document vault / dynamic forms
8. hard validation engine
9. screening / pre-check / decision support
10. reviewer / evaluator / scoring module
11. approval / decision / outcome generation
12. agreement / document / disbursement / fulfillment flow
13. reporting / compliance / post-approval tracking
14. notifications / communication / admin / audit
15. AI-assisted modes if required
16. unit tests
17. integration / E2E tests
18. demo hardening / seed polishing / README

SECTION 15 — Exhaustive Test Case Pack
Generate tests directly from the requirement.

Include:

- field validations
- document checklist validations
- eligibility checks
- workflow/state transition checks
- role/RBAC checks
- scoring/review checks
- financial/calculation checks
- compliance/reporting checks
- notifications
- audit logging
- E2E happy paths
- E2E failure paths
- edge cases

For every test case include:

- test ID
- module
- title
- preconditions
- input
- expected result
- test type (unit / integration / E2E)

SECTION 16 — Assumptions, Ambiguities, and Open Questions
List anything not explicitly defined in the requirement documents but needed for implementation.

For each item:

- describe ambiguity
- explain why it matters
- provide the safest default assumption
- clearly label it as assumption, not source truth

IMPORTANT OUTPUT QUALITY RULES

- The document must feel like a rigorous implementation pack, not a casual summary.
- Preserve exact requirement fidelity wherever possible.
- Organize content with strong headings and subheadings.
- Use tables where useful for structured extraction.
- Use bullet lists only where they improve clarity.
- Keep the coding prompts in code blocks for easy copy-paste.
- Keep the shared context block in its own code block.
- Keep each prompt clearly numbered.
- Make the final result long, detailed, and operationally useful.

VERY IMPORTANT EXTRACTION RULE
Before writing the prompt pack, first internally extract all business rules, fields, validations, statuses, roles, and documents from the source files.
Do not start generating the prompt pack until you have performed that extraction.

VERY IMPORTANT FIDELITY RULE
Whenever the source documents define:

- exact field names
- exact numeric constraints
- exact workflow statuses
- exact document names
- exact report sections
- exact reviewer rules
- exact decision conditions
  you must carry them forward exactly into the output.

FINAL INSTRUCTION
Produce the final answer as one complete, polished document.
Do not give a short summary first.
Do not ask follow-up questions unless the source documents are unreadable or critically incomplete.
Start directly with the final document.
