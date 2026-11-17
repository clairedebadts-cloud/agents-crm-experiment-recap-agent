# Braze test recap: week of 10 to 16 November 2026 (DRAFT, not sent)

Source: ostseekorb_braze_campaign_daily.csv, ostseekorb_partner_actions.csv, ostseekorb_transactions.csv. One test this week (DE, B2B partner stores). The send went out Tuesday 10 Nov at 17:00, with 7 days of results (10 to 16 Nov).

## Email

**Subject: Braze test recap, 10 to 16 Nov: the earnings angle got more stores to add an evening pickup window**

Hi,

Result first: the earnings subject line (Variant A) got more partner stores to add a second pickup window than the plain one (Control). 14 stores added a window after Variant A and 10 after Control. Each variant was delivered to about 790 stores.

**B2B test: ask stores to add an evening pickup window (cmp_b2b_5503, DE)**

| | Control | Variant A (earnings angle) |
|---|---|---|
| Sent / delivered | 800 / 790 | 800 / 792 |
| Stores that added a window | 10 | 14 |
| Conversion rate (of delivered) | 1.27% | 1.77% |
| Clicks (unique) | 48 (6.1%) | 62 (7.8%) |
| Opens (unique, incl. machine opens) | 385 (48.7%) | 407 (51.4%) |
| Unsubscribes | 2 | 2 |
| Spam reports | 0 | 0 |

Variant A's conversion rate is 0.5 percentage points higher than Control's. That is a lift of about +40% against Control (1.77% vs 1.27%), which in plain numbers is 4 more stores out of roughly 790. Variant A also got more clicks: 7.8% against 6.1%, a lift of about +29%.

Opens are close (51.4% vs 48.7%). These counts include machine opens from Apple Mail Privacy Protection, which are about 44% of opens in both variants (170 of 385 and 180 of 407). So opens say little about who did better, and I'm not calling a winner from them.

The stores that converted also say how much they expect to add. Variant A stores expect 31 extra bags a day in total (about 2.2 per store). Control stores expect 19 (1.9 per store). This is what stores expect to list, not sales.

Unsubscribes were the same, 2 in each variant (0.25% of delivered).

**Checks:** Braze conversions match the partner actions file: 10 Control and 14 Variant A, and the day-by-day counts match too. There is no B2C campaign this week, so the transactions file is empty and there is no revenue to report.

**What to watch**
- This is one week and one send. The gap is 4 stores, so it could be chance. No significance test was run.
- Whether the stores keep the evening window and the extra bags actually show up.
- Whether Variant A holds its lead if repeated, before it becomes the default.
- No analysis report was in the files, so these numbers were not compared against one.

## Slack version

*Braze test recap, 10 to 16 Nov (DE, B2B evening pickup window)*
- Variant A (earnings angle) beat Control: 14 stores added a window vs 10, against about 790 delivered each.
- Conversion rate 1.77% vs 1.27% of delivered, about +40% lift. Clicks 7.8% vs 6.1%, about +29%.
- Opens 51.4% vs 48.7%, but about 44% are machine opens, so no call on opens alone.
- Unsubscribes 2 vs 2. Conversions match the partner actions file. No B2C this week.
- One week, 4 stores apart, no significance test, no analysis report to check against.
