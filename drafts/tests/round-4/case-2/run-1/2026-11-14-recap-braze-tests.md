# Draft: Braze test recap, week of 3-9 Nov 2026 (not sent, for approval)

Source: sample_braze_campaign_daily.csv, sample_transactions.csv, sample_partner_actions.csv, README_sample_data.md, analysis_report.md (case-2, synthetic data). One week only: send Tue 3 Nov 17:00, 7 days of attribution.

---

## EMAIL

**Subject:** Braze test recap, 3-9 Nov 2026

Hi,

**Result.** In the B2C subject line test, Variant A ("Only 3 dinner bags left near you") is the winner. It got 33% more purchases per delivered email than Control, and the data team's report says this is significant at 98%. In the B2B test, Variant A is ahead of Control by 7.5%, but that is not a winner: the report has no significance result for it, and A is behind in two of the three markets.

**B2C: Winter dinner bags, subject line test (DE, FR, NL).**
Rates below are against deliveries, not sends.
- Purchases (Braze conversions): Control 637, Variant A 847, Variant B 725.
- Purchase rate: Control 0.60% of 106,798 deliveries, A 0.79% of 106,796, B 0.67% of 108,518. Lift against Control: A +33%, B +12%.
- Revenue, refunded orders left out (as in the report): Control 3,712.33 EUR, A 4,956.08 EUR, B 4,216.50 EUR, total 12,884.91 EUR. Braze shows 13,113.08 EUR because it counts 39 refunded orders (the transactions file has exactly 39 rows marked refunded).
- Variant B (emoji + price) is ahead of Control but behind A. The report gives no significance result for B, so B is not a winner.
- By market, purchase-rate lift of A against Control: DE +35%, FR +38%, NL +19%. For B: DE +12%, FR +17%, NL -1% (level with Control). A is ahead in all three markets. The markets differ in size (NL has about 18,000 deliveries per variant, DE and FR 41,000 to 49,000), and NL shows the weakest lift.
- Open rates (these include machine opens, which are about 47% of all opens in every variant): Control 43.9%, A 44.9%, B 48.2%. B opened best, but opens alone say nothing about which variant is better, and B bought less than A.

**B2B: ask partner stores to add a second pickup window (DE, FR, NL).**
- Stores that added a second window: Control 178, Variant A 188. That is 2.16% against 2.32% of delivered emails (8,248 and 8,101 deliveries), a lift of +7.5% for A.
- By market, A against Control: DE 68 vs 72 stores (-6%), FR 74 vs 80 (-5%), NL 46 vs 26 (+82%). The overall edge for A comes from NL alone, on about 1,400 deliveries per variant, so it is a thin result.
- Stores expect to list 378 extra bags a day in the new slot after A and 357 after Control. That is about 2 bags per store in both, so the subject line changed how many stores said yes, not how big the slot is.
- Open rates (including machine opens): Control 51.4%, A 53.5%.

**Checks.**
- B2C: 2,209 rows in the transactions file match the 2,209 purchase conversions in Braze (the transaction IDs line up with Braze's counts per variant and market).
- B2B: 366 rows in the partner actions file match the 366 conversions in Braze (178 Control, 188 A).
- Every buyer ID and store ID in the files is the same placeholder value, so I could not check for repeat buyers or stores.

**What to watch.**
- This is one week and one send. I ran no significance test myself. The only test is the data team's 98% for A on B2C purchases. There is none for B, and none for B2B.
- B2B: do not roll out on this week. Retest, and look at DE and FR separately, where A was slightly behind.
- B2C: A is the clear leader, but the markets differ, so check NL again on the next send.
- Open rates include machine opens, so use purchases to judge subject lines.

Numbers behind this (7 days, summed over DE, FR and NL):

| B2C | Deliveries | Unique opens (incl. machine) | Clicks | Purchases | Revenue, refunds left out | Unsubscribes |
|---|---|---|---|---|---|---|
| Control | 106,798 | 46,857 | 3,336 | 637 | 3,712.33 EUR | 162 |
| Variant A | 106,796 | 47,959 | 3,922 | 847 | 4,956.08 EUR | 167 |
| Variant B | 108,518 | 52,263 | 3,516 | 725 | 4,216.50 EUR | 176 |

| B2C purchases / deliveries | Control | Variant A | Variant B |
|---|---|---|---|
| DE | 254 / 42,090 (0.60%) | 331 / 40,721 (0.81%) | 279 / 41,160 (0.68%) |
| FR | 268 / 46,351 (0.58%) | 375 / 47,084 (0.80%) | 331 / 48,865 (0.68%) |
| NL | 115 / 18,357 (0.63%) | 141 / 18,991 (0.74%) | 115 / 18,493 (0.62%) |

| B2B | Deliveries | Unique opens (incl. machine) | Clicks | Stores that added a window | Extra bags a day they expect | Unsubscribes |
|---|---|---|---|---|---|---|
| Control | 8,248 | 4,236 | 477 | 178 | 357 | 4 |
| Variant A | 8,101 | 4,334 | 614 | 188 | 378 | 5 |

---

## SLACK

*Braze test recap, 3-9 Nov 2026 (draft)*
- B2C purchases / revenue (refunds left out): Control 637 / 3,712.33 EUR, A 847 / 4,956.08 EUR, B 725 / 4,216.50 EUR, total 12,884.91 EUR; Braze shows 13,113.08 EUR because it counts 39 refunded orders.
- A is the winner: purchase rate +33% vs Control (0.79% vs 0.60% of deliveries), significant at 98% per the report; B is ahead at +12% but behind A, with no significance shown.
- By market, A vs Control: DE +35%, FR +38%, NL +19%; B: DE +12%, FR +17%, NL -1%. Markets differ in size, NL is smallest; open rates (incl. machine opens) are highest for B at 48.2% but prove nothing alone.
- B2B second pickup window: A 188 stores vs Control 178 (+7.5%, ahead, no significance test); DE -6%, FR -5%, NL +82% (46 vs 26); stores expect 378 extra bags a day with A vs 357 with Control.
- Purchase and partner rows match Braze (2,209 and 366); one week only, so retest B2B and don't roll it out, and recheck NL for B2C.
