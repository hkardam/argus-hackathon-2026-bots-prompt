You are a Principal Software Architect and Technical Program Manager.

Your task is to generate a single consolidated implementation context document for a hackathon development team.

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

1. requirements.md
2. prd.md
3. architecture.md
4. schema.md
5. api-contracts.md
6. feature-ownership.md

Your objective is NOT to reproduce these documents.

Your objective is to compress all critical implementation information into a concise but complete development context.

The output should be optimized for:

* AI coding assistants
* Feature implementation
* Code review
* Testing
* Merge review

The output should be understandable without reading any of the original documents.

---

## SECTION 1: PROJECT SUMMARY

Provide:

Project Name

Problem Being Solved

Target Users

Business Objective

Core Value Proposition

One paragraph maximum.

---

## SECTION 2: MVP SUMMARY

List:

Must Have Features

Should Have Features

Stretch Features

Clearly identify:

What MUST be completed during the hackathon.

---

## SECTION 3: TECH STACK

Frontend

Backend

Database

Deployment

Development Tools

State Management

UI Libraries

Authentication Strategy

---

## SECTION 4: SYSTEM ARCHITECTURE SUMMARY

Provide:

High-level architecture

Major modules

Data flow

Key design decisions

Implementation constraints

Only implementation-relevant details.

---

## SECTION 5: FRONTEND STRUCTURE

Provide:

Routes

Pages

Layouts

Reusable Components

Hooks

Services

State Management

Folder Structure

Keep concise.

---

## SECTION 6: BACKEND STRUCTURE

Provide:

Routes

Controllers

Services

Repositories

Middleware

Folder Structure

Key responsibilities

---

## SECTION 7: DATABASE SUMMARY

Provide:

All tables

Purpose of each table

Primary relationships

Important constraints

Do not include full DDL.

Only implementation-relevant summaries.

---

## SECTION 8: API SUMMARY

Provide:

All APIs grouped by feature.

For each API:

Method

Route

Purpose

Authentication Requirement

Do not include full request/response payloads.

---

## SECTION 9: FEATURE OWNERSHIP

For every developer provide:

Owned Features

Owned APIs

Owned Pages

Owned Components

Owned Tables

Owned Services

Dependencies

---

## SECTION 10: DEVELOPMENT RULES

Generate mandatory rules.

Examples:

* Do not change database schema.
* Do not change API contracts.
* Do not rename routes.
* Do not introduce new libraries without approval.
* Do not modify files owned by another developer.
* Follow established folder structure.
* Keep business logic inside services.

Generate all relevant rules.

---

## SECTION 11: FILE OWNERSHIP RULES

For every developer provide:

Allowed Areas

Restricted Areas

Shared Areas

Merge Responsibilities

---

## SECTION 12: IMPLEMENTATION GUIDELINES

Generate implementation standards.

Examples:

Frontend:

* Use reusable components.
* Keep pages thin.
* Use services for API calls.

Backend:

* Controllers handle requests.
* Services contain business logic.
* Repositories contain database access.

Database:

* No schema modifications.
* Follow naming conventions.

---

## SECTION 13: INTEGRATION CHECKLIST

Generate checklist.

Before merge verify:

API contract compliance

Database compliance

Authentication compliance

Ownership compliance

Build success

---

## SECTION 14: TESTING CHECKLIST

Generate:

Feature Testing

API Testing

Integration Testing

Demo Testing

---

## SECTION 15: DEMO CRITICAL FEATURES

Identify:

Features that absolutely must work during demo.

Features that can fail without ruining the presentation.

---

## SECTION 16: QUICK REFERENCE

Generate:

Project in 30 Seconds

Project in 2 Minutes

Project in 5 Minutes

This section should allow any developer or AI assistant to understand the entire system quickly.

---

## OUTPUT REQUIREMENTS

The output must:

* Be concise
* Be implementation-focused
* Be less than 5 pages when possible
* Contain all critical information needed during development
* Replace the need to repeatedly read the original planning documents

The final output should be saved as:

master-context.md

This document becomes the official development source of truth for the entire hackathon team.
