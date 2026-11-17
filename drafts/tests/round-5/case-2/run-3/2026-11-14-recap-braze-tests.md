# Draft: Braze test recap, week 3-9 Nov 2026 (not sent, for approval)

## Email

**Subject:** Braze test recap, 3-9 Nov: Variant A is the winner in the B2C subject line test

Hi,

**The result:** In the B2C subject line test, Variant A ("Only 3 dinner bags left near you") is the winner. It got 847 Surprise Bag purchases against 637 for Control. That is 0.79% of delivered emails against 0.60%, a lift of +33%. The data team's analysis report shows this is significant at 98%. The B2B test is ahead for Variant A, but it is not a winner.

How to read the numbers: all rates are against deliveries (emails that arrived), not sends. Lift is a variant's rate against Control's. Conversions are Surprise Bag purchases (B2C) and stores adding a second pickup window (B2B).

**B2C: subject line test, Winter dinner bags (DE, FR, NL).** Each variant went to about 107,000 to 108,500 people.
- Control ("New Surprise Bags near you tonight"): 106,798 delivered, 637 purchases (0.60%).
- Variant A ("Only 3 dinner bags left near you"): 106,796 delivered, 847 purchases (0.79%), +33% against Control.
- Variant B ("Rescue tonight's dinner for 4.50 EUR", with emoji): 108,518 delivered, 725 purchases (0.67%), +12% against Control. It is ahead of Control, and the report does not call it a winner.
- Revenue, after refunded orders are taken out: Variant A 4,956.08 EUR, Variant B 4,216.50 EUR, Control 3,712.33 EUR, 12,884.91 EUR in total. Braze shows 13,113.08 EUR because it counts 39 refunded orders.
- Opens (these include machine opens, which are opens triggered by Apple Mail Privacy Protection, so they overstate real reading): Control 43.9% (46,857), Variant A 44.9% (47,959), Variant B 48.2% (52,263). Variant B has the highest open rate, but I do not call anything on opens alone. Clicks: Control 3.12% (3,336), Variant A 3.67% (3,922), Variant B 3.24% (3,516). Unsubscribes were similar: 162, 167 and 176.
- The three markets differ. Purchase rate against deliveries (Control / A / B): DE 0.60% / 0.81% / 0.68%, FR 0.58% / 0.80% / 0.68%, NL 0.63% / 0.74% / 0.62%. Variant A is ahead of Control in all three: DE +35%, FR +38%, NL +19%. Variant B is ahead in DE (+12%) and FR (+17%) and level with Control in NL (about -1%). The report's 98% result is for the total, not for each market.

**B2B: ask partner stores to add a second pickup window (DE, FR, NL).**
- Control ("Add a second pickup window to your store"): 8,248 delivered, 178 stores added a window (2.16%).
- Variant A (earnings angle, "Stores like yours sell 2 more bags a day with an evening slot"): 8,101 delivered, 188 stores added a window (2.32%), +8% against Control.
- Variant A is ahead, not a winner. The analysis report does not cover this test and no significance test is shown, so a gap of 10 stores should not be taken as proof.
- The markets point in different directions. Variant A is behind Control in DE (68 against 72 stores, -6%) and FR (74 against 80, -5%), and well ahead in NL (46 against 26, +82%). The whole B2B gap comes from NL, and those numbers are small.
- The stores that added a window expect to list about 378 extra bags a day for Variant A and 357 for Control (about 2 per store in both). These are the stores' own expectations, not sales.
- Opens (include machine opens): Control 51.4% (4,236), Variant A 53.5% (4,334). Clicks: Control 5.78% (477), Variant A 7.58% (614). Unsubscribes: 4 and 5.

**Checks against the other files.**
- B2C: Braze counts 2,209 purchases in total, and the transactions file has 2,209 rows. The total matches. I did not re-add the 2,209 order amounts or the refunded orders myself, so the revenue and the 39 refunds are the data team's figures, not rechecked. I also did not split the transaction rows by variant, so the purchase counts per variant are Braze's.
- B2B: Braze counts 366 store actions (178 Control, 188 Variant A), and the partner actions file has 366 rows (178 and 188). They match.
- The user and store ID columns hold one placeholder value for every row, so I could not check for the same person or store counted twice.

**What to watch.**
- This is one week only (send on Tue 3 Nov, 7 days of attribution). A second week would show if the B2C lift holds.
- The B2C result is significant for Variant A on the total. There is no significance result for Variant B, and none for B2B.
- NL reacts differently from DE and FR in both tests. Look at each market before a roll-out.
- Do not use the open rates to pick a subject line while machine opens are included.
- Next step: use Variant A's subject line in B2C as the new default if you agree, and retest B2B for another week before changing anything.

(Draft only. Nothing has been sent.)

## Slack version

**Braze tests 3-9 Nov (one week, draft)**
- B2C subject lines: Variant A is the winner, 847 purchases vs 637 Control (0.79% vs 0.60% of deliveries, +33%, significant at 98% per the data team); Variant B 725 (+12%), ahead, not a winner.
- B2C revenue after refunds: 12,884.91 EUR total (A 4,956.08, B 4,216.50, Control 3,712.33). Braze shows 13,113.08 because it counts 39 refunded orders.
- B2C markets differ: A ahead in all three (DE +35%, FR +38%, NL +19%), B level in NL; open rates include machine opens, so no call on opens; unsubscribes similar.
- B2B second pickup window: A 188 stores vs Control 178 (+8%), ahead, not a winner, no significance test; DE -6%, FR -5%, NL +82% (46 vs 26); stores expect 378 vs 357 extra bags a day.
- Purchases (2,209) and store actions (366) match their rows; revenue and refunds not rechecked. One week only: retest B2B, check each market before rolling out.
