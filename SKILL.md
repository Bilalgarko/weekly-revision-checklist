---
name: weekly-revision-checklist
description: Helps a university student build a weekly revision checklist shown as a table with topic, priority, time needed and done columns. Use when the student says help me revise, quiz me or make a study plan, or asks to organise their revision for the week. Not for graded homework, assessed coursework, exams or any work submitted for marks.
license: MIT
---

# Weekly Revision Checklist

## When to use this skill

Use this skill when a university student asks to:

- "help me revise"
- "quiz me"
- "make a study plan"
- organise, plan or review their revision for the week

Use it for self-directed revision planning only.

## What to ask the user first

Ask briefly (one short message, not a long form) for anything missing:

1. Course or module name and level (for example second year biology).
2. The topics or lecture weeks to cover this week.
3. Any dates that matter (exam, quiz, or submission dates for other courses).
4. Total hours available for revision this week.
5. Confidence per topic (low, medium, high) or which topics feel hardest.

If the user already supplied this information, do not ask again. If some
items are unknown, proceed with reasonable assumptions and state them.

## Step-by-step process

1. **Confirm scope.** Restate which subjects and topics the week covers.
2. **List the topics.** Break broad topics into revision-sized units (one
   unit is roughly what can be reviewed in 25 to 60 minutes).
3. **Set priority.** Use High, Medium or Low per the scheme in
   [references/REFERENCE.md](references/REFERENCE.md), based on exam dates,
   topic weight and the user's confidence.
4. **Estimate time.** Give a time range per topic using the guidance in
   [references/REFERENCE.md](references/REFERENCE.md).
5. **Order the list.** Highest priority first, with hard deadlines earlier
   in the week.
6. **Render the checklist table** in the output format below.
7. **Offer next steps.** Ask whether the user wants to be quizzed on any
   topic, keeping the do-not rules below in mind.

## Output format

Always output the checklist as a Markdown table with exactly these columns:

| Topic | Priority | Time needed | Done? |
| --- | --- | --- | --- |
| Week 3 - Cell respiration | High | 50 min | [ ] |
| Week 4 - Photosynthesis | Medium | 40 min | [ ] |

Rules for the table:

- One row per revision unit.
- Priority is exactly High, Medium or Low.
- Time needed is a duration such as 25 min or 1 h 10 min, and may be a
  range like 40-50 min.
- Done? starts as [ ] and the user changes it to [x] when finished.
- Follow the table with the estimated total time for the week.

## Do not

- Do not do graded homework, assessed coursework, take-home exams or any
  work the user will submit for marks.
- Do not write essays, lab reports, problem solutions, proofs or code that
  counts towards a grade.
- Do not accept a request to "revise" that is really a request to produce
  assessed work. If the request is assessed work, say so politely, decline
  that part, and offer revision help instead (for example explaining a
  concept, or a practice quiz with answers withheld until the user tries).
- Do not invent course facts. If the user's syllabus, exam date or topic
  list is unknown, ask or clearly mark assumptions.
- Do not fabricate mark schemes or official answer keys.

## Files

- [references/REFERENCE.md](references/REFERENCE.md) - priority scheme,
  time estimation guidance, a full example checklist and edge cases.
