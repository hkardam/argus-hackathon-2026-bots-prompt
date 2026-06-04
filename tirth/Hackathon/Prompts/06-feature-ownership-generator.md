You are a Principal Engineering Manager responsible for organizing a 4-person team for an 8-hour AI-assisted hackathon.

Technology Stack:

Frontend:

* React
* TypeScript
* Vite
* Tailwind

Backend:

* Node.js
* Express
* TypeScript

Database:

* PostgreSQL

Inputs:

1. prd.md
2. architecture.md
3. schema.md
4. api-contracts.md

Your objective is to create a feature ownership plan that maximizes:

* Parallel development
* Minimal merge conflicts
* Minimal communication overhead
* Fast MVP delivery
* Clear accountability

Do NOT organize by frontend/backend.

Do NOT organize by technical layers.

Instead organize by vertical feature ownership.

Each developer must own:

* Frontend
* Backend
* Database usage
* API integration
* Testing

for their assigned feature.

---

## SECTION 1: SYSTEM FEATURE BREAKDOWN

Identify all major system features.

For each feature provide:

Feature Name

Description

Business Value

Priority

MVP Status:

* Must Have
* Should Have
* Nice To Have

Complexity:

* Low
* Medium
* High

---

## SECTION 2: TEAM STRUCTURE

Assume 4 developers.

Assign:

Developer A

Developer B

Developer C

Developer D

Balance workload as evenly as possible.

Provide reasoning for assignments.

---

## SECTION 3: FEATURE OWNERSHIP

For EACH developer provide:

Feature Name

Business Goal

User Flows Owned

Pages Owned

Frontend Components Owned

Backend Routes Owned

Controllers Owned

Services Owned

Database Tables Used

API Endpoints Owned

State Management Ownership

Testing Responsibility

Demo Responsibility

Dependencies

Expected Deliverables

---

## SECTION 4: FILE OWNERSHIP

Generate explicit ownership.

Example:

Developer A

Frontend Files:

src/pages/auth/*
src/components/auth/*

Backend Files:

src/routes/auth/*
src/controllers/auth/*
src/services/auth/*

Database Tables:

users
sessions

Owned APIs:

POST /auth/login
POST /auth/register
GET /auth/profile

---

## SECTION 5: FORBIDDEN FILES

For every developer generate:

Files that should NOT be modified.

Example:

Developer A

Must Not Modify:

dashboard/*
analytics/*
reports/*

Reason:
Owned by Developer C

---

## SECTION 6: DEPENDENCY GRAPH

Identify:

Feature Dependencies

Blocking Dependencies

Shared Resources

Shared Components

Potential Conflict Areas

Recommend mitigation strategies.

---

## SECTION 7: MERGE STRATEGY

Generate:

Branch Structure

Recommended Branch Names

Merge Order

Merge Frequency

Conflict Prevention Rules

Recommended Git Workflow

Example:

main

feature/auth

feature/core-feature

feature/dashboard

feature/analytics

---

## SECTION 8: MVP EXECUTION PLAN

Provide implementation order.

Hour 1

Hour 2

Hour 3

Hour 4

Hour 5

Hour 6

Hour 7

Hour 8

Identify:

Critical Path Features

Features that must be completed first

Features that can be delayed

---

## SECTION 9: AI DEVELOPMENT GUIDELINES

Generate instructions for all developers.

Rules:

Do not modify schema.

Do not modify API contracts.

Do not modify another developer's owned files.

Do not introduce new libraries without approval.

Do not rename routes.

Do not rename database entities.

All changes must remain within assigned ownership boundaries.

---

## SECTION 10: OUTPUT SUMMARY

Generate:

1. Team Assignment Matrix
2. Feature Ownership Matrix
3. File Ownership Matrix
4. API Ownership Matrix
5. Database Ownership Matrix
6. Dependency Matrix
7. Merge Strategy Summary

The output should be directly usable as feature-ownership.md and become the official ownership contract for the entire hackathon team.
