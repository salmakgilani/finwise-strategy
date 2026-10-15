# The Signals · FinWise

> Module 4 · Data & Analytics. The data pattern you found and the indicators you'll steer by.

## The data pattern

**Carried over from Module 1:**
- **Hypothesis:** FinWise's biggest growth problem is that trial-to-paid conversion has been stuck at ~2% for 13 straight months, because using the product during the trial isn't turning into a reason to pay.
- **Biggest drop-off: Revenue stage (trial → paid).** 98% of trials (6,296 of 6,424) don't convert, more than the 93% lost between visit and trial.

**What the funnel data revealed** _(source: [trial funnel data, Oct 2023 – Oct 2024](../data/finwise-trial-funnel.csv))_:
- **Conversion is a ceiling, not a decline.** Trial → paid held between 1.87% and 2.08% in all 13 months.
- **Usage rose, value didn't follow.** Modeling use nearly doubled (25% → 47%, first half vs. second half) while sessions got shorter (11.5 → 9.3 min, only 5–8 min in Jul–Sep) and 1-year churn rose from 19 to 29 a month.
- **The real problem behind the headline metric:** trial users try the forecast but don't stay with it long enough to get an answer they act on. All the indicators below sit inside the trial, before the paywall, where the Revenue-stage drop-off is decided.

**Pattern by metric** _(dashboard: [FinWise Trial Funnel](https://claude.ai/artifact/6bnfDbjXqNUqtvh2M5Fai5))_:

| Metric | Pattern |
|---|---|
| Trial-to-Paid Conversion Rate | **Ceiling.** Holds between 1.87% and 2.08% in all 13 months, even as trials swing from 321 to 644 a month. |
| Financial Modeling Feature Usage % | **Doesn't fit cleanly: rising, with big swings.** 10.8% (Nov 2023) to 58.3% (Apr 2024), down to ~37% (Jun), back to 58.1% (Sep), then 36.0% (Oct). Flagged because usage nearly doubled while conversion stayed at its ceiling. |
| Get Started Import Feature Usage % | **Ceiling.** Grew from ~30% (Jan–Mar 2024) to ~40% (Apr–Jun), then flattened at 41–45% (Jul–Oct). More than half of users still never import. |
| Average Session Duration | **Cliff.** Held at 11–14 min from Dec to Jun, then dropped from 12.1 min (Jun 2024) to 7.0 (Jul) and 5.1 (Aug). Hasn't recovered (7.9 and 9.0 min since). |
| Average Sessions Per User | **Doesn't fit cleanly: rising.** 3 (Jan 2024) to 8–9 by Aug–Oct, possibly flattening at 9. Flagged because, with the session-duration cliff, users come back more often but stay briefly. |

_Across all five: from July 2024, sessions per user rose to 7–9, modeling stayed at 47–58%, and session length dropped to 5–8 min, while conversion stayed flat at ~2%._

**Does the leading indicator correlate with conversion? No.** Import usage (the closest proxy in this data for "imported data in session 1") and trial → paid have a correlation of −0.05. Indexed to their 13-month averages, import usage swung from 78 to 116 while conversion stayed between 94 and 105. Months with more importing didn't produce more paid users.

**Hypothesis: ↻ Revised.** Exercise 1 started from "users don't see FinWise's value, and conversion has dropped over the year." The data contradicts both parts: conversion is a flat Ceiling, not a decline, and users do find the features (import 41–45%, modeling 47–58%, sessions per user up from 3 to 9).

**What the data pattern actually reveals:** FinWise has a value problem disguised as an engagement success. Every activity metric went up: users import, model, and come back more often. Conversion stayed capped at ~2% anyway. The session-duration Cliff in July 2024 (12.1 → 5.1 min) is the tell: users return more often but leave within minutes, consistent with glancing at a number rather than getting an answer they can act on. The real problem isn't getting users to use FinWise. It's that using it doesn't end in a decision they'd pay for: "can I make payroll," "can I afford this hire." Until the product turns activity into an outcome, pushing more activity won't move conversion.

_Implication for the North Star: import and modeling are the activities that rose without lifting conversion. This is monthly data, not user-level, so it doesn't rule the North Star out, but "first modeling output" should mean an output that answers a real question, and Module 5 should test whether reaching it predicts paying._

_____

## Leading indicators

Aim · Move · Prove, working backward from the North Star.

| Layer | Metric | Why (one sentence) |
|---|---|---|
| 🎯 **Aim** · North Star | The number of trial users who import financial data and reach their first modeling output. | The single behavior that proves a user has felt FinWise's core value. |
| 🔧 **Move** #1 (test first) | % of trial signups who import data in session 1 | The North Star can't happen without data in the product, and onboarding screen 2 (connect your money) is built to lift this. |
| 🔧 **Move** #2 | Time from signup to first modeling output | Every extra day before the first output is a day closer to the end of the trial, so speeding this up should lift the North Star and conversion together. |
| 🔧 **Move** #3 | % of trial users who run a second modeling output in a later week | A repeat during the trial shows the first output was useful, not just viewed. |

_Instrumentation gap: none of these can be read from today's monthly table. FinWise needs per-trial-user tracking of import, first modeling output (with timestamps), and repeat outputs by week._

_____

## Lagging indicators

| Layer | Metric | Why (one sentence) |
|---|---|---|
| ✅ **Prove** | Trial → paid conversion from 2% to 3%, with fewer customers churning in year one (today 60%) | It proves that more users reaching a modeling output actually fixes the Revenue-stage drop-off at scale. |

_Supporting outcomes: net paid customers per month (new minus churned, negative every month today) and revenue._

_The Prove metric also checks the North Star. Import and modeling rose last year without lifting conversion, so if the North Star rises and conversion still doesn't move, the North Star needs revisiting._

_____
