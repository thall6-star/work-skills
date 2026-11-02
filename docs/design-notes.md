# Design notes: why v3 is built this way

v3 is a separate agent built from what v1 and v2 taught us. It puts every rule that must be exact where the agent always reads it, turns judgment calls into fixed rules, and is tested against a known-good sample before anyone uses it.

## If I did this again

1. **List the platform limits before writing anything.** Each limit decides where a rule lives:

   | Limit we hit | Design consequence in v3 |
   |---|---|
   | Instructions box caps at 8,000 characters | Instructions stay short (about 4,900 characters); stage rules live in skills |
   | Knowledge files are searched, not read in full | Anything that must be exact lives in a skill or the instructions: call sheet questions, bullet rules, CFO reread. Only the K-12 Finance Lens stays as knowledge |
   | Suggested prompts drop line breaks and send only the message | Prompts are one line; the skill sends the intake form |
   | Web search cannot open JavaScript sites like BoardDocs; LinkedIn is blocked | Research comes from budget books and district pages; reps attach the budget book and check LinkedIn |
   | Outlook, Teams and connectors are off | Reps bring transcripts and {{VENDOR}} Products from Salesforce |
   | The agent cannot see page breaks | Each section has its own limit and a cut order; no total word caps |

2. **Define each document by its reader and the decision it supports**, then build one known-good example before writing rules. Rules are written to reproduce the example.
3. **Turn every judgment into a rule with fixed outcomes.** Examples: the Timing Read month rule, three MEDDPICC statuses, "Likely:" on every inference, and "leave it out" when there is no evidence.
4. **Build the test set before the first prompt**, including districts with thin data and common names.
5. **Build and test one stage at a time**: Discovery Prep first, then Demo Prep, then Demo Debrief.
6. **Keep one source of truth.** Change this repo first, version it, and paste whole blocks into Agent Builder.
7. **Freeze, then pilot.** No changes during the pilot; collect what reps skip and what they question.

## How v3 works

| Stage | Rep runs it | Rep brings | Agent produces |
|---|---|---|---|
| Discovery Prep | Before discovery | Intake form; budget book if they have it; {{VENDOR}} Products from Salesforce | Discovery Brief: rep summary, call sheet Q1 to Q9, SE layer |
| Demo Prep | Right after discovery | Discovery Brief, Teams transcript, notes | Demo Prep: MEDDPICC table, SE Request, demo plan, SE appendix |
| Demo Debrief | After the demo | Demo Prep document, demo transcript | Demo Debrief: demo notes, MEDDPICC changes, tasks by role |

## What changed from v2

| Area | v2 | v3 |
|---|---|---|
| Call sheet questions | Pulled from the Discovery Guide knowledge file | Built into the discovery-prep skill, Q1 to Q9, word for word |
| Research and bullet rules | In the Discovery Research Method knowledge file | Built into the discovery-prep skill |
| CFO reread | Checklist inside the Lens knowledge file | Five questions in the agent instructions, applied every time |
| Knowledge files | Three | One: K-12 Finance Lens v1 |
| Timing Read | Needed proof that next year's budget work had not started, so it was often blank | Month rule: months 1 to 3 Current-year funds, 4 to 6 Either, 7 to 12 Next-year request; a published calendar overrides |
| Strategic Direction status | Current, Expired, In development | Adds Undated, for board goals with no years |
| Vendor and product clues | Not captured | New SE Layer item, Clues to Confirm, labeled as clues |
| MEDDPICC | Paragraphs | A table: Component, Status, Evidence, Next question |
| Demo Prep topic table | One row per Discovery Guide topic (file-dependent) | Discovery Answers: one row per Q1 to Q9 |

**What did not change:** stage names, document names, page budgets of 3, 4 and 3 pages, the intake form, Who We're Meeting, and the Demo Debrief sections.
