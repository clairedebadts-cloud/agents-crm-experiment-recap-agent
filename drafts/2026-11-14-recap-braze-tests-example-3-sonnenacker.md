# Draft: Braze tests recap, 20-26 Oct 2026, Sonnenacker example (not sent)

Source: data/examples/example-3-sonnenacker/ (3 CSVs and the README). Invented data. Rates are against deliveries. Week = send on Tue 20 Oct, plus 7 days of results. No analysis report was in data/, so the numbers could not be checked against one.

## Email

Subject: Braze tests, week of 20 Oct: no clear difference between the variants

Hi,

Here is the recap of last week's Braze test.

**Result: no clear difference. Variant A is slightly ahead, but the gaps are tiny. Nothing is called a winner: there is no analysis report and no significance test, and it is one week of data.**

**B2B surplus alert reminder (partner stores, DE and AT)**
Variant A, "Your surplus alert is waiting", got 6.09% clicks against 5.98% for Control, "Remind your team to list surplus bags" (+2%). Stores added a second pickup window 40 times for Variant A and 38 times for Control: 2.26% against 2.14% of delivered emails (+5%). Stores expect about 86 extra bags a day from Variant A and 75 from Control. Those are expected, not sold.
Open rates were 49.1% and 48.1%. Opens include machine opens, so they say little. Unsubscribes were 12 for Variant A and 17 for Control, both low.

**What to watch**
- A gap of 2 stores (40 against 38) is well within what chance can produce. I would not act on this result.
- One week, no significance test. There was no B2C test, so the transactions file has only a header row. That is expected.
- The data is invented, per its README. Braze windows added match the partner actions file (78 rows).

## Slack

*Braze tests, 20-26 Oct: no clear difference*
- B2B surplus alert: A had 40 stores add a window vs 38 for Control (2.26% vs 2.14%, +5%). Clicks 6.09% vs 5.98% (+2%).
- Stores expect 86 extra bags a day (A) vs 75. These are expected, not sold.
- Unsubscribes: 12 for A, 17 for Control, both low.
- The gap is tiny, so I would not act on it. One week, no significance test, no analysis report.
