# Med Device Revenue Copilot (Sales + Customer Success)

## Overview

A multi-agent AI system that joins sales and support conversations, surfaces real-time insights to reps, and autonomously prepares post-meeting actions—while keeping the human in control.

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

* Background agents generate post-meeting actions in real time
* Each action requires explicit **Approve / Deny** from the rep

Examples:

* Draft follow-up email → Approve / Deny
* Schedule next meeting → Approve / Deny
* CRM update → Approve / Deny
* Refund / resolution suggestion → Approve / Deny

---

## Architecture: Multi-Agent Orchestration

### Head Agent (Orchestrator)

* Joins meetings and maintains full context
* Interprets conversation intent and routes tasks
* Aggregates outputs from sub-agents
* Surfaces insights + actions to the frontend

---

### Specialized Sub-Agents

#### CRM & Data Agent

* Prepares CRM updates and structured notes
* Creates/updates leads and opportunities

#### Analytics Agent

* Pulls sales data and historical records
* Assesses deal health and recommends next steps

#### Trust & Decision Agent

* Scores customer claims and evaluates resolutions
* Flags high-risk or anomalous scenarios

#### Support & Bug Triage Agent

* Extracts and classifies issues raised
* Prepares bug reports and internal routing

#### Compliance Agent

* Validates outputs against med device regulations
* Flags non-compliant suggestions before surfacing

#### Communication Agent

* Drafts follow-ups and meeting summaries
* Adapts messaging based on context and tone

---

## Post-Meeting Key Functions (One-Liners)

* Generate meeting summary and key takeaways
* Extract and classify customer intent
* Draft follow-up email for approval
* Recommend and schedule next steps
* Prepare CRM updates for approval
* Log and triage product issues
* Validate all outputs for compliance
* Score deal health and customer sentiment
* Flag items requiring human escalation
* Trigger resolution recommendations (pending approval)

---

## Key Insight

The system doesn’t replace the rep—it **runs in parallel**, handling analysis and prep work while the rep stays in control of final decisions.

---

## Positioning

**A real-time AI copilot that thinks, prepares, and executes in the background—while the sales rep stays the decision-maker.**
