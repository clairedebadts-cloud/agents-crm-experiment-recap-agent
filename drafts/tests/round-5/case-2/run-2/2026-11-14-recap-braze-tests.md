# Braze tests recap, week of 3-9 Nov 2026 (DRAFT, nothing sent)

Input: drafts/tests/cases/case-2/ (sample_braze_campaign_daily.csv, sample_transactions.csv, sample_partner_actions.csv, README_sample_data.md, analysis_report.md). One week: send Tue 3 Nov 17:00, 7 days of attribution (3-9 Nov). Markets DE, FR, NL.

---

## Email

**Subject:** Braze tests, 3-9 Nov: "Only 3 dinner bags left near you" is the winner for app users

**Result first.** In the app-user subject line test, Variant A ("Only 3 dinner bags left near you") is the winner. Its purchase rate was 33% higher than Control's (0.79% of delivered emails ended in a Surprise Bag purchase, against 0.60% for Control). The data team's report shows this is significant at 98%. Variant B (emoji and price) is ahead of Control but is not a winner: the report does not show it as significant. In the store test, Variant A is slightly ahead, but the gap is small and nothing shows it is a real difference.

Revenue from the app-user test, with refunded orders left out (as in the data team's report): 12,884.91 EUR in total. Control 3,712.33 EUR, Variant A 4,956.08 EUR, Variant B 4,216.50 EUR. Braze shows 13,113.08 EUR because it counts 39 refunded orders.

All rates below are against deliveries (emails that arrived), not sends. Unique opens include machine opens (Apple Mail Privacy Protection), so open rates are only a rough guide.

**App users: subject line test, Winter dinner bags (cmp_b2c_2645)**

| | Deliveries | Unique opens (incl. machine) | Clicks | Purchases | Purchase rate | Lift vs Control | Unsubscribes |
|---|---|---|---|---|---|---|---|
| Control ("New Surprise Bags near you tonight") | 106,798 | 46,857 (43.9%) | 3,336 (3.12%) | 637 | 0.60% | n/a | 162 |
| Variant A (scarcity) | 106,796 | 47,959 (44.9%) | 3,922 (3.67%) | 847 | 0.79% | +33% | 167 |
| Variant B (emoji + price) | 108,518 | 52,263 (48.2%) | 3,516 (3.24%) | 725 | 0.67% | +12% | 176 |

Variant A is the winner: +33% purchases against Control, significant at 98% per the analysis report. It also had the most clicks (3.67% of deliveries against 3.12% for Control). Variant B has the highest open rate (48.2%), but opens include machine opens, so we do not read that as a result. On purchases B is ahead of Control by 12%, and it is not a winner.

The markets differ. Variant A's purchase lift against Control was +35% in DE (0.81% against 0.60%), +38% in FR (0.80% against 0.58%) and +19% in NL (0.74% against 0.63%). Variant B was +12% in DE, +17% in FR and about level with Control in NL (0.62% against 0.63%, -1%). The NL group is the smallest (about 18,000 deliveries per variant), so its numbers move more with a few purchases. Prices also differ by market (4.50 EUR DE, 4.99 EUR FR, 4.95 EUR NL).

**Partner stores: second pickup window (cmp_b2b_0871)**

| | Deliveries | Unique opens (incl. machine) | Clicks | Stores that added a window | Rate | Lift vs Control | Unsubscribes |
|---|---|---|---|---|---|---|---|
| Control ("Add a second pickup window to your store") | 8,248 | 4,236 (51.4%) | 477 (5.78%) | 178 | 2.16% | n/a | 4 |
| Variant A (earnings angle) | 8,101 | 4,334 (53.5%) | 614 (7.58%) | 188 | 2.32% | +7.5% | 5 |

Variant A is ahead: 188 stores added a second window against 178 for Control, 10 more stores. The analysis report has no result for this test, so there is no sign this gap is more than chance. It is not a winner. The result is mixed by market: A is ahead in NL (46 stores, 3.2%, against 26, 1.8%) but behind Control in DE (68 against 72) and FR (74 against 80). Stores expect to list about 378 extra bags a day in the new slots after Variant A (188 stores, about 2.0 each) and about 357 after Control (178 stores, about 2.0 each). These are the stores' own expectations, so expect, not promise.

**Do the sources agree?** The purchase and store counts in Braze match the detail files: 2,209 app-user purchases in Braze and 2,209 rows in the transactions file; 366 store actions in Braze and 366 rows in the partner actions file. For stores, the per-variant counts (178 Control, 188 Variant A) also match the rows. For purchases I checked the total, not each variant's row count, and I did not recount the 39 refunded orders or the report's refund-free revenue from the rows; I used the report's figures.

**What to watch**
- This is one week and one send. The data team's significance result covers purchases in the app-user test only. No significance result is given for Variant B, for the store test, or for opens and clicks.
- Variant A did best in DE and FR and less clearly in NL. Retest before rolling a scarcity subject line out to all markets.
- Open rates include machine opens. Do not use them to pick a subject line.
- Store test: repeat it before changing how we write to stores; the gap is 10 stores and the markets point in different directions.

---

## Slack

*Braze tests 3-9 Nov (draft)*
- App users: Variant A is the winner, +33% purchases vs Control, significant at 98% (847 vs 637 purchases, 0.79% vs 0.60% of deliveries). Variant B ahead at +12% (725), not a winner.
- Markets differ: A is +35% DE, +38% FR, +19% NL; B is +12% DE, +17% FR, -1% NL. Retest before rolling out everywhere.
- Revenue 12,884.91 EUR (refunds excluded): Control 3,712.33, A 4,956.08, B 4,216.50. Braze shows 13,113.08 EUR because it counts 39 refunded orders. Purchase and store counts match the detail files.
- Stores: A ahead, not a winner, with no significance shown: 188 vs 178 added a window (+7.5%); ahead in NL, behind in DE and FR. Stores expect +378 bags/day (A) vs +357 (Control).
- One week only; opens include machine opens, so don't judge on opens. Rates are against deliveries.
