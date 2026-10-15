# The Mechanic · FinWise

> Module 3 · Retention & Engagement. The engagement mechanic that builds the habit loop, with rationale and a wireframe.

## The mechanic

**Mechanic:** Progress Bar: a forecast confidence meter that tracks how trustworthy the cash forecast is, not how much the app is used.

- **Trigger:** The weekly cash moment before payroll or bills are due. A notification fires only when there's new data: *"14 new transactions since your last review. Update your forecast before Friday's payroll."*
- **Action:** Import the latest transactions and review the updated cash-flow forecast, ideally with an accountant or co-founder (weekly cadence).
- **Reward:** The confidence bar moves up, with a concrete answer: *"Forecast confidence: High. Last month's forecast was within 5% of actual. You have 6 weeks of cash runway, so the March hire is covered."* The answer is new each week.
- **Investment:** Confirm transaction categories, add known upcoming items (invoices due, a planned hire, a tax payment), or invite an accountant. Each one makes next week's forecast more accurate and next week's trigger more relevant.

_____

## Rationale

This addresses value-related churn. Modeling use nearly doubled (25% → 47%), yet sessions got shorter (11.5 → 9.3 min, and only 5–8 min in Jul–Sep), and churn rose from 19 to 29 a month. Users are trying the forecast but not getting an answer they can act on. Price isn't the driver: revenue per conversion stayed flat at $78,125 while churn rose.

This progress bar measures how trustworthy the forecast is, not how active the user is. Every review ends in a decision or a check of accuracy, so the value shows up each week. A user about to churn is the one who opens a forecast, can't act on it, and leaves after 5 minutes. They would stay because the forecast now shows it's right and answers a real question. Leaving for a spreadsheet would also mean losing the accuracy they've built up. Because FinWise uses a reverse trial, users build 2–3 weeks of confidence before the paywall. Losing a "High confidence" forecast when they're downgraded is a real loss, and it comes from value they've seen rather than pressure from a streak.

_What I chose not to build: a forecast-freshness streak. Loss aversion only works when the thing being lost has value, and the data suggests modeling isn't delivering it yet. A streak would push more of the activity that's rising alongside churn. To validate (Module 4): compare 1-year churn for modeling vs. non-modeling users, and check whether shorter sessions mean users finish quickly or give up partway through._

_____

## Wireframe

[Clickable wireframe: forecast confidence habit loop](https://claude.ai/artifact/8FCBDDiyfDqVp3nJPMCzZq): three screens, (1) trigger on the home screen, (2) weekly review with the confidence bar moving Medium → High, (3) investment step to add upcoming items and invite an accountant. Sample business data is illustrative.

![FinWise forecast confidence habit loop: trigger, action and reward, investment](habit-loop-wireframe.png)

_____
