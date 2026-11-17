# Draft: Braze test recap, week of 3-9 Nov 2026 (not sent, for approval)

## Email

**To:** (you to fill in)
**Subject:** Braze tests, 3-9 Nov: Variant B is ahead but not proven, retest before rolling out

Hi,

**The result:** In the subject line test, Variant B ("Rescue tonight's dinner for 4.50 euro") got more purchases than Control, but the data team's analysis report says it is not a winner. The lift is +12% on purchases per delivered email, significant at 95% but not at the 98% bar we use. Recommendation from the report: retest, do not roll out. The markets do not agree, so read the overall number with care: DE +12.3% (not significant), FR +17.2% (not significant), NL -0.7% (flat).

All rates below are against deliveries (emails that arrived), not sends. This is one week only (send Tuesday 3 Nov, 17:00, then 7 days of attribution to 9 Nov).

**Subject line test, winter dinner bags (app users, DE, FR, NL).**
Purchases, all three markets together:
- Control ("New Surprise Bags near you tonight"): 637 purchases from 106,798 deliveries = 0.60%.
- Variant A ("Only 3 dinner bags left near you"): 847 purchases from 106,796 deliveries = 0.79%, which is +33% against Control.
- Variant B (emoji + price): 725 purchases from 108,518 deliveries = 0.67%, which is +12% against Control.

Variant B by market against Control: DE 0.68% vs 0.60% (+12.3%), FR 0.68% vs 0.58% (+17.2%), NL 0.62% vs 0.63% (-0.7%). The B lift comes from DE and FR; in NL there is no difference. The analysis report only covers Variant B. Variant A is clearly ahead on these numbers (ahead in all three markets), but no significance test has been run on it, so it is not a winner either.

Revenue: Braze shows 3,839 euro (Control), 5,028 euro (Variant A) and 4,245 euro (Variant B) because it counts refunded orders too. The analysis report gives no revenue figure and I did not total the refunds, so revenue after refunds is not known.

Opens, clicks and unsubscribes: open rates include machine opens (Apple Mail Privacy), so I do not use them to judge. They were 43.9% (Control), 44.9% (A) and 48.2% (B). Click rates were 3.1%, 3.7% and 3.2%. Unsubscribes were about 0.15% to 0.16% for all three.

**Partner stores test, second pickup window (DE, FR, NL).**
A store "converts" when it adds a second pickup window.
- Control ("Add a second pickup window to your store"): 178 stores from 8,248 deliveries = 2.16%.
- Variant A (earnings angle, "Stores like yours sell 2 more bags a day with an evening slot"): 188 stores from 8,101 deliveries = 2.32%, which is +7.5% against Control.
- By market, A against Control: DE 68 vs 72 (-5.7%), FR 74 vs 80 (-4.5%), NL 46 vs 26 (+81.8%). The overall gain comes from NL, where the numbers are small; in DE and FR Control is slightly ahead.
- Stores say they expect to list 378 extra bags a day (Variant A) against 357 (Control).
- No analysis report covers this test and no significance test was run, so A is ahead, not a winner.

**Checks.** Purchases in the transactions file (2,209 rows) match the Braze purchase count (2,209). Partner actions (366 rows) match the Braze store count (366), and the daily counts match for each of the 7 days. I did not re-add the order amounts, so the revenue check against the transactions file was not done, and I did not recount rows per variant and market in the transactions file. All user and store IDs in the files are the same placeholder, so unique buyers and unique stores cannot be checked.

**What to watch.**
- Retest Variant B, ideally with a longer window or more volume, before any roll-out.
- Ask the data team for a test on Variant A, which looks stronger than B on purchases.
- Ask for revenue after refunds.
- The partner store result rests on small NL numbers.

Thanks

---

## Slack version

**Braze tests 3-9 Nov (one week, rates vs deliveries)**
- App subject line test, purchases: Control 637, Variant A 847 (+33%), Variant B 725 (+12%). B is ahead but not proven: significant at 95%, not at the 98% bar. Retest, don't roll out. A has no significance test.
- B by market vs Control: DE +12.3%, FR +17.2% (both not significant), NL -0.7% (flat). The markets differ.
- Revenue: Braze shows 3,839 / 5,028 / 4,245 euro (Control / A / B) because it counts refunded orders too. The report gives no revenue figure; net of refunds is not known. Open rates include machine opens, not used to judge.
- Partner stores, second pickup window: Control 178, Variant A 188 (+7.5%). DE 68 vs 72, FR 74 vs 80, NL 46 vs 26 (+81.8%, small numbers). Expect 378 vs 357 extra bags a day. No test run, so A is ahead only.
- Purchase and store counts match the transaction and partner files; order amounts were not re-added.

---
Not sent. Saved for your approval.
