# The Validation · FinWise

> Module 5 · Experimentation Methods. The experiment brief that tests the bet.

## Method

**Method:** A/B test, randomized 50/50 per user: new trial signups get either the current onboarding or the 4-screen answer-first onboarding from Module 2.

**Why:** Onboarding can be randomized per user with no spillover between groups, and at ~490 trials a month an A/B test gives a clean read of the primary metric in about 8 weeks. Module 4 showed the monthly data can't settle cause and effect (import usage and conversion didn't move together), so only a randomized test can show whether the new flow causes more users to reach a first modeling output. Before launch, a 1–2 week A/A check confirms the new per-user tracking and the split work. After a win, a 5–10% holdout stays on the old onboarding to measure the long-term effect on trial → paid conversion and 1-year churn.

_Not chosen: geo testing (onboarding can be randomized per user, and ~490 trials a month split across regions would be noisy), switchback (no shared resource between users, and alternating by time would mix in month-to-month swings), multi-armed bandit (the result arrives 7 days after signup, and uneven groups would break the follow-through to conversion)._

_____

## Hypothesis + primary metric

If we replace the current trial onboarding with a 4-screen answer-first flow (pick a question → connect your account → confirm recurring items → see the answer), then more new trial users will import data and reach their first modeling output within 7 days, because the flow fills in their data automatically and ends on an answer to a question they chose, instead of an empty product.

**Primary metric:** % of new trial users who import data and reach their first modeling output within 7 days of signup (the North Star, measured per user), target: +10 percentage points over control (e.g. 40% → 50%; baseline to be confirmed during the A/A check)

_Experiment: Answer-first onboarding, A/B test (50/50)_

_Testing the 4-screen answer-first onboarding on all new trial signups. Current experience: full access to every feature from day 1, with no guided path to a first output._

_Predicted outcome: the treatment group reaches a first modeling output faster and more often. If successful: roll the flow out to 90–95% with a 5–10% holdout, follow those users through to trial → paid, then test the Module 3 weekly-review mechanic on top. If unsuccessful: find which of the 4 screens users drop off at. If they import but don't reach an output, the problem is the output, not onboarding. If nothing moves, onboarding isn't the bottleneck, and the North Star needs revisiting._

**Why the primary metric isn't trial → paid:** detecting a lift from 2% to 3% needs ~3,800 trials per group, about 15 months at FinWise's volume. The North Star metric, at a ~40% baseline with a +10-point target, needs ~390 per group (under 2 months). Trial → paid stays the long-term Prove metric from Module 4, read through the holdout. Because this test tracks individual users, it also answers the open Module 4 question: do users who reach a first modeling output actually convert more?

_Assumptions: the ~40% baseline is not yet measured (closest monthly figures: import ~44%, modeling ~48%, Jul–Oct 2024); details of the current day-1 experience beyond "reverse trial, full access" are unconfirmed._

_____

## Guardrail + read date

- **Guardrail:** Onboarding completion (share of signups who finish onboarding) must not fall more than 5 points below control, since asking for a bank connection on screen 2 is the step most likely to scare users off. Trial → paid is also monitored and must not fall below control.
- **Read date:** 8 weeks after launch (~7 weeks to enroll ~780 trials at ~490 a month, plus 7 days for the last signups to reach their output). The A/A check runs for 1–2 weeks before launch.

_____
