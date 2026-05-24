# Curated Option Architecture: Approach B Agent-Assisted Playbook

Date: `2026-05-24`

Approach B means using an AI agent to draft 2-3 option paths from a structured brief. The agent should not invent availability, final prices, or delivery promises.

## 1. Ways To Achieve It

| Strategy layer | What to achieve | Agent-assisted method | Human role |
|---|---|---|---|
| Business Strategy | Keep option paths aligned to premium positioning | Agent checks options against offer lane and refusal rules | Founder approves what fits the brand |
| Operations Strategy | Make options feasible and bounded | Agent marks sourcing, handmade, timeline, and complexity assumptions | Founder validates feasibility |
| Marketing Strategy | Make options easy to understand and story-led | Agent names each option by emotional intent and use case | Founder adjusts tone and sophistication |
| Digital Strategy | Use option examples to educate future customers | Agent converts past proposals into anonymized examples | Founder approves examples and privacy |
| Agent Automation Strategy | Draft options consistently | Agent uses a fixed schema and confidence fields | Founder rates and corrects outputs |

## 2. Required Inputs

The agent needs:

- completed emotional brief,
- offer lane,
- occasion,
- recipient profile,
- desired feeling,
- budget band if known,
- needed-by date,
- available handmade formats,
- known sourced product categories,
- customization limits,
- refusal rules.

If any of these are missing, the agent must say what is missing instead of drafting overconfident options.

## 3. Required Analysis Workflow

### Step 1: Reconstruct Past Gift Structures

Using photos and founder memory, create records of past gift structures.

For each photo/order, identify:

- occasion,
- visible contents,
- handmade element,
- sourced items,
- packaging style,
- likely budget band if known,
- complexity level,
- what made it visually strong,
- what could become repeatable,
- what should not be repeated.

### Step 2: Cluster Into Option Patterns

Ask the agent to cluster reconstructed records into patterns:

```text
You are the Curated Option Architecture Agent for Krafted For You.

Analyze the reconstructed gift records.

Do not invent prices or availability.

Cluster the records into reusable option patterns by:
- occasion,
- emotional intent,
- recipient type,
- handmade element,
- sourced element,
- complexity,
- visual style.

For each cluster, propose:
- option path name,
- best-fit occasion,
- customer problem solved,
- typical inclusions,
- personalization levers,
- budget band placeholder,
- lead-time risk,
- what should remain flexible,
- what should be standardized.
```

### Step 3: Founder Review

Founder marks:

- premium enough / not premium enough,
- feasible / risky,
- repeatable / one-off,
- brand-fit / off-brand,
- likely margin issue,
- needs better sourcing.

### Step 4: Create First Playbooks

Build:

- birthday playbook,
- anniversary playbook,
- farewell/gratitude playbook.

Each playbook should have 3 option paths:

1. safe refined choice,
2. most personal choice,
3. premium statement choice.

### Step 5: Test On New Inquiries

For every new qualified lead:

- generate 2-3 options,
- founder edits,
- proposal sent,
- track selected option or rejection reason.

## 4. Required Analysis Template

Use [required_analysis_template.csv](required_analysis_template.csv).

## 5. Progress And Feedback Loop

Weekly:

- count proposals using option paths,
- track selected option,
- track customer confusion,
- log founder edits,
- identify repeated patterns.

Monthly:

- retire weak options,
- rename confusing options,
- update budget and lead-time assumptions,
- add new playbook only if repeated demand appears.

## 6. Success Metrics

| Metric | First-month target |
|---|---:|
| Reconstructed gift structures analyzed | 20 |
| Reusable option clusters created | 5 |
| Occasion playbooks created | 3 |
| Qualified leads receiving options | 80% |
| Proposals accepted with minor edits | 60% |
| Option selected without full redesign | 60% |

