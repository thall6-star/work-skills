# Agent setup (v3)

Build v3 as a new agent, for example "Deal Workflow - {{PRODUCT}} v3", so v2 stays available for comparison.

## Build steps

1. **Check the two blocks written from source materials** before pasting:
   - **Call sheet** (Page 2 in `deal-discovery-prep`): the opening and Q1 to Q8 were transcribed from a prior known-good Discovery Brief, and Q9 was added. Compare them word for word with the Discovery Guide.
   - **Slide Bullet Rules** (`deal-discovery-prep`): written from known-good bullets in a prior Discovery Brief. If Discovery Research Method v1 has different rules, paste its rules into this block instead.
2. **Create the agent** and turn on the capability that creates Word files (Code Interpreter or document creation).
3. **Paste [`instructions.md`](instructions.md)** into the Instructions box (about 4,900 characters with placeholders filled; the box caps at 8,000).
4. **Add three skills** by pasting each `SKILL.md` in full: `deal-discovery-prep`, `deal-demo-prep`, `deal-demo-debrief`. If you started from a copy of v1, delete the old v1 skill named `deal-demo-prep` first.
5. **Confirm each skill saved in full.** The discovery-prep skill is about 11,300 characters. Open it after saving and check that the Final Check section is at the bottom.
6. **Knowledge:** `K-12 Finance Lens v1` only. Outlook off, Teams off, Copilot connectors off, Web search on, Attachments on.
7. **Add the four suggested prompts** below.
8. **Run Cedar Plains ISD first** with the exact intake in [`../tests/cedar-plains-isd-sample.md`](../tests/cedar-plains-isd-sample.md) and compare section by section. Then run the rest of the test set.

## Suggested prompts

Only the message is sent, so each one names its stage.

| Order | Title | Message |
|---|---|---|
| 1 | Start here. | Start here. How do I use this agent? |
| 2 | Discovery Prep. | Discovery Prep. |
| 3 | Demo Prep. | Demo Prep. Attached: the Discovery Brief, the discovery transcript, and my notes if I have any. |
| 4 | Demo Debrief. | Demo Debrief. Attached: the Demo Prep document and the demo transcript. |

## Knowledge

`K-12 Finance Lens v1` only (same file as v2). Keep `{{PRODUCT}} SE Discovery Guide v1` and `Discovery Research Method v1` as team reference documents; v3 does not load them.
