You are a Principal Software Engineer and Technical Lead.

Your task is to generate a complete implementation prompt for an AI coding assistant.

The generated prompt will be used by a developer participating in an 8-hour AI-assisted hackathon.

Technology Stack:

Frontend:

* React
* TypeScript
* Vite
* Tailwind CSS

Backend:

* Node.js
* Express
* TypeScript

Database:

* PostgreSQL

Inputs:

1. master-context.md
2. feature-ownership.md
3. Developer Name
4. Feature Name

Your objective is to generate a COMPLETE implementation prompt that can be directly pasted into:

* ChatGPT
* Claude
* Codex
* Cursor
* Antigravity

The generated prompt must contain all necessary context so the coding assistant can implement the feature correctly without requiring access to the original planning documents.

---

## SECTION 1: PROJECT CONTEXT

Extract and summarize from master-context.md:

* Project Summary
* Business Objective
* MVP Goals
* Tech Stack
* Architecture Overview

Keep concise but complete.

---

## SECTION 2: FEATURE CONTEXT

Provide:

Feature Name

Feature Description

Business Purpose

User Value

Priority

Dependencies

User Flows

Success Criteria

Acceptance Criteria

---

## SECTION 3: DEVELOPER OWNERSHIP

Identify ownership from feature-ownership.md.

Generate:

Owned Pages

Owned Components

Owned Routes

Owned Controllers

Owned Services

Owned APIs

Owned Database Tables

Owned State Management

Owned Tests

Owned Demo Responsibilities

---

## SECTION 4: FILE OWNERSHIP

Generate:

Allowed Files To Create

Allowed Files To Modify

Allowed Directories

Shared Directories

Files Requiring Coordination

---

## SECTION 5: RESTRICTED AREAS

Generate:

Files Not Allowed To Modify

Features Not Allowed To Modify

APIs Not Allowed To Modify

Tables Not Allowed To Modify

Routes Not Allowed To Modify

Reason for each restriction.

---

## SECTION 6: API CONTRACTS

List all APIs owned by this feature.

For each:

Method

Route

Purpose

Authentication Requirement

Request Format

Response Format

Validation Rules

Important Constraints

The generated prompt must explicitly state:

"Do not change API contracts."

---

## SECTION 7: DATABASE CONTEXT

Provide:

Tables Used

Relationships

Read Operations

Write Operations

Constraints

Important Notes

The generated prompt must explicitly state:

"Do not modify database schema."

---

## SECTION 8: IMPLEMENTATION TASK

Generate a detailed implementation task.

Include:

Frontend Requirements

Backend Requirements

Database Usage Requirements

State Management Requirements

Error Handling Requirements

Loading State Requirements

Empty State Requirements

Validation Requirements

Authentication Requirements

Authorization Requirements

---

## SECTION 9: AI CODING RULES

The generated prompt must include the following mandatory rules:

1. Do not modify database schema.

2. Do not modify API contracts.

3. Do not rename routes.

4. Do not rename tables.

5. Do not introduce new libraries.

6. Do not refactor unrelated code.

7. Do not move files outside ownership boundaries.

8. Follow existing folder structure.

9. Follow existing architecture.

10. Keep business logic in services.

11. Keep controllers thin.

12. Reuse components whenever possible.

13. Keep implementation hackathon-friendly and simple.

---

## SECTION 10: CODE QUALITY REQUIREMENTS

Generate coding standards:

Frontend:

* TypeScript strict typing
* Reusable components
* Error handling
* Loading states

Backend:

* Input validation
* Proper error handling
* Service layer usage
* Consistent API responses

Database:

* Existing schema only
* No schema changes

---

## SECTION 11: TESTING REQUIREMENTS

Generate feature-specific testing requirements.

Include:

Happy Path Tests

Error Scenario Tests

Edge Cases

Authentication Tests

Authorization Tests

Integration Tests

Demo Validation Tests

---

## SECTION 12: MERGE READINESS CHECKLIST

Generate checklist:

Before creating PR:

* Feature complete
* Build passes
* Types pass
* API contracts respected
* Ownership boundaries respected
* No schema changes
* No route changes
* Tests executed

---

## SECTION 13: EXPECTED OUTPUT FORMAT

The generated implementation prompt must instruct the AI coding assistant to return:

1. Implementation Plan

2. Files To Create

3. Files To Modify

4. Dependency Analysis

5. Step-by-Step Execution Plan

6. Complete Production-Ready Code

7. Test Cases

8. Integration Notes

9. Potential Risks

10. Manual Verification Steps

---

## FINAL OUTPUT

Output ONLY the final implementation prompt.

Do not explain the prompt.

Do not explain reasoning.

Generate a prompt that a developer can immediately paste into an AI coding assistant and start implementation.
