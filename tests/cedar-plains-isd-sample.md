# Sample Discovery Brief: Cedar Plains ISD (fictional)

This is the answer key for testing v3. It follows `deal-discovery-prep` exactly. The district, people, schools, publishers, figures and links are fictional and were adapted from a real answer key built from public sources. To use it as a live test, rebuild it for a real district from that district's public sources, then run the same intake in the agent and compare section by section.

## Test input

```text
Discovery Prep.
District: Cedar Plains ISD
State: TX
Discovery Date: November 10, 2026
Attendees (name, title): Dr. Alan Reyes, Deputy Superintendent of Finance and Operations/CFO; Dana Whitfield, Director of Financial Services
{{VENDOR}} Products:
What we know so far:
Links or attachments (budget book, board presentation, recent news):
```

**Expected file name:** CedarPlainsISD_TX_1_Discovery Brief.docx

**Expected chat reply:** the file, plus "Cedar Plains Independent School District, Cedar Plains, Texas. Missing: {{VENDOR}} Products, What we know so far, Links."

## Page 1: Rep Summary

### Cedar Plains Independent School District Discovery Brief

**Opportunity**

| Field | Value |
|---|---|
| District | Cedar Plains Independent School District, Cedar Plains, Texas |
| Discovery Date | November 10, 2026 |
| {{VENDOR}} Products | |

**District Facts**

| Total Enrollment | Schools | Total Budget | ERP |
|---|---|---|---|
| 14,020 (average enrollment, fiscal 2025) | 21 campuses plus 2 alternative programs | $141.6M General Fund expenditures, 2026-27, adopted | Unknown, ask Q2 |

**Brief**

Trustees adopted the 2026-27 General Fund budget on Aug. 25, 2026, with spending about $3.6 million above revenue; district leaders tied the gap to lower enrollment, a $1,000 employee stipend, and a plan to reduce campuses. Discovery should learn how enrollment projections set campus staffing as two more elementary schools close, and how program budget packages roll up into the adopted budget.

**What We Understand**

- Your average enrollment fell 7.8% from fiscal 2021 to 2025, to 14,020 students, while teacher FTEs fell 10.8%.
- Your adopted 2026-27 General Fund budget plans $141.6 million in spending against $138.1 million in revenue.
- You are reducing campuses: three elementary schools closed in the past year, and Hillside and Maple close after 2026-27.

**Listen For**

- Q3: Programs build budgets as unit packages with three years of actuals; learn who prepares them and how they roll up.
- Q7: Five elementary closures change where students go; learn how dollars and staff follow them to receiving campuses.
- Q9: The 2026-27 budget was adopted in August; confirm whether a purchase would use this year's funds.

**Budget Timing**

- Fiscal Year: September 1 to August 31 (Financial Transparency page, fiscal year ended August 31, 2025).
- Where They Are: November 10, 2026 is month 3 of fiscal 2026-27; the budget went to an August 11, 2026 workshop and was adopted August 25, 2026.
- Timing Read: Likely: current-year funds, from funds already identified or mid-year savings, with time to implement before 2027-28 budget work.
- Process Clues:
  - Program budgets are built as budget unit packages, each showing three years of actuals, the current budget, year-to-date actuals, and next year's budget (2026-27 Budget Workshop Book).

**Who We're Meeting**

| Name | Title | Budget Lens |
|---|---|---|
| Dr. Alan Reyes | Deputy Superintendent of Finance and Operations/CFO | Likely: narrowing the $3.6 million 2026-27 gap during the year while enrollment falls and campuses close. |
| Dana Whitfield | Director of Financial Services | Likely: assembling program budget packages and tracking spending against the adopted budget. |

**Strategic Direction**

Board Goals; board-adopted goals; years not stated; status: Undated (district Board Goals page). Goal areas: Student Achievement; Family and Community Engagement; Safe and Modern Facilities.

**In the News**

- Aug. 28, 2026, Cedar Plains Courier: Trustees voted 7-0 to adopt the 2026-27 General Fund budget, with $141.6 million in spending and $138.1 million in revenue, and set a $1.0712 tax rate.
- Aug. 28, 2026, Cedar Plains Courier: Elm, Oakridge and Pinecrest elementaries closed in the past year; Hillside and Maple elementaries close at the end of 2026-27.

## Page 2: Call Sheet

The call sheet should match the opening and Q1 to Q9 in [`deal-discovery-prep`](../skills/deal-discovery-prep/SKILL.md) word for word, each followed by "Notes:".

