# Setup: how to use these skills

This repo contains **Claude Agent Skills** (`SKILL.md` format) built from
*The 10x Method* by Hexa. Each skill teaches Claude one specific framework
from the book so you can apply it to your own startup. This guide explains
how to install and trigger them, whether you use **Claude Code** (CLI, VS
Code, web) or **claude.ai**.

## 1. Where to put the skills

Each `skills/<skill-name>/` folder (its `SKILL.md` and, for some skills, a
`references/` subfolder) must be copied into a `skills/` folder that Claude
recognises. Pick one of three options:

**Option A: one project (recommended to start)**

Copy the skills you want into `.claude/skills/` at the root of your
project's repo:

```bash
mkdir -p /path/to/your-project/.claude/skills
cp -r skills/idea-categorizer /path/to/your-project/.claude/skills/
cp -r skills/mvp-scope-checker /path/to/your-project/.claude/skills/
# ...repeat for each skill you want, or copy them all:
cp -r skills/* /path/to/your-project/.claude/skills/
```

They will only be available in Claude Code sessions opened on that project.

**Option B: all your projects**

Copy them into your global user folder so they're available in every
Claude Code session:

```bash
mkdir -p ~/.claude/skills
cp -r skills/* ~/.claude/skills/
```

**Option C: claude.ai (web and desktop app)**

Zip each `skills/<skill-name>/` folder you want, then upload it in the
Skills section of your claude.ai settings. The content and format
(`SKILL.md` + `references/`) are exactly the same.

## 2. How skills get triggered

You don't need to "launch" a skill manually. Claude reads the
`description` field of each `SKILL.md` and picks the right skill on its
own when your request matches.

Examples of prompts that trigger a skill automatically:
- *"I have a fintech startup idea, what do you think?"* → `idea-categorizer`
- *"Here's my MVP plan, am I overbuilding?"* → `mvp-scope-checker`
- *"Help me write the job description for my first engineer"* → `job-description-builder`
- *"I'm preparing my pitch deck for our seed round"* → `pitch-deck-structure-builder`

You can also be explicit: *"Use the scorecard-builder skill to prepare my
interviews"*.

If a skill doesn't trigger as expected, check that:
1. the folder was copied to one of the locations above,
2. the folder name matches the `name:` field in the frontmatter,
3. you opened a **new session** after copying (skills load when a session
   starts).

## 3. Which skills to use when

The skills follow the book's progression. That's useful if you're building
a startup from scratch, but every skill also works on its own.

| Stage | Skills | Chapter |
|---|---|---|
| 1. Become a 10x founder | `mindset-diagnostic`, `weekly-momentum-email-builder` | Ch. I |
| 2. Find and validate the idea | `idea-categorizer`, `idea-validation-roadmap-builder` | Ch. II |
| 3. Choose your cofounder | `cofounder-self-assessment`, `cofounder-alignment-assessor`, `cofounder-process-tracker` | Ch. III |
| 4. Build the MVP | `mvp-scope-checker`, `milestone-roadmap-builder`, `product-rituals-setup`, `pivot-decision-helper` | Ch. IV |
| 5. Hire your first talents | `job-description-builder`, `scorecard-builder`, `hiring-case-study-designer`, `reference-check-script-builder`, `onboarding-ritual-builder` | Ch. V |
| 6. Land your first customers | `icp-definer-refiner`, `design-partner-deck-builder`, `bant-qualifier`, `dp-offer-pricing-helper`, `gtm-ritual-setup`, `outbound-sequence-builder` | Ch. VI |
| 7. Brand and communications | `brand-foundations-builder`, `brand-voice-finder`, `website-tagline-builder`, `founder-branding-content-planner`, `pr-pitch-angle-builder` | Ch. VII |
| 8. Raise funds | `executive-summary-builder`, `pitch-deck-structure-builder`, `data-room-builder`, `objection-anticipation-prep`, `round-structuring-helper` | Ch. VIII |
| 9. ESG from day one | `esg-checklist` | Ch. IX |

For a chapter's full context (summary, quotes, frameworks that weren't
turned into a skill), see the matching file in `chapter-readmes/`.

## 4. Updating or adding skills

We add new skills to this repo in regular drops (see "Always growing" in
the `README.md`). New skills install the same way. If a skill you already
installed gets updated, copy it again to the location you chose in step 1
and restart your session so the change is picked up.
