---
name: milestone-roadmap-builder
description: Build a lightweight milestone roadmap (Objective/Why/What/When) instead of a Gantt roadmap, per Hexa's 10x Method. Use for product planning or roadmap requests.
---

# Milestone Roadmap Builder

Source: *The 10x Method* (Hexa), Chapter IV — "Building the MVP", pages 81-82.

## Why this approach (per the book)

> "At Hexa, we believe in momentum over meticulous planning... Forget the Gantt charts, the multi-quarter planning, and the overly detailed feature breakdowns."

> "Forget perfect plans, momentum is your greatest asset. In startups, progress comes from shipping fast, not mapping everything out. Because for every 10 features you launch, only one might stick." — Seraphie de Tracy, CEO & Cofounder of Cohort

The roadmap should be a simple table, reviewed and reset quarterly — never planning more than one quarter ahead.

## The template (verbatim structure from the book)

| Objective | Why it's a priority | Key things to build | When |
|---|---|---|---|
| What are we aiming to achieve? Should be a clear, concise goal related to the product's next step. | Why is this important now? Explain how achieving this objective moves the product forward and aligns with the broader vision. | What needs to be built to achieve this goal? Could be features, backend improvements, or integrations. | Timeframe defined at the quarterly review — should never be more than a quarter away. |

### Worked example from the book (internal Hexa project "LegalX")

| Objective | Why it's a priority | What to achieve | When we plan to achieve it |
|---|---|---|---|
| Private ChatGPT for Lawyers | Start collecting first conversations. Deliver ChatGPT value in a private environment for lawyers. Cover rephrase, summarize, and translate use cases. | Private storage; ChatGPT-like threads & interactions | 1 month |
| Leverage mailbox | Leverage context data in the chat. Display objects in chat with hyperlinks. | Connect Outlook; sync & store data; trigger from mailbox to increase usage | 1.5 months |
| Organise internal data | Organise data per customer & users; structure knowledge (customers, matters). | Label documents; consolidate templates of typical documents; right management & search | 2 months |

## Workflow

1. **Get the founder's current planning state** — a feature list, a rough roadmap, or just their long-term vision if they're starting from scratch.
2. **Build 2-4 objectives max for the current quarter** — resist the urge to list everything; if there are more than 4 candidate objectives, ask the founder to prioritize which ones actually move the needle this quarter.
3. **Fill in "why it's a priority" honestly** — this should tie explicitly back to the long-term vision, not just be a restated objective.
4. **Break "key things to build" into concrete, buildable items** — features, backend work, integrations — not vague workstreams.
5. **Cap "when" at one quarter out.** If something feels like it needs longer, either it's too big for one objective (split it) or it belongs in a future quarter's table, not this one.
6. **Pair with product rituals** — mention the weekly product committee cadence (see the book's "Product rituals" section, same chapter) as the mechanism that keeps this roadmap honest week to week; offer to help set that up too (see `product-rituals-setup`, a Solid-tier skill from the same chapter, if available).

## Output format

Produce the roadmap as a markdown table with exactly the 4 columns above, populated with the founder's real objectives — not a generic template with placeholders.
