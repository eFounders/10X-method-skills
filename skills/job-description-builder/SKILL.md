---
name: job-description-builder
description: Write an early-stage job description in Hexa's 10x Method 7-section structure (title, about, missions, stack, requirements, why join, timeline). Use for any JD request.
---

# Job Description Builder

Source: *The 10x Method* (Hexa), Chapter V — "Hiring and Retaining Early Talent", pages 120-123.

Full writing rules and rationale for each section: see `references/jd-writing-rules.md` — read it before writing, it contains the book's exact guidance and example phrasing for each section.

## What this skill does

Writes a complete, early-stage-appropriate job description in the book's 7-section structure, actively avoiding the two failure modes the book calls out: sounding too "corporate" (copy-pasted from big-company JDs) or too try-hard "cool" (confusing candidates about the actual role).

## The 7 sections

1. Title (searchable, not just cute)
2. About the company (the "why", in one punchy paragraph)
3. What you'll do / missions (core problems owned, not a laundry list; include how the role evolves over 6-9 months)
4. Technical stack (if relevant to the role)
5. Who you are / requirements (3-5 traits max, must-have vs. nice-to-have)
6. Why join (values, ways of working, unique impact — not just perks)
7. Hiring timeline (the 4-step process, or the founder's actual process)

## Workflow

1. **Gather inputs** from the founder: role title, what the company does, the 2-3 core problems this hire will own, technical stack (if relevant), and their actual hiring process steps. If any of this is missing, ask — don't invent company specifics.
2. **Write each section following the rules in the reference file** — pay particular attention to:
   - Keeping the missions section richer than the requirements section (the book flags this as the #1 common imbalance).
   - Capping requirements at 3-5 must-matter traits.
   - Making the "About the company" paragraph punchy and specific, not generic startup boilerplate.
3. **Flag anything under-specified**: if the founder hasn't defined their hiring timeline or technical stack yet, don't fabricate one — note it explicitly as a TODO in the draft.
4. **Offer the pairing skill**: mention that once candidates start coming in, the `scorecard-builder` skill turns this same JD's missions into a structured evaluation scorecard.

## Output format

A complete JD in the 7-section structure, ready to post, with clear section headers matching the book's structure. If inputs were incomplete, end with a short "Before you post this" checklist of gaps to fill.
