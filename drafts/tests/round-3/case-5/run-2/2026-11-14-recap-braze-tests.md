# Braze test recap, week of 10 to 16 November 2026 (DRAFT, nothing sent)

## Email

**To:** (you to fill in)
**Subject:** Braze test recap: evening pickup window, B2B DE

Hi,

Result first: the "earnings angle" email (Variant A) is ahead of Control. 14 stores added a second pickup window after Variant A, against 10 after Control. That is a conversion rate of 1.77% against 1.27%, a lift of about 40%. It is not a winner: there is no analysis report for this week, so no significance test has been run, and the gap is only 4 stores.

**Test: ask partner stores to add an evening pickup window (B2B, Germany, sent Tuesday 10 Nov at 17:00, 7 days of results)**
- Control ("Add an evening pickup window"): 800 sent, 790 delivered. 10 stores added a second window (1.27% of deliveries). 48 clicks (6.1%). 2 unsubscribes.
- Variant A ("Stores like yours add 2 bags a day with an evening slot"): 800 sent, 792 delivered. 14 stores added a second window (1.77% of deliveries). 62 clicks (7.8%). 2 unsubscribes.
- Stores expect to list extra bags per day in the new slot: 31 with Variant A (14 stores) against 19 with Control (10 stores). Treat these as expectations from the stores, not sales.
- Opens: Control 385 (48.7% of deliveries), Variant A 407 (51.4%). These unique opens include machine opens (Apple Mail Privacy Protection): 170 for Control and 180 for Variant A. Opens are not a reliable sign of which email did better, so I did not use them to judge the test.

**Checks**
- Braze conversions match the partner actions file: 10 rows for Control and 14 for Variant A, same as the Braze counts, and the dates line up day by day.
- Revenue: none for B2B (Braze shows 0 by design), so there is nothing to compare.
- The transactions file has no rows because there was no B2C campaign this week. That check was not needed here.

**What to watch**
- One week, one market (DE), one B2B campaign, and no significance test. A difference of 4 stores could be chance. A retest or a larger send would tell us more before rolling Variant A out to everyone.
- Check whether the stores that added a window keep it open and really list the bags they expect.
- Unsubscribes are low and equal (2 each). No spam reports.

## Slack

*Braze test recap, 10 to 16 Nov (B2B, DE, evening pickup window)*
- Variant A (earnings angle) is ahead of Control: 14 stores added a window vs 10, so 1.77% vs 1.27% of deliveries (790 Control, 792 Variant A), lift about 40%. Not a winner: no analysis report, no significance test, only 4 stores apart.
- Stores expect 31 extra bags a day with Variant A vs 19 with Control (expectations, not sales). Clicks 62 vs 48.
- Opens (Variant A 51.4%, Control 48.7%) include machine opens, so we don't judge on them. Unsubscribes 2 each.
- Braze conversions match the partner actions file (14 and 10). No B2C test and no revenue this week. One week, one market (DE): retest before rolling out.
