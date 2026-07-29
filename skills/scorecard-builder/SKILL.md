---
name: scorecard-builder
description: Build a hiring scorecard (criteria, priority, skill type, question) per Hexa's 10x Method, capped at 12 criteria. Use when preparing candidate interviews.
---

# Scorecard Builder

Source: *The 10x Method* (Hexa), Chapter V — "Hiring and Retaining Early Talent", pages 123-125.

Full worked example (Founding Engineer scorecard) and the book's exact rules: see `references/scorecard-example.md` — read it before building a new scorecard, and use its structure as the template to follow.

## Why this matters (per the book)

Most founders aren't experienced recruiters, which makes them especially vulnerable to bias — overvaluing charisma, shared background, or someone who "just feels right." A scorecard is a structured framework to evaluate candidates on defined criteria instead of gut feeling, and it makes rejection easier: objective reasons instead of debating feelings.

## The rules

- Categorize each criterion as **Must Have / Should Have / Nice to Have**.
- Cover both **hard skills** and **soft skills** — plus behaviors/mindset where relevant (e.g. "entrepreneurial mindset").
- **Cap at 12 criteria total** — more makes the process too complex.
- Every criterion needs a **key question to ask** — the same question, asked identically to every candidate, so comparisons are reliable.
- Each criterion should trace back to an actual mission from the job description (pair with `job-description-builder` output when available).

## Workflow

1. **Get the role context**: job title, the 2-4 core missions (ideally from an existing JD), and any must-have technical requirements.
2. **Draft 8-12 criteria**, mixing hard skills, soft skills, and behaviors — don't over-index on technical skills alone; the worked example includes problem-solving, "gets things done," team player, and entrepreneurial mindset as explicit criteria.
3. **Assign priority** (Must/Should/Nice to Have) to each — be disciplined; if everything is "Must Have," the prioritization is meaningless.
4. **Write expectations** for each criterion — what "good" concretely looks like, not a vague label.
5. **Write one key interview question per criterion**, phrased to elicit a specific story or example (behavioral, "tell me about a time...", "walk me through...") rather than a yes/no answer.
6. **Check the count**: if above 12 criteria, cut down — ask which ones are truly non-negotiable for this specific role at this specific stage.

## Output format

A markdown table with exactly these columns: **Criteria | Priority | Skill Type | Expectations | Key question to ask** — following the structure of the worked example in the reference file.
