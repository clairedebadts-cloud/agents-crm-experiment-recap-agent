# Braze test recap, week of 3 to 9 November 2026

Status: DRAFT for approval. Nothing has been sent.

## Email

**Subject:** Braze test recap, 3 to 9 Nov: Variant B is ahead of Control, not a winner, retest

Hi,

**Result.** In the subject line test (B2C, DE/FR/NL), Variant B (emoji + price) is ahead of Control on bag purchases, but it is not a winner. Per delivered email, purchases are 12% higher: 0.67% against 0.60% for Control. The data team's test says this is significant at 95% but not at our 98% rule (p = 0.036). By market, B against Control: DE +12.3% (p 0.18, not significant), FR +17.2% (p 0.053, not significant), NL -0.7% (p 0.96, flat). The data team recommends a retest and no roll-out.

**Subject line test (B2C, Winter dinner bags).** Sent Tuesday 3 Nov at 17:00, results counted for 7 days (3 to 9 Nov). Rates are against delivered emails.
- Purchases: Control 637 from 106,798 delivered (0.60%). Variant A (scarcity) 847 from 106,796 (0.79%). Variant B 725 from 108,518 (0.67%).
- Lift against Control: A +33.0%, B +12.0%.
- Variant A is further ahead than B, but the data team's report only tests B. A has no significance result, so it is ahead, not confirmed. Its lift by market: DE +34.7%, FR +37.7%, NL +18.5%.
- The markets do not move together: B is flat in NL, A is ahead in all three.
- Revenue after refunds: Control EUR 3,712.33, A EUR 4,956.08, B EUR 4,216.50. The data team's report gives no revenue figure, so these are summed from the transactions file after taking out the 39 refunded orders (Control 20, A 13, B 6; refunds tallied by hand). Braze shows EUR 3,839.46 / EUR 5,028.24 / EUR 4,245.38 (Control / A / B) because it counts refunded orders.
- Opens and clicks: unique open rate is 43.9% Control, 44.9% A, 48.2% B. These include machine opens (about half of all opens, from Apple Mail Privacy Protection), so they say little about interest and are not a reason to pick a variant. Click rate: 3.1%, 3.7%, 3.2%. Unsubscribes: 162, 167, 176 (about 0.15 to 0.16% each, no real difference).

**Partner stores test (B2B, second pickup window).** Same send and window, 3 to 9 Nov.
- Stores that added a second pickup window: Control 178 from 8,248 delivered (2.16%), Variant A (earnings angle) 188 from 8,101 (2.32%). That is +7.5% for A.
- By market: DE 72 against 68 (A -5.7%), FR 80 against 74 (A -4.5%), NL 26 against 46 (A +81.8%). A is ahead overall only because of NL, where the numbers are small. In DE and FR it is behind.
- Stores expect to list 357 extra bags a day (Control) and 378 (A), so +21 bags a day, +5.9%.
- Unique open rate (includes machine opens) 51.4% against 53.5%. Click rate 5.8% against 7.6%. Unsubscribes 4 against 5.
- There is no analysis report for this test, so no significance test: A is ahead, not confirmed.

**Checks.**
- B2C: the transactions file has 2,209 purchases, and Braze shows 2,209. I checked the total only, not the split per variant. I did not re-add all 2,209 amounts, so revenue against the Braze revenue column is not confirmed.
- B2B: the partner actions file has 366 rows, and Braze shows 366. The split (178 Control, 188 A) and the 236 on send day match Braze.

**What to watch.**
- One week of data only. The only significance test is B against Control; none was run for A or for the B2B test.
- Ask the data team to test Variant A and the B2B test, and put A into the retest with B.
- Do not roll out B on this week's numbers. Retest first.
- Check NL separately: B is flat there, and A's B2B result depends on it.

Best,
[name]

## Slack version

*Braze tests, 3-9 Nov (one week, no roll-out yet)*
- B2C subject lines, purchases: Control 637, A 847, B 725 (0.60% / 0.79% / 0.67% of delivered). B is +12% on Control, p 0.036: significant at 95%, not at our 98% rule, so B is not confirmed. A is +33% but the data team did not test it.
- B vs Control by market: DE +12.3% (p 0.18), FR +17.2% (p 0.053), NL -0.7% (flat); none significant alone, markets differ. A: DE +34.7%, FR +37.7%, NL +18.5% (no test).
- Revenue after refunds (report has no revenue figure): Control EUR 3,712.33, A EUR 4,956.08, B EUR 4,216.50. Braze shows EUR 3,839.46 / EUR 5,028.24 / EUR 4,245.38 because it counts 39 refunded orders. Purchase counts match the transactions file (2,209).
- B2B second pickup window: Control 178 stores, A 188 (+7.5%); DE 72 v 68 (-5.7%), FR 80 v 74 (-4.5%), NL 26 v 46 (+81.8%). Stores expect 357 v 378 extra bags a day. Ahead only through NL, no test run; counts match the partner file (366).
- Next: retest B (with A), do not roll out. One week only; open rates include machine opens, so not used.
