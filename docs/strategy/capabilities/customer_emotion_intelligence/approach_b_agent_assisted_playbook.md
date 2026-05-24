# Customer Emotion Intelligence: Approach B Agent-Assisted Playbook

Date: `2026-05-24`

Approach B means using an AI agent to convert sparse inputs into a structured emotional brief. Because historical customer data is limited, the agent must work from photos, founder memory, and new inquiry notes, while clearly separating facts from assumptions.

## 1. Ways To Achieve It

| Strategy layer | What to achieve | Agent-assisted method | Human role |
|---|---|---|---|
| Business Strategy | Decide which emotional jobs Krafted wants to own | Agent clusters reconstructed orders by occasion, relationship, desired feeling | Founder approves target emotions and rejects weak categories |
| Operations Strategy | Capture useful emotional data before proposal | Agent extracts brief fields and missing questions from inquiry notes or photo descriptions | Founder validates emotional interpretation |
| Marketing Strategy | Turn emotions into stories customers understand | Agent drafts brief-to-gift story from reconstructed order | Founder approves story accuracy and privacy |
| Digital Strategy | Capture emotional fields in future inquiries | Agent recommends form questions based on repeated missing data | Founder chooses final form language |
| Agent Automation Strategy | Make emotional interpretation repeatable | Agent uses standard output schema with confidence and assumptions | Founder reviews corrections weekly |

## 2. Data Constraint Handling

Since there is no 10-year structured customer database, use this data hierarchy:

| Priority | Source | How to use | Risk |
|---:|---|---|---|
| 1 | Existing hamper/workshop photos | Describe visible items, colors, packaging, handmade elements | Does not reveal emotional intent by itself |
| 2 | Founder memory | Add occasion, relationship, why the customer ordered, what worked | Memory may be incomplete |
| 3 | Captions or old posts | Extract public story, date, product context | May be marketing-led, not full brief |
| 4 | Customer reactions/testimonials if available | Capture exact customer value language | Sparse or unavailable |
| 5 | New inquiries going forward | Capture complete structured brief prospectively | Takes time to build volume |

Rule: if the source is photo-only, mark desired feeling as `inferred`, not fact.

## 3. Required Analysis Workflow

### Step 1: Build A Reconstructed Order Set

Create `20-30` anonymized records from available photos and founder memory.

Minimum viable record:

| Field | Required? | Source |
|---|---|---|
| Record ID | Yes | Create |
| Photo reference | Yes | Existing photo filename or folder |
| Occasion | Yes if known | Founder memory / caption |
| Buyer-recipient relationship | Yes if known | Founder memory |
| Visible gift elements | Yes | Photo |
| Handmade element | Yes if visible | Photo/founder memory |
| Sourced element | Yes if visible | Photo/founder memory |
| Intended feeling | Best effort | Founder memory or inference |
| Customer reaction | Optional | Founder memory/testimonial |
| What made it hard | Optional | Founder memory |
| Confidence score | Yes | Agent + founder |

### Step 2: Ask Agent To Extract Emotional Pattern

Prompt:

```text
You are the Customer Emotion Intelligence Agent for Krafted For You.

Analyze the reconstructed order records below.

Separate facts from assumptions.
Do not invent customer data.

For each record, extract:
- occasion,
- buyer-recipient relationship,
- visible gift elements,
- likely emotional job,
- recipient archetype if inferable,
- personalization clues,
- missing information,
- confidence score.

Then summarize recurring patterns:
- top occasions,
- top relationship types,
- top desired feelings,
- recurring personalization clues,
- common gaps in the data,
- questions Krafted should ask in future inquiries.
```

### Step 3: Founder Review

Founder reviews:

- wrong emotional reads,
- missing emotional nuance,
- overconfident assumptions,
- archetypes that feel off-brand,
- questions that would feel awkward to ask customers.

### Step 4: Create Version 1 Emotion System

Output:

- top 5 occasions,
- top 5 recipient archetypes,
- top 8 desired feelings,
- top 10 future inquiry questions,
- emotional brief template.

### Step 5: Use Prospectively

For every new serious inquiry, use the brief template and track:

- fields captured,
- assumptions,
- founder corrections,
- customer response,
- option proposal outcome.

## 4. Required Analysis Template

Use [required_analysis_template.csv](required_analysis_template.csv).

## 5. Progress And Feedback Loop

Weekly:

- count reconstructed records completed,
- count new inquiries captured,
- review founder corrections,
- remove confusing fields,
- add missing prompts.

Monthly:

- update recipient archetypes,
- update occasion emotion map,
- update agent prompt,
- compare conversion and proposal clarity.

## 6. Success Metrics

| Metric | First-month target |
|---|---:|
| Reconstructed records created | 20 |
| Records with confidence score | 100% |
| New serious inquiries using brief | 80% |
| Agent emotional reads accepted with minor edits | 60% |
| Future inquiry questions reduced to essentials | 8-10 questions |