## Page 3: SE Layer

**Public Data Depth:** Moderate. Found: adopted 2026-27 budget figures, five years of enrollment and staffing, and program budget packages. Not found: a budget calendar, a budget process description, and the ERP.

**Attendee Backgrounds**

| Name | Background |
|---|---|
| Dr. Alan Reyes | Named CFO and Assistant Superintendent of Business Support Services, April 2022; earlier principal, Westbrook Middle School, and assistant principal, Lakeview High School. |
| Dana Whitfield | No public background found. |

**Alternate Bullets**

- Your programs build budgets as unit packages showing three years of actuals beside next year's budget.
- State revenue makes up about 61% of your 2026-27 General Fund revenue.

**Bullet Support**

1. 7.8% enrollment decline (15,200 in fiscal 2021 to 14,020 in fiscal 2025) and 10.8% teacher FTE decline (1,012.5 to 903.2). Financial Transparency, Cedar Plains ISD.
2. 2.5% of spending: $141,615,220 in expenditures against $138,050,904 in revenue, a $3,564,316 gap. 2026-27 Budget Workshop Book; Cedar Plains Courier, Aug. 28, 2026.
3. Five elementary campuses closed or closing: three in the past year, Hillside and Maple after 2026-27. Cedar Plains Courier, Aug. 28, 2026.

**Issues to Explore**

- **Three enrollment figures.**
  - Evidence: 14,020 average enrollment in fiscal 2025 (district); 13,480 in the most recent state data, year not stated (state school data explorer); 12,280 students on every 2026-27 budget package.
  - What it could mean: 2026-27 projections may sit well below last year's enrollment, or the figures measure different things.
  - Question to validate: Which enrollment number drives 2027-28 staffing and revenue, and who produces it?
- **Campus consolidation.**
  - Evidence: Board President Jordan Ellis tied a balanced budget to getting campus locations right; five elementary closures in two years.
  - What it could mean: staffing allocations are being redrawn for receiving campuses.
  - Question to validate: How do staff and dollars move when a campus closes?
- **Closing the gap during the year.**
  - Evidence: officials said they would work during 2026-27 to narrow the $3.6 million gap.
  - What it could mean: mid-year savings or reduction decisions are ahead.
  - Question to validate: Which options are being considered this year, and how are they modeled?

**Unknowns**

- ERP and hosting.
- When 2027-28 budget work starts and who submits requests; no calendar is published.
- Who approves software purchases, and at what dollar threshold.

**Clues to Confirm**

- Clue: the district site links a staff self-service portal; its vendor is not stated.
- Clue: the district site links a {{VENDOR}} parent portal and a learning management system; confirm {{VENDOR}} Products in Salesforce.
- Clue: the Purchasing pages list BuyBoard and other purchasing cooperatives.

**Sources**

1. [Financial Transparency](https://example.org/cedar-plains-isd/financial-transparency), Cedar Plains ISD, undated.
2. [Budget Workshop Book 2026-2027](https://example.org/cedar-plains-isd/budget-book-2026-2027.pdf), Cedar Plains ISD, Aug. 11, 2026.
3. [Cedar Plains ISD Addresses $3.6 Million Budget Deficit](https://example.org/cedar-plains-courier/budget-deficit), Cedar Plains Courier, Aug. 28, 2026.
4. [District Administration](https://example.org/cedar-plains-isd/district-administration), Cedar Plains ISD, undated.
5. [Cedar Plains ISD Welcomes New Administrators](https://example.org/cedar-plains-courier/new-administrators), Cedar Plains Courier, Apr. 14, 2022.
6. [Board Goals](https://example.org/cedar-plains-isd/board-goals), Cedar Plains ISD, undated.
7. [Cedar Plains ISD student and teacher data](https://example.org/state-schools-explorer/cedar-plains-isd), state school data explorer, undated.

## How to score the agent's run

- **Must match exactly:** fiscal year, month 3, Timing Read of Current-year funds, the call sheet, "No public background found" for the Director of Financial Services, ERP Unknown, and no NCES ID (none was confirmed).
- **Must match in substance:** the three bullet topics, the enrollment-figure issue, and the campus closures.
- **May differ in wording:** Brief, Listen For, Budget Lens, and Issues to Explore, as long as every fact traces to a source.
- **Fail:** a guessed ERP, an NCES ID that is not sourced, a background for the Director of Financial Services taken from a different person, the proposed budget instead of the adopted one, or any section filled with generic text.
