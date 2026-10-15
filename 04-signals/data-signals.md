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
