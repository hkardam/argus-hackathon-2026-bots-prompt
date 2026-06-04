You are a Principal Software Architect and Staff Engineer.

Your task is to generate a complete project skeleton for an AI-assisted hackathon.

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
2. architecture.md
3. schema.md
4. api-contracts.md

Your objective is NOT to implement business features.

Your objective is to generate a development-ready foundation that allows multiple developers to work in parallel.

Optimize for:

* Fast setup
* Clear ownership
* Minimal merge conflicts
* Reusable architecture
* Hackathon delivery speed

---

## SECTION 1: FRONTEND PROJECT STRUCTURE

Generate:

Complete folder structure.

Example:

src/

pages/

layouts/

components/

hooks/

services/

contexts/

store/

types/

constants/

utils/

assets/

Provide:

Purpose of each folder.

Recommended ownership boundaries.

---

## SECTION 2: BACKEND PROJECT STRUCTURE

Generate:

Complete folder structure.

Example:

src/

routes/

controllers/

services/

repositories/

middleware/

validators/

types/

config/

utils/

Provide:

Purpose of each folder.

Recommended ownership boundaries.

---

## SECTION 3: DATABASE STRUCTURE

Generate:

Migration strategy

Seed strategy

Database folder structure

Naming conventions

Recommended initialization process

---

## SECTION 4: SHARED TYPES

Generate:

Shared type organization.

Example:

types/

api.types.ts

user.types.ts

feature.types.ts

Provide recommendations for maintaining type consistency.

---

## SECTION 5: ROUTING STRUCTURE

Generate:

Frontend routes

Backend routes

Protected routes

Public routes

Admin routes (if applicable)

Routing organization strategy

---

## SECTION 6: STATE MANAGEMENT STRUCTURE

Generate:

State ownership strategy.

Global state

Feature state

Local state

Service layer responsibilities

Data fetching strategy

---

## SECTION 7: API CLIENT STRUCTURE

Generate:

Frontend API service organization.

Example:

services/

auth.service.ts

dashboard.service.ts

analytics.service.ts

Error handling strategy.

Request interceptor strategy.

Response handling strategy.

---

## SECTION 8: AUTHENTICATION FOUNDATION

Generate:

Authentication structure.

Authorization structure.

Protected route strategy.

Session handling strategy.

Token handling strategy.

Do NOT implement feature-specific auth logic.

---

## SECTION 9: ERROR HANDLING FOUNDATION

Generate:

Frontend error strategy.

Backend error strategy.

Validation strategy.

Logging strategy.

User-friendly error presentation strategy.

---

## SECTION 10: ENVIRONMENT STRUCTURE

Generate:

Frontend environment variables.

Backend environment variables.

Database configuration variables.

Development variables.

Production variables.

---

## SECTION 11: COMMON REUSABLE COMPONENTS

Identify components that should exist before feature development.

Examples:

Button

Modal

Loader

Toast

Error Boundary

Empty State

Layout Containers

Navigation Components

Generate complete reusable component inventory.

---

## SECTION 12: DEVELOPMENT BOOTSTRAP TASKS

Generate a step-by-step implementation plan.

Phase 1:

Project initialization

Phase 2:

Folder structure

Phase 3:

Database setup

Phase 4:

Authentication setup

Phase 5:

Shared components

Phase 6:

API foundation

Phase 7:

Developer handoff

---

## SECTION 13: PARALLEL DEVELOPMENT PREPARATION

Generate recommendations for:

4 developer team setup.

Shared modules.

Ownership boundaries.

Conflict prevention.

Branch strategy.

Merge strategy.

---

## SECTION 14: SKELETON COMPLETION CHECKLIST

The skeleton is complete when:

Frontend builds successfully.

Backend builds successfully.

Database connects successfully.

Authentication foundation exists.

API foundation exists.

Routing foundation exists.

Shared components exist.

Environment setup exists.

No business features implemented yet.

---

## SECTION 15: AI IMPLEMENTATION PROMPT

Generate a final implementation prompt that can be pasted into:

* ChatGPT
* Claude
* Codex
* Cursor
* Antigravity

The prompt should instruct the AI to:

1. Generate the complete skeleton.
2. Follow architecture.md.
3. Follow schema.md.
4. Follow api-contracts.md.
5. Avoid implementing business features.
6. Create only the foundation required for future feature development.

---

## OUTPUT REQUIREMENTS

Output:

1. Skeleton Architecture Document

2. Folder Structures

3. Development Bootstrap Plan

4. Parallel Development Recommendations

5. Skeleton Completion Checklist

6. AI Implementation Prompt

This output should allow a team to generate the base project and immediately begin feature development.
