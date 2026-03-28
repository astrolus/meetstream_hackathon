# Med Device Revenue Copilot (Sales + Customer Success)

## Overview

A multi-agent AI system that joins sales and support conversations, surfaces real-time insights to reps, and autonomously prepares post-meeting actions—while keeping the human in control. It aids the medical device sales rep here with surfacing the right information for them, shows the real-time actions it's performing to aid it as well as providing an overall sentiment of the meeting with the doctor. It's overall purpose is to aid the medical device sales rep with closing the deal with the doctor.

---

## Frontend Experience (Rep Interface)

### Live Meeting View

* Real-time transcription and summarized insights
* Instant answers to doctor questions using internal data + context
* Key signals surfaced (buy intent, objections, concerns)

### Sentiment & Call Health

* Live sentiment bar indicating how the conversation is trending
* Highlights risk moments (confusion, hesitation, dissatisfaction)

### Action Panel (Human-in-the-Loop)

* Background agents generate real-time meeting actions
* Each action requires explicit **Approve / Deny** from the rep

Examples:

* Draft follow-up email → Approve / Deny
* Schedule next meeting → Approve / Deny
* CRM update → Approve / Deny
---

## Architecture: Multi-Agent Orchestration

### Head Agent (Orchestrator)

* Joins meetings and maintains full context
* Interprets conversation intent and routes tasks
* Aggregates outputs from sub-agents
* Surfaces insights + actions to the frontend

---

### Specialized Sub-Agents

#### Scheduler Agent

* Schedules follow-up meetings if needed
* updates calendar and plans new meeting for new leads identified

#### Analytics Agent

* Pulls sales data and historical records
* Assesses deal health and recommends next steps
* Provides real time data in response to doctor questions

#### Background Communication Agent

* Drafts follow-ups email content and meeting summaries
* Adapts messaging based on context and tone

---

