# Braze test recap, week of 10 to 16 Nov 2026 (DRAFT, nothing sent)

## Email

Subject: Braze test recap: cold-weather lunch bags subject line test (DE)

Hi,

Variant A is ahead of Control on every measure, but this is not a winner. No analysis report was in the files, so no significance test was run. Treat it as a first signal and not as a result to roll out.

**Cold-weather lunch bags, subject line test (B2C, Germany only).** Each version went to 5,000 people on 10 Nov. All rates below are against deliveries (4,930 for Control, 4,928 for Variant A).
- Purchases (primary conversions): Control 24 (0.49%), Variant A 30 (0.61%). That is 6 more purchases, a lift of about 25% against Control.
- Clicks: Control 150 (3.04%), Variant A 180 (3.65%). Lift of about 20%.
- Opens: Control 2,100 (42.6%), Variant A 2,240 (45.5%). These are unique opens and they include machine opens (Control 910, Variant A 964), so they overstate real opens. We do not call a variant ahead on opens alone.
- Unsubscribes: 3 for each version (about 0.06%). No difference.
- Revenue: the file has no revenue figures, so there is none to report.
- Subject lines: Control was "Lunch bags are back near you". The file has no subject line for Variant A, so we can't say what was tested against it.

**What the data can't tell us**
- Purchase counts are not confirmed. The partner actions file has no rows and there is no transactions file, so Braze conversions could not be checked against transaction or partner action rows. Expected extra bags per day can't be given for the same reason.
- It is one week and one market (Germany). Other markets may behave differently.
- The gap is 6 purchases out of about 4,900 deliveries per version. With numbers this small it could be chance.
- The file includes rows dated 15 and 16 Nov, which is after today (14 Nov). Please check where those rows come from. The totals above include them (1 purchase each from 15 Nov, none on 16 Nov).

**What to watch**
- Get the transactions and partner actions data, so the purchase counts can be checked.
- Get the analysis report and see whether the difference is significant at 98%.
- Retest, or let the test run longer, before rolling out Variant A.

## Slack version

Braze recap, lunch bags subject line test (DE only, 10 to 16 Nov):
- Variant A is ahead, not a winner: 30 purchases vs 24 for Control (0.61% vs 0.49% of deliveries, lift about +25%). Clicks 180 vs 150 (+20%).
- Opens 45.5% vs 42.6%, but they include machine opens, so we don't lean on them. Unsubscribes 3 each.
- No analysis report, so no significance test. One week, one market, and a small gap. The file has rows dated after today (15 and 16 Nov), included in these numbers.
- Purchases can't be checked: no transactions file, partner actions file is empty. No revenue in the file, so no expected extra bags.
- Next: retest before any rollout.
