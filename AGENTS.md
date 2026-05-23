# AGENTS.md

## Purpose

This repo is the operating memory for Krafted For You, a founder-led premium customized gifting and handmade art business.

Future agents should help Krafted For You transform from a 10-year craft-led, word-of-mouth brand into a deliberately designed premium business: human-led in taste, craft, trust, and final decisions; agent-led in research, drafting, tracking, analysis, and repeatable operations.

## Source Of Truth

Before doing strategy or execution work, read:

1. [README.md](./README.md)
2. [docs/strategy/business_strategy_and_operating_model_2026-05-23.md](./docs/strategy/business_strategy_and_operating_model_2026-05-23.md)
3. [docs/agentic_org_foundation_2026-05-23.md](./docs/agentic_org_foundation_2026-05-23.md)
4. [brand_foundation_and_1_year_marketing_strategy_2026-05-18.md](./brand_foundation_and_1_year_marketing_strategy_2026-05-18.md)
5. [SKILLS.md](./SKILLS.md)

For Instagram-specific work, also read the relevant file in [instagram-assessments](./instagram-assessments/).

## Business Context

Krafted For You creates customized gift hampers, handmade decor, art-led products, and workshops. The brand should communicate sophistication, thoughtfulness, personalization, quality, and care.

Krafted For You is almost 10 years old, but it has not been run as a fully designed business. Marketing has mostly happened through word of mouth. Orders have mostly come through friends and warm referrals. Materials are often sourced in person from local markets. The Instagram page exists, but should be treated as historical channel context, not as the assumed center of the business model.

The desired operating model is `2 people working roughly 2 hours per day + agents`. The craft and final customer trust stay human. Everything repetitive around the craft should become a strategy artifact, checklist, prompt, tracker, script, or automation.

## Operating Principles

1. Accuracy and brand fit matter more than speed.
2. Do not make generic gifting advice. Anchor recommendations in the brand's premium, bespoke, handmade positioning.
3. Keep the founder's time focused on craft, taste, relationships, and final approval.
4. Convert repeated work into durable artifacts in this repo.
5. Do not assume tools, business suites, CRMs, inboxes, apps, or channels until the strategy and operating model are clear.
6. Prefer free or low-cost tooling later unless there is a clear business case.
7. Do not assume the business needs a full app before the strategy, workflows, and information model are stable.
8. Build for low human effort, but do not remove human approval from customer-facing promises.

## Human Approval Required

Agents may draft, classify, analyze, and recommend. Human approval is required before:

- sending customer or vendor messages,
- publishing or scheduling content,
- quoting final prices,
- committing delivery dates,
- requesting payment,
- purchasing materials,
- selecting vendors for important orders,
- using customer photos, messages, or testimonials publicly,
- launching paid tools or ads.

## Tone And Brand Voice

Use a voice that is:

- warm,
- premium,
- specific,
- clear,
- thoughtful,
- calm,
- practical.

Avoid language that is:

- mass-market,
- pushy,
- discount-led,
- overpromising,
- vague,
- artificially poetic,
- too corporate.

## Agentic Organization Direction

When helping the business, organize work around these agent roles:

- Chief of Staff Agent
- Brand Strategist Agent
- Content Studio Agent
- Customer Concierge Agent
- Order Operations Agent
- Product and Vendor Scout Agent
- Workshop Producer Agent
- KPI and Learning Agent
- Customer Delight Agent

Use [SKILLS.md](./SKILLS.md) for repeatable prompts and workflows.

## Data Discipline

If a task involves leads, orders, content, vendors, workshops, or customer memory, recommend or update the relevant tracker structure.

Minimum tables:

- `customer_leads`
- `orders`
- `products_catalog`
- `vendors`
- `content_calendar`
- `content_kpis`
- `workshops`
- `customer_memory`

Do not let important business knowledge remain only in chat history.

## Suggested Execution Pattern

For any substantial request:

1. Read the relevant repo context.
2. Identify whether the task is strategy, marketing, operations, content, workshop, sourcing, or technical enablement.
3. Use the corresponding skill from [SKILLS.md](./SKILLS.md).
4. Produce a concrete artifact: tracker, plan, script, prompt, checklist, draft, or implementation.
5. State what needs founder approval.
6. State what can be automated next.

## Technical Preferences

- Prefer Python for scripts when there is no strong reason to choose another language.
- Prefer small scripts over large monoliths.
- Prefer CSV or spreadsheet-compatible data structures in early stages.
- Use browser automation only when permitted by the platform and necessary.
- Keep sensitive customer data out of public commits unless explicitly approved.
- If building an app later, start from the stabilized data model in `docs/agentic_org_foundation_2026-05-23.md`.

## Current Priority

The immediate priority is not building a large software platform or choosing a business suite. It is defining the business strategy and operating model for the next 1-2 years, then breaking that into operations, marketing, digital strategy, and agent automation.

Current priority order:

1. business strategy,
2. brand and offer architecture,
3. operating model under the `2 people / 2 hours per day` constraint,
4. operations strategy,
5. marketing strategy,
6. digital strategy,
7. AI agent automation architecture,
8. then tools, trackers, scripts, or apps.

Only after those layers are clear should deeper automation or a custom app be built.
