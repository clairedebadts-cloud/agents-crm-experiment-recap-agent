# Braze test recap, week of 3-9 Nov 2026 (draft, nothing sent)

## Email

**Subject:** Braze tests recap, send of 3 Nov (attribution 3-9 Nov)

Hi,

**Result first:** in the app-user subject line test, Variant A ("Only 3 dinner bags left near you") is the winner. It got 33% more purchases than Control, significant at 98% according to the data team's analysis report. In the partner-store test, the earnings message is slightly ahead of Control, but that is not a winner: no significance result exists for it.

**B2C subject line test (Winter dinner bags, DE + FR + NL).** Rates below are against deliveries. Open rates include machine opens (about 47% of all opens in each variant), so they are not a reason to pick a variant.
- Control: 106,798 delivered, 637 purchases (0.60%), 3,336 clicks (3.12%), 46,857 opens (43.9%), 162 unsubscribes.
- Variant A: 106,796 delivered, 847 purchases (0.79%), 3,922 clicks (3.67%), 47,959 opens (44.9%), 167 unsubscribes. Purchases +33% against Control.
- Variant B ("Rescue tonight's dinner for €4.50"): 108,518 delivered, 725 purchases (0.67%), 3,516 clicks (3.24%), 52,263 opens (48.2%), 176 unsubscribes. Purchases +12% against Control. It is ahead, not a winner: the report gives no significance result for it.
- Revenue (refunded orders left out, from the analysis report): Control 3,712.33 EUR, Variant A 4,956.08 EUR, Variant B 4,216.50 EUR, total 12,884.91 EUR. Braze's own export shows a higher figure because it still counts 39 refunded orders, so we use the report's number.
- By market, purchases against Control (by deliveries): Variant A is ahead in all three: DE +35% (331 vs 254), FR +38% (375 vs 268), NL +19% (141 vs 115). Variant B is ahead in DE +12% (279) and FR +17% (331) and level in NL (115, about -1%). The markets differ, so the overall figure hides a smaller gain in NL.

**B2B test (partner stores, ask to add a second pickup window; DE + FR + NL).** Rates are against deliveries.
- Control ("Add a second pickup window to your store"): 8,248 delivered, 178 stores added a window (2.16%), 477 clicks (5.78%), 4,236 opens (51.4%), 4 unsubscribes.
- Variant A (earnings angle, "Stores like yours sell 2 more bags a day with an evening slot"): 8,101 delivered, 188 stores added a window (2.32%), 614 clicks (7.58%), 4,334 opens (53.5%), 5 unsubscribes. Conversions +8% against Control.
- Stores expect to list 357 extra bags a day in the new slots under Control and 378 under Variant A (the stores' own estimate, so expect, not a result). That is about 2.0 per store in both.
- Variant A is ahead overall, but not a winner. By market it is behind Control in DE (68 vs 72; 2.18% vs 2.31%) and FR (74 vs 80; 2.08% vs 2.18%) and well ahead only in NL (46 vs 26; 3.23% vs 1.78%). The overall lead comes from NL alone, a small market. Open rates include machine opens. B2B revenue is not tracked (always 0).

**What to watch**
- One week only (send 3 Nov, 7 days of attribution). Only the B2C subject line test has a significance result (the analysis report). No significance test was run for the B2B test or for Variant B.
- B2B: retest before rolling out the earnings angle. The lead sits in NL while DE and FR are slightly behind.
- Opens are inflated by machine opens (Apple Mail Privacy Protection). Judge on purchases and store conversions.
- Purchase counts include refunded orders. The report's 98% result is on conversions.
- Checks: the 2,209 rows in the transactions file match the 2,209 B2C conversions in Braze, and the 366 rows in the partner actions file match the 366 B2B conversions. Not done: I did not re-add the transaction amounts, split the transaction rows by variant or market, or recount the 39 refunded orders. The refund count comes from the analysis report, so revenue is not confirmed from the rows.

## Slack version

- App test (B2C, DE+FR+NL): Variant A ("Only 3 dinner bags left") is the winner, significant at 98% per the analysis report: 847 purchases vs 637 for Control (0.79% vs 0.60% of deliveries), +33%. Variant B is ahead, 725 purchases (+12%), not confirmed: no significance result.
- By market A is ahead everywhere: DE +35%, FR +38%, NL +19%. B: DE +12%, FR +17%, NL level. The markets differ. Opens include machine opens (~47%), so ignore them.
- Revenue (refunds left out, report): Control 3,712.33 EUR, A 4,956.08 EUR, B 4,216.50 EUR, total 12,884.91 EUR. Braze shows a higher figure because it still counts 39 refunded orders, so we use the report's number.
- Partner stores (B2B): Variant A is ahead, 188 stores added a second window vs 178 for Control (2.32% vs 2.16%, +8%), not confirmed, no significance result: ahead only in NL (46 vs 26), behind in DE (68 vs 72) and FR (74 vs 80). Stores expect 378 extra bags a day vs 357 for Control. Retest before rolling out.
- One week only, no significance test for B2B or Variant B. Purchase and store counts match the transaction and partner files (2,209 and 366). Revenue and refund count not re-added from the rows.
