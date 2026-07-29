---
name: idea-categorizer
description: Classify a startup idea into Hexa's 3 idea categories (problem-solution fit, market/tech shift, category creation) and get tailored discovery tactics. Use for any rough startup idea.
---

# Idea Categorizer

Source: *The 10x Method* (Hexa), Chapter II — "Finding and Validating the Idea", pages 32-35.

## What this skill does

Takes a founder's raw idea (or the industry/space they want to explore) and:
1. Classifies it into one of Hexa's 3 categories of startup ideas.
2. Explains what has to be true for the idea to hold up in that category.
3. Gives category-specific tactics for finding or sharpening ideas of that type.

## The 3 categories (from the book)

| Category | Problem recognition | Existing solutions? | Solution type | Examples (book) |
|---|---|---|---|---|
| **Cat 1 — Problem-solution fit** | Clearly recognized | No good solutions | New or better way to solve a known pain | Superhuman, Figma (UX angle), first online tax filing |
| **Cat 2 — Market or technology shift** | Clearly recognized | Yes, but outdated | Using new capabilities that didn't exist before | Tandem, Tesla, Notion, ChatGPT for support |
| **Cat 3 — Category creation** | Not widely recognized | No clear solutions | Creates an entirely new way of doing things | Facebook, Airbnb, Uber, Slack |

**Category 1 — Problem-solution fit**
- Source of the idea: personal frustration, industry knowledge, or market insight.
- The problem exists today and is clearly felt by a specific group; existing options are missing, bad, or outdated.
- How to find them: tap into personal frustrations, leverage industry expertise, ask investors/founders what pain points remain unsolved, watch for manual workarounds (people copy-pasting between tools, using Notion/Sheets to hack a solution), critically examine existing tools for gaps.

**Category 2 — Market or technology shift**
- Source: a new technology, market trend, or regulatory change makes an existing, already-recognized problem solvable in a dramatically better, faster, or cheaper way.
- How to find them: become an expert in an emerging technology (AI, web3, green tech...), track regulatory changes (e.g. GDPR created demand for privacy tools), talk to users in legacy industries (law, logistics, finance, healthcare) who know their tools are outdated but don't know what's newly possible, map existing workflows against new capabilities ("how would this work if invented today?"), study recent startup failures to see if the market is now ready.

**Category 3 — Category creation**
- Source: a paradigm shift / behavior change that the market hasn't even recognized as a problem yet ("just the way things are").
- The hardest to find, but the highest potential reward.
- How to find them: study behavior (not just stated problems) — watch for friction people have accepted as normal; explore cultural shifts and generational changes; question assumptions about ownership, work, and standard processes.

## Workflow

1. **Get the raw material.** Ask the founder to describe their idea (or the space/industry they're exploring) in a few sentences. If they only have a vague direction (e.g. "something in fintech for SMBs"), that's enough to start — this skill can also help *find* an idea, not just classify an existing one.
2. **Test against each category's criteria** using the table above:
   - Is the problem already clearly recognized by the target users? → rules toward Cat 1 or 2.
   - Do decent existing solutions already exist? → No good ones = Cat 1. Outdated ones = Cat 2. None = Cat 3.
   - Is there a new technology/trend making something newly possible? → Cat 2.
   - Is the "problem" actually an accepted behavior nobody complains about? → Cat 3.
3. **Assign the category** (be honest if it's ambiguous — some ideas straddle two categories; say so and explain the tension).
4. **Give category-specific next steps**: pull the relevant "how to find them" tactics above and turn them into 3-5 concrete actions the founder can take this week (e.g. for Cat 2: "go interview 5 people in [legacy industry] about how they currently do X").
5. **Flag the risk profile**: Cat 1 ideas are easier to validate but more competitive; Cat 2 ideas need genuine technical/timing edge; Cat 3 ideas are the hardest to validate with normal customer discovery (people won't say they want something they've never conceived of) — mention this explicitly so the founder calibrates their validation approach (see the `idea-validation-roadmap-builder` skill for that next step).

## Output format

Structure the response as:
1. **Category assigned** (with a one-line justification against the 3 criteria)
2. **Why this matters** for how they should approach validation
3. **3-5 concrete next actions**, tailored to the category
4. A short note if the idea has traits of two categories at once

Keep the tone direct and pragmatic — this mirrors Hexa's own operating style, not generic startup-advice fluff.
