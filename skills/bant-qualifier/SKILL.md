---
name: bant-qualifier
description: Qualify a sales or design-partner call using BANT (Budget, Authority, Need, Timing) per Hexa's 10x Method, with a next-step recommendation. Use after a discovery call.
---

# BANT Qualifier

Source: *The 10x Method* (Hexa), Chapter VI — "Acquiring the Very First Customers", page 149.

## Context (per the book)

A Design Partner Program isn't just feedback collection — it's your first sales motion, even if the MVP is rough. The book recommends structuring first calls as 15 minutes discovery + 15 minutes on the DP deck, then qualifying with BANT.

## The BANT framework (verbatim)

- **Budget**: Do they have the budget or flexibility to pay?
- **Authority**: Are you speaking to the decision maker?
- **Need**: Is the problem clearly defined and urgent?
- **Timing**: Can they start using it within a reasonable timeframe?

## The next-step logic (verbatim from the book)

Every call should end with a clear determination of where the lead stands:
- **Not a fit** → Close the loop and move on. (It's okay to say no to a prospect — don't dilute your positioning by accepting every edge case.)
- **Not now** → Add to your nurture list and check in later.
- **Qualified** → Send an offer (an actual offer, not a pitch deck).
- **Second call needed** → Only if you need other teams (product, dev, ops) to assess feasibility or finalize with the real decision maker.

If the lead isn't a fit, it's fine to cut the call short — respect your time and theirs. If they're not the decision-maker but show real interest, set up a second call with the right stakeholders.

## Workflow

1. **Get the call details** from the founder: what was discussed, who they spoke with, what was said about budget, urgency, decision authority, and desired timeline.
2. **Score each of the 4 BANT dimensions** explicitly: clear yes / unclear / clear no, with the specific detail from the call that supports the score.
3. **Apply the next-step logic** from the table above based on the combined BANT read — don't just average the 4 scores; a hard "no" on Authority with everything else strong points to "second call needed," not "qualified."
4. **Give the recommendation directly**: Not a fit / Not now / Qualified — send an offer / Second call needed — and say who should be looped in if a second call is warranted.
5. **If qualified**, remind the founder to move fast: send an actual offer with a validity date, not another deck (this pairs well with the `design-partner-deck-builder` skill for building that offer/deck).

## Output format

1. **BANT scorecard**: 4 rows (Budget/Authority/Need/Timing), each with a status and the evidence from the call
2. **Next-step recommendation**: one of the 4 categories, stated directly
3. **Immediate action**: what the founder should do in the next 48 hours
