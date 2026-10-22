# The Signals · FinWise

> Module 4 · Data & Analytics. The data pattern you found and the indicators you'll steer by.

## The data pattern

**From Module 1:** conversion is stuck at ~2%, and the biggest drop-off is the Revenue stage (98% of trials don't convert).

| Metric | Pattern |
|---|---|
| Trial-to-Paid Conversion | Ceiling, flat at 1.87–2.08% for 13 months |
| Modeling Usage % | Rising with big swings, 10.8% → 58% |
| Import Usage % | Ceiling, rose to ~40% then flat at 41–45% |
| Avg Session Duration | Cliff, 12.1 → 5.1 min from Jun to Aug 2024 |
| Sessions per User | Rising, 3 → 9 |

**Did import usage correlate with conversion?** No (r = −0.05). Revised my hypothesis: conversion isn't dropping and users do find the features.

**What it reveals:** Users are more active but sessions got shorter and conversion didn't move, so the problem is value, not engagement.

[Dashboard](https://claude.ai/artifact/6bnfDbjXqNUqtvh2M5Fai5) · [Data](../data/finwise-trial-funnel.csv)

_____

## Leading indicators

| Layer | Metric | Why |
|---|---|---|
| 🎯 Aim · North Star | Trial users who import financial data and reach their first modeling output | The behavior that shows a user has felt FinWise's core value. |
| 🔧 Move #1 | % of trial signups who import data in session 1 | No North Star without data in the product. |
| 🔧 Move #2 | Time from signup to first modeling output | Faster output, more time to see value before the trial ends. |
| 🔧 Move #3 | % of trial users with a second modeling output in a later week | Shows the first output was useful. |

_____

## Lagging indicators

| Layer | Metric | Why |
|---|---|---|
| ✅ Prove | Trial-to-paid conversion 2% → 3%, with lower year-one churn (60% today) | Shows the Revenue-stage drop-off is fixed at scale. |

_____
