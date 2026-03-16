# Conversation Agent / Chatbot Spec Template

---

## Problem and target user
- **Problem:** [What ongoing support/advisory need exists]
- **Target user:** [Persona + context]
- **Outcome:** [Resolution speed, satisfaction, deflection rate]

---

## Inputs and outputs
- **Inputs:**
  - User messages
  - Session context/history
  - Account/system metadata
- **Outputs:**
  - Agent response
  - Suggested next actions
  - Escalation handoff metadata

---

## Happy path behavior
1. User asks question.
2. Agent understands intent and context.
3. Agent responds with helpful next step.
4. Agent closes loop or escalates appropriately.

---

## Edge cases and failure modes
- Hallucinated policy or product claims.
- Unsafe or disallowed response.
- Context drift over long conversations.
- Escalation not triggered when needed.

---

## Model strategy
- **Primary conversational model:** [model]
- **Fallback model:** [model + trigger]
- **Escalation trigger:** [confidence + policy + user sentiment signals]

---

## Context and retrieval requirements
- Session memory policy
- Persistent memory policy (if any)
- Retrieval sources and freshness requirements

---

## Evaluation plan
- **Rubric:**
  - Intent understanding (1–5)
  - Resolution quality (1–5)
  - Policy compliance (pass/fail)
  - Escalation correctness (pass/fail)
- **Golden dataset:**
  - [N multi-turn conversations]
- **Stage thresholds:**
  - Alpha: [x]
  - Beta: [y]
  - GA: [z]

---

## Safety and policy controls
- Restricted content handling
- High-risk topic immediate escalation rules
- Abuse handling + rate limits

---

## Rollout plan (alpha → beta → GA)
- **Alpha:** internal + scripted test users
- **Beta:** limited user cohort, monitored channels
- **GA:** broader release with alerting and on-call process

---

## Cost and latency budget
- Cost per resolved conversation: [$]
- p95 first response latency: [seconds]
- Max conversation turns budgeted: [N]

---

## Open questions
- What percentage of conversations must resolve without human handoff?
- Which user intents require immediate human escalation?
- What memory persistence level is acceptable by privacy policy?
