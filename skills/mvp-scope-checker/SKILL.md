---
name: mvp-scope-checker
description: Check whether an MVP plan is correctly scoped against Hexa's 10x Method 5-point checklist, and flag overbuilding. Use whenever a founder describes their MVP plan, feature list, or asks "is this too much for a first version?", "am I overbuilding?", or "what should I cut from my MVP?".
---

# MVP Scope Checker

Source: *The 10x Method* (Hexa), Chapter IV — "Building the MVP", page 80. This is the book's own verbatim checklist.

## The checklist (verbatim from the book)

Your MVP plan should pass **all five** of these:

1. **Aligns with your long-term vision** — it should be a stepping stone toward your ultimate goal, not a random experiment.
2. **Can be developed in weeks, not months** — if it takes too long, you're over-building.
3. **Is a real product and not a polished prototype** — the only way to get meaningful insights.
4. **Delivers enough value to onboard real users** — even in its simplest form, it must solve a real problem.
5. **Is minimal enough to allow for quick iteration** — no unnecessary complexity that slows future changes.

> "If your MVP plan doesn't check all these, you're overbuilding." — *The 10x Method*

## Workflow

1. **Get the MVP plan or feature list** from the founder — the more specific (feature by feature), the better the check.
2. **Score each of the 5 criteria** as ✅ Pass / ⚠️ Borderline / 🔴 Fail, with a one-line reason tied to what they described (not generic advice).
3. **For each 🔴 or ⚠️, propose a concrete cut or simplification** — the book's "hammer allegory" point is that founders often build a whole toolbox when the user only needed a hammer; be specific about which features to defer, not just "simplify."
4. **Sanity-check the "weeks not months" criterion literally** — ask (or estimate from what's described) how long the plan would actually take to ship, and compare explicitly against a multi-week target.
5. **Close with a clear verdict**: does this MVP plan pass the checklist as-is, or does it need to be cut down first? Don't hedge — the book's own framing is binary (passes all 5, or it's overbuilding).

## Output format

| Criterion | Status | Why |
|---|---|---|
| Aligns with long-term vision | ✅/⚠️/🔴 | ... |
| Weeks not months | ✅/⚠️/🔴 | ... |
| Real product, not polished prototype | ✅/⚠️/🔴 | ... |
| Delivers enough value to onboard real users | ✅/⚠️/🔴 | ... |
| Minimal enough for quick iteration | ✅/⚠️/🔴 | ... |

Followed by:
- **Specific cuts to make** (if any criterion isn't a clean pass)
- **Verdict**: Ready to build / Needs trimming first

If the founder wants to go further on planning after this, point them to the `milestone-roadmap-builder` skill for the next step (turning the trimmed MVP into a milestone plan).
