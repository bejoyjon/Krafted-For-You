# Krafted For You Agent Automation Architecture 2026

Date: `2026-05-24`

Scope: first-pass AI-agent architecture for `Customer Emotion Intelligence` and `Curated Option Architecture`.

## 1. Automation Goal

Agents should reduce human effort in understanding inquiries and drafting options while preserving human control over taste, pricing, promises, and customer-facing messages.

## 2. First Agents To Build

| Agent | Purpose | Output |
|---|---|---|
| Brief Extraction Agent | Turns messy inquiry notes into structured brief | Brief, missing fields, confidence score |
| Emotion Interpretation Agent | Infers likely desired emotional outcome | Emotional intent, assumptions, questions |
| Option Path Agent | Drafts 2-3 gift directions | Option paths with fit reasoning |
| Proposal Draft Agent | Converts approved options into customer-ready draft | Proposal draft requiring human approval |
| Learning Agent | Reviews outcomes weekly | Template changes and conversion learnings |

## 3. Human Approval Matrix

| Task | Agent can do | Human must approve |
|---|---|---|
| Extract brief | Yes | Only if ambiguous |
| Infer emotional intent | Draft only | Yes |
| Ask missing questions | Draft only | Yes before sending |
| Generate option paths | Draft only | Yes |
| Quote price | Draft assumptions only | Yes |
| Promise delivery date | No | Yes |
| Send customer message | No | Yes |
| Update learning log | Yes | Review weekly |

## 4. Data Required

Agents need:

- lead brief fields,
- offer lane definitions,
- recipient archetypes,
- occasion playbooks,
- product and keepsake menus,
- budget bands,
- sourcing constraints,
- proof examples,
- founder correction history.

## 5. Prompt Output Format

### Brief Extraction Output

```text
Brief completeness score:
Customer:
Occasion:
Recipient:
Relationship:
Desired feeling:
Budget:
Needed-by date:
Style preference:
Known constraints:
Missing questions:
Assumptions:
Confidence:
```

### Option Generation Output

```text
Option A:
- Concept:
- Emotional intent:
- Best fit:
- Inclusions:
- Handmade element:
- Personalization:
- Budget band:
- Lead-time risk:
- Why this fits:

Option B:
...

Option C:
...

Founder decisions needed:
Customer questions needed:
```

## 6. Tactical Challenges

| Challenge | Mitigation |
|---|---|
| Agent makes generic suggestions | Feed past orders, playbooks, and brand rules |
| Agent overpromises | Force risk and human approval fields |
| Agent misses taste nuance | Founder rates outputs and corrections are logged |
| Too much review burden | Use agents only after brief reaches minimum completeness |
| Data is scattered | Start with a simple structured brief template |

## 7. Feedback Loop

Weekly learning agent should review:

- number of briefs processed,
- missing fields frequency,
- founder corrections,
- option selected,
- proposal conversion,
- customer confusion,
- repeated sourcing needs.

Monthly, update:

- prompts,
- brief fields,
- offer playbooks,
- option templates,
- refusal rules.

## 8. Tie To First-Year Priorities

| Priority | Agent contribution |
|---|---|
| Become Legible | Agents enforce consistent language and brief structure |
| Productize Without Losing Bespoke | Agents use option playbooks while preserving personalization |
| Build A Proof Library | Agents convert order data into story drafts |
| Build Vendor Memory | Agents identify repeated sourcing patterns |
| Build Agent-Readable Business Memory | This architecture creates the memory schema |

