# Draft: Braze test recap, week of 17-23 Nov 2026 (for approval, nothing sent)

## Email

Subject: Braze test recap: subject line test, Winter dinner bags (17-23 Nov)

Hi,

Result first: Variant A ("Only 3 dinner bags left near you") is ahead of Control ("Fresh dinner bags near you tonight") overall, but it is not a winner. Overall it got 130 Surprise Bag purchases against Control's 100, a lift of +30% (0.88% against 0.68% of delivered emails). The data team's report says this is significant at 95% but not at 98%, which is our bar. The three markets also disagree, so we should not roll it out.

Subject line test (campaign cmp_b2c_7703, B2C app users, DE, FR, NL). Each variant was delivered to 14,700 people (4,900 per market). Rates below are purchases per delivered email.
- Overall: Control 100 purchases (0.68%), Variant A 130 (0.88%). Lift +30%. Ahead, not a winner.
- DE: Control 20 (0.41%), Variant A 60 (1.22%). Lift +200%. Variant A clearly ahead.
- FR: Control 50 (1.02%), Variant A 40 (0.82%). Lift -20%. Variant A behind, not significant on its own.
- NL: Control 30 (0.61%), Variant A 30 (0.61%). Lift 0%. Flat.
- Revenue (EUR): Control 477.50, Variant A 607.60 (+27%). No orders were refunded, so Braze and the data team's figures are the same.
- Opens and clicks: Control 6,150 unique opens (41.8%), Variant A 6,300 (42.9%). These include machine opens (Apple Mail Privacy Protection: 2,760 for Control, 2,820 for Variant A), so opens alone say little. Clicks: Control 441 (3.0%), Variant A 450 (3.1%). Unsubscribes: 6 each. Spam reports: 0.
- The whole overall gain comes from DE (+40 purchases). FR is 10 purchases lower and NL is level.
- Check on the numbers: Braze shows 230 conversions (100 + 130). The transactions file has 230 purchase rows, and the per-market and per-variant counts match. Braze revenue matches the transaction sums. There was no B2B campaign, and the partner actions file is empty, which fits.

What to watch:
- This is one week of data. The data team ran a significance test on the overall result only. The markets are not tested separately beyond what the report says.
- Do not roll out. Keep testing. The report suggests a follow-up test in DE, where Variant A did best.
- Expected extra bags per week: not in the files, so I have not estimated it. This week Variant A had 30 more purchases (30 more bags, one bag per purchase) than Control.

## Slack

Braze test recap, 17-23 Nov (subject line test, Winter dinner bags, DE/FR/NL):
- Variant A ("Only 3 bags left") is ahead overall, but not strong enough to roll out: 130 purchases vs Control 100 (0.88% vs 0.68%, +30%). Significant at 95%, not at the 98% bar. Revenue EUR 607.60 vs 477.50.
- By market: DE 60 vs 20 (+200%, clearly ahead), FR 40 vs 50 (-20%, behind, not significant), NL 30 vs 30 (flat).
- Opens are about level (42.9% vs 41.8%) and include machine opens. Braze and transaction counts match (230).
- Do not roll out. Keep testing, maybe a follow-up in DE. One week only. No expected extra bags figure in the files; this week Variant A sold 30 more bags.
