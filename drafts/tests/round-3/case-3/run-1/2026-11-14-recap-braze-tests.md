# Braze test recap, week of 3 to 9 November 2026 (draft, not sent)

## Email

Subject: Braze tests, 3-9 Nov: Variant B is ahead of Control but not a winner, retest before any rollout

Hi,

Here is the recap of last week's two Braze tests (emails sent Tuesday 3 Nov at 17:00, results counted for 7 days, 3 to 9 Nov).

**The result.** In the B2C subject line test, Variant B ("Rescue tonight's dinner for €4.50") got 12% more Surprise Bag purchases than Control. The data team's report says this is significant at 95% but not at our 98% rule, so Variant B is not a winner. The recommendation is to retest and not roll out. The lift is not the same everywhere: DE +12.3% (not significant, p 0.18), FR +17.2% (not significant, p 0.053), NL -0.7% (flat, p 0.96). Overall: +12% (p 0.036).

**B2C subject line test (cmp_b2c_2645, DE, FR, NL).** Rates below are purchases per delivered email.
- Control: 637 purchases from 106,798 delivered = 0.60%.
- Variant A ("Only 3 dinner bags left near you"): 847 purchases from 106,796 delivered = 0.79%. That is +33.0% against Control (DE +34.7%, FR +37.7%, NL +18.5%). Variant A is ahead in all three markets, but the report does not cover Variant A, so no significance test exists for it and it can only be called ahead.
- Variant B: 725 purchases from 108,518 delivered = 0.67%, +12.0% against Control (DE 279 vs 254, FR 331 vs 268, NL 115 vs 115).
- Opens: Control 43.9%, Variant A 44.9%, Variant B 48.2% of delivered. These include machine opens (about 47% of all opens in each variant), so they say little about real interest and we don't judge on them.
- Clicks per delivered: Control 3.12%, Variant A 3.67%, Variant B 3.24%. Unsubscribes: 162, 167 and 176 (0.15% to 0.16% each).

**B2B test, second pickup window (cmp_b2b_0871, DE, FR, NL).** Rates are stores adding a second window per delivered email.
- Control: 178 stores from 8,248 delivered = 2.16%. Variant A (earnings angle): 188 stores from 8,101 delivered = 2.32%, +7.5% against Control.
- It is not even across markets: NL 46 vs 26 stores (3.23% vs 1.78%), but DE 68 vs 72 (2.18% vs 2.31%) and FR 74 vs 80 (2.08% vs 2.18%) are slightly behind Control. The overall lead comes from NL, where the groups are small (about 1,400 stores each).
- Stores expect to list 378 extra bags a day under Variant A and 357 under Control (about 2 per store in both). No significance test was provided for this test, so Variant A is ahead, not proven better.

**Do the sources agree?** Braze conversions match the other files. B2C: 2,209 purchase rows in the transactions file equals 637 + 847 + 725 Braze purchases (the total only; I did not count rows per variant). B2B: 366 partner action rows equals 178 + 188 Braze conversions, and the per-day and per-variant counts match too. Revenue is left out of this recap: Braze's revenue counts refunded orders and the analysis report gives no revenue figure, so there is no agreed number to show.

**What to watch.**
- One week only, one send. Markets differ (NL is flat for Variant B, FR is the strongest), so don't read the overall number as the same everywhere.
- Retest Variant B before any rollout. Consider asking the data team to run the same significance test for Variant A (B2C) and for the B2B test.
- Open rates include machine opens, so keep judging on purchases.

## Slack version

*Braze tests, 3-9 Nov (one week, drafts only)*
- B2C subject lines, purchases (rate per delivered): Control 637 (0.60%), Variant A 847 (0.79%, +33.0%), Variant B 725 (0.67%, +12.0%).
- Variant B vs Control by market: DE +12.3% (p 0.18), FR +17.2% (p 0.053), NL -0.7% (flat); overall +12% (p 0.036) is significant at 95% but not at 98%, so B is ahead but not proven: retest, don't roll out. Markets differ.
- Variant A is ahead in all 3 markets but has no significance test yet, so it is ahead only. Opens include machine opens (~47%), so we don't judge on them.
- B2B second pickup window: Variant A 188 stores (2.32%) vs Control 178 (2.16%), +7.5%; NL 46 vs 26, DE 68 vs 72, FR 74 vs 80. Stores expect 378 extra bags a day (A) vs 357 (Control). Not tested, so ahead only.
- Purchase and store counts match the transaction and partner rows (totals for B2C, by variant for B2B). Revenue left out: Braze counts refunded orders and the report has no revenue figure.
