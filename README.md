# PathPredict – Internship Readiness & Career Intelligence Platform

PathPredict is an AI-powered career guidance platform that helps students find
internships they can actually get by analyzing their skills, academic year,
and availability. Instead of listing random internships, PathPredict provides
clarity, readiness prediction, and a clear learning path.

---

## Problem Statement

Many students fail to secure internships not because they lack potential, but
because they lack clarity:
- Which internships are they eligible for?
- What skills are missing?
- Should they apply now or upskill first?
- How long will it take to become internship-ready?

Existing platforms mostly list opportunities without personalized guidance.

---

## Solution

PathPredict acts as a **decision-making system**, not just an internship portal.
It evaluates student profiles, predicts readiness, highlights skill gaps, and
guides students with actionable next steps.

---

## Key Features

- Student profile intake (year, skills, role, weekly hours)
- Internship search portal (API-ready)
- Internship readiness score (0–100)
- Apply Now / Upskill First decision
- Missing skills identification
- Career path & timeline prediction
- What-if simulator (add skills or time)
- Internship comparison mode
- LinkedIn-based mentorship guidance
- Protected routes with authentication

---

## System Architecture

Frontend (React + TypeScript)
        ↓
Google Cloud Function (Backend API)
        ↓
Google ADK-based Agent Orchestration
        ↓
Gemini AI Reasoning
        ↓
JSON Response → Dashboard UI

---

## Google Technologies Used

### 1. Gemini CLI (Google CLI)

Gemini CLI was used during development for **prompt engineering and validation**.
Career reasoning prompts were tested using `gemini chat`. During testing, the
free-tier quota was exhausted, confirming real API usage.

---

### 2. Google ADK (Agent Development Kit – Conceptual Implementation)

PathPredict follows **Google ADK principles** using a multi-agent architecture.

Agents used:
- Profile Agent – processes student input
- Skill Match Agent – compares skills with role requirements
- Readiness Agent – calculates readiness score
- Timeline Agent – predicts preparation time
- Decision Agent – determines Apply or Upskill decision

All agents are orchestrated through a central controller.

---

### 3. Google Cloud

The backend is deployed as a **Google Cloud Function** using Node.js.  

## How It Works

1. Student logs in and enters profile details
2. Frontend sends data to Google Cloud backend
3. ADK agents process the data step by step
4. Gemini AI generates reasoning and explanation
5. Backend returns readiness, decision, and timeline
6. Frontend dashboard displays results

---

## Tech Stack

- Frontend: React, TypeScript, Tailwind CSS
- Backend: Node.js, Google Cloud Functions
- AI: Gemini API
- Architecture: Google ADK (agent-based)
- Authentication: Context-based auth

---

## Why PathPredict Is Different

- Not just an internship listing platform
- Not generic career advice
- A clarity-driven decision system
- Predicts readiness and timelines
- Explains why a student should apply or upskill

---

## Judge Summary

PathPredict uses **Gemini CLI** for prompt engineering, **Google ADK** for
agent-based decision logic, and **Google Cloud Functions** to deploy a real,
scalable AI-powered backend for internship readiness prediction.

---

## Author

Ankit  
PathPredict – Career Intelligence Platform
the frontend.

---
