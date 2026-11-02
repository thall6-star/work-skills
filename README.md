# K-12 Sales Workflow Agent

An agent and three skills that support {{PRODUCT}} sellers and Solution Engineers through a K-12 district budgeting opportunity. Each stage produces one Word document for the opportunity folder, with Salesforce-ready content at the top.

| Stage | When | Skill | Produces |
|---|---|---|---|
| Discovery Prep | Before the discovery call | [`deal-discovery-prep`](skills/deal-discovery-prep/SKILL.md) | Discovery Brief (3 pages) |
| Demo Prep | Right after discovery | [`deal-demo-prep`](skills/deal-demo-prep/SKILL.md) | Demo Prep (4 pages) |
| Demo Debrief | After the demo | [`deal-demo-debrief`](skills/deal-demo-debrief/SKILL.md) | Demo Debrief (3 pages) |

## What's here

```
agent/
  instructions.md        Paste into the agent's Instructions box
  setup.md               Build steps, suggested prompts, knowledge settings
skills/
  deal-discovery-prep/SKILL.md
  deal-demo-prep/SKILL.md
  deal-demo-debrief/SKILL.md
tests/
  test-plan.md           Test districts, checklists, pilot plan
  cedar-plains-isd-sample.md   Answer key for the first test run
docs/
  design-notes.md        Why v3 is built this way; changes from v2
CHANGELOG.md
```

The knowledge file `K-12 Finance Lens v1` is not included.

## Placeholders

Vendor, product and product-module names are replaced with placeholders. Find and replace them before pasting anything into an agent:

| Placeholder | Meaning |
|---|---|
| `{{VENDOR}}` | The company that sells the product |
| `{{PRODUCT}}` | The product being sold |
| `{{MODULE_1}}`, `{{MODULE_2}}`, `{{MODULE_3}}` | The product's three functional areas, used to tag call sheet questions and rank demo focus |

The district in the sample answer key is fictional.

## Getting started

Follow [`agent/setup.md`](agent/setup.md).

## Changing it

This repo is the source of truth. Edit the file here, add a line to `CHANGELOG.md`, run the test set in [`tests/test-plan.md`](tests/test-plan.md), then paste the whole updated block into the agent.
