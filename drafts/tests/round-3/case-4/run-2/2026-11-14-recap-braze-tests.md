# Braze test recap, week of 10-16 Nov 2026 (DRAFT, not sent)

## Email

Subject: Braze test recap: lunch bag subject lines, week of 10 Nov

Hi,

Result first: Variant A is ahead of Control on every rate, but this is one week, one market (B2C, DE), and no significance test or analysis report was available. Variant A is not a winner. Treat it as a lead to retest, not a reason to roll out.

**Cold-weather lunch bags, subject line test (B2C, DE, 10-16 Nov)**
Both versions went to 5,000 people. Deliveries were 4,930 for Control ("Lunch bags are back near you") and 4,928 for Variant A. The Variant A subject line is blank in the file, so I can't say what it was. All rates below are against deliveries.

| | Control | Variant A | Variant A vs Control |
|---|---|---|---|
| Deliveries | 4,930 | 4,928 | |
| Unique opens (include machine opens) | 2,100 (42.6%) | 2,240 (45.5%) | +6.7% |
| of which machine opens | 910 | 964 | |
| Clicks | 150 (3.04%) | 180 (3.65%) | +20% |
| Purchases (Braze primary conversions) | 24 (0.49%) | 30 (0.61%) | +25% |
| Unsubscribes | 3 | 3 | same |
| Revenue | not in file | not in file | |

In plain words: out of every 1,000 people reached, Control got about 4.9 purchases and Variant A about 6.1. That is 6 more purchases over about 4,900 deliveries. Opens include machine opens (automatic opens by mail software), so the open gap says little on its own, and I am not judging the variants on opens. Clicks and purchases point the same way as opens.

Expected extra bags per day: not in the data (the partner actions file has no rows), so I can't give an expectation.

**What the checks could not confirm**
- The purchase counts are Braze's own. There is no transactions file, and the partner actions file has headers only, so Braze conversions could not be matched to transaction or partner rows. Don't take the 24 and 30 as confirmed.
- No revenue figures are in the file, so there is no revenue result.
- No analysis report and no significance test were provided. The gap of 6 purchases is small and could be chance.
- The file has rows dated 15 and 16 Nov, which are after today (14 Nov). Please check the export date, as these days may be projected or mislabelled. The figures above include them: those two days add 1 purchase to each variant.

**What to watch**
- Retest before rolling out, ideally with a significance test and with the Variant A subject line recorded.
- Get the transactions and partner actions files so purchases can be checked.
- Only one market (DE) is covered; other markets may differ.

## Slack

Braze recap, 10-16 Nov, lunch bags subject test (B2C, DE, one market only):
- Variant A is ahead of Control, not a winner: no significance test or analysis report, so retest before rolling out.
- Purchases (Braze, deliveries 4,928 vs 4,930): A 30 (0.61%) vs Control 24 (0.49%), lift +25%. Clicks 180 vs 150 (+20%).
- Opens 2,240 vs 2,100 include machine opens, so not used to judge. Unsubscribes 3 vs 3. No revenue in file, no extra-bag expectation possible.
- Purchases not confirmed: no transactions file, partner actions file empty. Variant A subject line blank, and rows dated 15-16 Nov are after today, so check the export.
