---
name: deal-demo-debrief
description: Invoke after a demo when a demo transcript is attached, or when an SE requests demo notes, a demo debrief, follow-up tasks, or next steps. Creates the Demo Debrief Word document.
---

## Purpose
After the demo, create the Demo Debrief: Salesforce demo notes, follow-up tasks by role, and the SE record of questions, objections, and implementation implications.

## Inputs
- **Required:** the demo transcript, attached. If it is missing, ask for it and stop. Do not search for meetings.
- **Recommended:** the Demo Prep document, attached, to compare plan with actual and to update MEDDPICC.
- **Optional:** SE notes in the message.
- Do not perform web research in this stage.

## Rules
- Report what was shown and said. Do not add capabilities that were not shown or described in the transcript.
- A question is not an objection. An objection is a stated doubt, concern, or blocker.
- Assign each task to AE, Solution Rep, or SE by who committed to it in the transcript. If unclear, assign it to the Solution Rep and add "(owner unclear)".
- Create a Word document named `<District>_<ST>_3_Demo Debrief.docx`.
- Keep the document to 3 pages maximum.

### Section 1: Salesforce Updates
- Start with the exact line: `Copy these into Salesforce.`
- Add **Demo Notes**: 3 paragraphs, about 200 to 300 words total. (1) What we showed and how the district responded, by {{MODULE_1}}, {{MODULE_2}}, and {{MODULE_3}}. (2) Technical Q&A, including ERP, data, integration, and security. (3) Objections, concerns, and other factors that could affect the deal or the implementation.
- Add **MEDDPICC Changes**: only the components whose status or evidence changed since the Demo Prep document. Use the same status labels as the Demo Prep document (Confirmed, Partial, or Gap). For each, give the new status and 1 to 2 sentences on what in the demo moved it. If none changed, write "No changes."

### Section 2: Next Steps
- Add **Follow Up Tasks** as a table: AE To Do | Solution Rep To Do | SE To Do, one task per cell, with a due date if stated.
- Add **Next Steps**: the agreed next meeting or action, owner, and date. If none was agreed, say so.
- Add **Dealbreakers**: stated must-haves with the speaker, or "None stated".
- Add **Product Gaps**: requests not met by something shown, with the speaker, each labeled "Confirmed gap" (the SE said it is not supported) or "Needs follow-up".

### Section 3: SE Details
- Start on a new page.
- Add **Plan vs Actual**: which Demo Focus items landed, were skipped, or got unplanned time. Up to 4 bullets.
- Add **Implementation Implications**: up to 4 bullets on data, ERP, timeline, staffing, or change management.
- Add **Stakeholder Read**: one line per district attendee: main interest and response, based only on what they said.
- Add **Playbook Signals** as a table: District pain (no names) | Capability shown | How it was framed | District reaction | Objection or follow-up. One row per moment the district reacted to something shown. No district names, person names, or identifying numbers.

## Final Check
- Demo Notes are 3 paragraphs and about 200 to 300 words.
- MEDDPICC Changes use the Demo Prep status labels and say what moved each status.
- Every task has an owner.
- Playbook Signals is anonymized.
