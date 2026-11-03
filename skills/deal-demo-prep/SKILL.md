---
name: deal-demo-prep
description: Invoke after a discovery call when a discovery transcript is attached, or when a seller requests Demo Prep, a discovery debrief, MEDDPICC updates, the SE Request description, or demo preparation. Creates the Demo Prep Word document.
---

## Purpose
After the discovery call, create the Demo Prep document: it updates Salesforce, gives the SE what is needed to accept the request and prepare the demo, and becomes the current record of the opportunity. Report what the district said. Do not describe {{PRODUCT}} capabilities.

## Inputs
- **Required:** the discovery transcript, attached. If it is missing, ask for it and stop. Do not search for meetings.
- **Recommended:** the Discovery Brief, attached. Use its header, District Facts, slide bullets, Budget Timing, and Who We're Meeting.
- **Optional:** rep notes in the message or as a file.
- Do not perform web research in this stage.

## How to Read the Transcript
1. For each call sheet question below, capture what was said, who said it, and a status: Answered, Partly, or Not asked. Use the answer wherever it was said in the call, not only where the question was asked.
   - Q1 Improvement goals
   - Q2 ERP and hosting
   - Q3 Budget development approach
   - Q4 Department participation
   - Q5 School and principal involvement
   - Q6 Budget monitoring access
   - Q7 School allocation method
   - Q8 Allocation people and tools
   - Q9 Budget timing and funding
2. Treat a system or practice as a fact, not a pain. Call something a pain only when the district described it as a problem or something to change.
3. Use `K-12 Finance Lens v1` to interpret budgeting terms. Do not add facts from it.
4. Rep notes add context but never override the transcript. If they conflict, follow the transcript and note the conflict under Corrections to Discovery Brief.

## Document
- Create a Word document named `<District>_<ST>_2_Demo Prep.docx`. 4 pages maximum. Cut detail before adding length.

### Section 1: Header
- Title: `<District full name> Demo Prep`.
- One table: District | Discovery Date | District attendees on the call (name, title) | Our attendees.

### Section 2: Salesforce Updates
- Start with the exact line: `Copy these into Salesforce.`
- **MEDDPICC** as a table: Component | Status | Evidence | Next question. One row per component in this order: Metrics, Economic Buyer, Decision Criteria, Decision Process, Paper Process, Identify Pain, Champion, Competition. Status is Confirmed, Partial, or Gap. Evidence is 1 to 2 sentences with names, titles, dates, and numbers from the call. Next question is one question, only when the status is Partial or Gap.
- Put information under the component it fits:
  - **Metrics:** outcomes the district wants measured, in its own numbers: positions over or under enrollment need, weeks spent on the budget cycle, grant funds lapsed, time to produce the budget book, share of spend tied to strategic plan goals. Enrollment, school count, and budget totals are context, not Metrics.
  - **Economic Buyer:** the person who approves the spend and controls the budget line, usually the CFO, Assistant Superintendent for Business, or Business Manager. Name someone only if the district identified them. The most senior attendee is not the Economic Buyer unless the district said so. Note whether board approval is required.
  - **Decision Criteria:** what the district said it will judge on, such as integration with its named ERP, ease of use for principals and budget managers, position control, grants, budget book, data security, peer references.
  - **Decision Process:** the steps and people from evaluation to a decision: who evaluates, demos, reference calls, cabinet review, target decision date.
  - **Paper Process:** how it gets bought: quote or RFP thresholds, cooperative contract, legal or data privacy review, board meeting date, which fiscal year the money comes from.
  - **Identify Pain:** problems the district described as problems, who said it, and the cost or consequence if stated. A system or practice alone is not pain.
  - **Champion:** a district person who wants the change, has access to the Economic Buyer, and has acted for the deal (shared data, set a meeting, brought in others). Interest alone is "Possible champion" plus what would confirm it.
  - **Competition:** other vendors, the ERP's own budgeting module, spreadsheets and the current process, or waiting a year. Name only what the district mentioned or showed.
- Economic Buyer and Paper Process are often Gap after one discovery call. That is expected. Give the next question.
- **SE Request Description**, about 450 words, in these labeled parts:
  - **District Snapshot:** 2 sentences.
  - **Current Systems and Process:** 3 sentences covering ERP, budget method, and tools.
  - **Primary Pain Points:** 3 to 4 bullets, one sentence each, naming who raised it.
  - **Who Is Impacted:** 2 sentences.
  - **Desired Outcomes:** 2 to 3 bullets, one sentence each.
  - **Timeline and Decision Process:** 2 sentences. Include where the district is in its budget cycle and how it would fund the purchase, from Q9 first and the Discovery Brief's Budget Timing second.
  - **Open Questions for the SE:** 3 to 5 bullets, one line each.

### Section 3: Demo Plan
- Start on a new page.
- **What We Understand**: the 3 slide bullets from the Discovery Brief, updated where the call corrected them. Add "(updated)" after a changed bullet.
- **What We Heard**: 3 to 4 slide-ready bullets in the district's own terms, each 8 to 18 words.
- **How We Can Help**: the exact line `SE to complete.` then a table with up to 4 rows: Pain | Who raised it | How it shows up today | Desired outcome | {{PRODUCT}} capability. Leave the {{PRODUCT}} capability cell blank.
- **Demo Focus**: rank {{MODULE_1}}, {{MODULE_2}}, and {{MODULE_3}} for this district, with one sentence of evidence each.
- **Gaps to Close Before Demo**: 3 to 5 gaps, each with one question.
- **Prep Call Agenda**: 4 to 6 items for the SE, seller, and AM.
- **Follow-Up Email Draft**: under 120 words, from the seller: thanks, 2 to 3 things we heard, and the agreed next step and date if stated. No product claims.

### Section 4: SE Appendix
- Start on a new page.
- **Discovery Answers** table: Question | What we learned (15 words or fewer) | Status | Speaker. One row for each of Q1 to Q9.
- **Stakeholder Map** table: Name | Title | Background | What they care about | Likely role in the decision. Take Background from Attendee Backgrounds in the Discovery Brief, or write "Not researched". "What they care about" comes only from the call.
- **Corrections to Discovery Brief**: bullets, or "None".
- **Risks to Watch**: up to 3.
- **Key Statements**: up to 5 short paraphrases with the speaker.

## Final Check
- Every claim traces to the transcript, the Discovery Brief, or rep notes.
- The MEDDPICC table has all 8 rows, and every status is supported by evidence.
- Every SE Request part is within its limit.
- Discovery Answers has a row for each of Q1 to Q9.
- What We Understand and What We Heard pass the CFO Reread.
- No {{PRODUCT}} capabilities are described.
