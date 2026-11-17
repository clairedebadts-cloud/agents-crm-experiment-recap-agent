# Braze test recap, week of 10 to 16 November 2026 (DRAFT, not sent)

## Email

**To:** (you decide)
**Subject:** Braze test recap: evening pickup window (B2B, DE)

Hi,

**Result:** The earnings message (Variant A) is ahead of Control. 14 partner stores added a second pickup window with Variant A, against 10 with Control. That is a conversion rate of 1.77% against 1.27%, a lift of about 40% (+39.6%). It is not a winner: there is no analysis report, and no significance test has been run. One week of data, 14 against 10 stores, is a small base.

**Test: ask partner stores to add an evening pickup window (B2B, market DE, campaign cmp_b2b_5503).** Sent Tuesday 10 November at 17:00, attributed over 7 days (10 to 16 November). All rates below are against deliveries, not sends.

| | Control | Variant A |
|---|---|---|
| Sends | 800 | 800 |
| Deliveries | 790 | 792 |
| Unique opens (incl. machine opens) | 385 (48.7%) | 407 (51.4%) |
| of which machine opens | 170 | 180 |
| Unique clicks | 48 (6.1%) | 62 (7.8%) |
| Conversions (store added a second pickup window) | 10 (1.27%) | 14 (1.77%) |
| Expected extra bags per day | 19 | 31 |
| Unsubscribes | 2 | 2 |

Variant A's subject line was "Stores like yours add 2 bags a day with an evening slot". Control's was "Add an evening pickup window". Variant A is ahead on clicks (about +29% against Control) and on conversions (about +40%). It is also ahead on opens, but open rates include machine opens (Apple Mail Privacy Protection), so we don't judge on opens. Stores in Variant A expect to list 31 extra bags a day in the new slot, against 19 for Control. That is about 2.2 bags per store against 1.9. These are the stores' own expectations, not sales. Unsubscribes were equal (2 each) and there were no spam reports.

There is no revenue for this test. Revenue is only tracked for B2C, and there was no B2C campaign this week.

**Checks:** Braze conversions match the partner action rows: 10 for Control and 14 for Variant A, and they match day by day. The transactions file has only a header row, which is right because there was no B2C campaign.

**What to watch:** Whether Variant A stays ahead over more sends. Run a significance test before calling it a winner. This is one week, one market (DE) and one send. Also watch whether the stores that added a window really list the extra bags.

## Slack

Braze recap, B2B evening pickup window (DE, 10 to 16 Nov): Variant A (earnings angle) is ahead of Control, not confirmed.
Stores that added a second pickup window: 14 with Variant A, 10 with Control. That is 1.77% against 1.27% of deliveries (792 and 790), a lift of about 40%.
Clicks: 62 (7.8%) against 48 (6.1%). Opens 51.4% against 48.7%, but opens include machine opens, so we don't judge on them.
Expect 31 extra bags a day from Variant A stores, against 19 from Control. There is no revenue, because B2B has none.
Braze matches the partner action rows. No analysis report and no significance test yet, one week only, so don't treat it as settled.
