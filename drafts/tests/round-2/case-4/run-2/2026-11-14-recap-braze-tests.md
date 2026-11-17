# Braze test recap, week of 2026-11-10 to 2026-11-16 (DRAFT, not sent)

## Email

Subject: Braze test recap: cold-weather lunch bags subject line test

Hi,

Result first: Variant A is ahead of Control on every measure, but this is one week of one test and no significance test was run, so Variant A is not a winner yet. Treat it as a lead, not a result.

**B2C DE | Cold-weather lunch bags | Subject line test** (5,000 sends per variant, 10 to 16 Nov)

All rates below are against deliveries (emails that arrived), not sends.

| | Control | Variant A | Variant A vs Control |
|---|---|---|---|
| Deliveries | 4,930 | 4,928 | |
| Purchases (conversions) | 24 | 30 | +6, lift +25% |
| Conversion rate | 0.49% | 0.61% | +25% |
| Clicks | 150 | 180 | |
| Click rate | 3.04% | 3.65% | +20% |
| Opens (unique, incl. machine opens) | 2,100 | 2,240 | |
| Open rate (incl. machine opens) | 42.6% | 45.5% | +6.7% |
| Unsubscribes | 3 | 3 | same (0.06% each) |

Paragraph on the test: Variant A's subject line led to 30 purchases against 24 for Control, on almost the same number of delivered emails. That is 6 more purchases, or a lift of 25% on the conversion rate. More people clicked too (180 against 150). Open rates are higher for Variant A, but opens include machine opens (automatic opens by mail apps, about 43% of opens in both variants), so we do not judge the test on opens. Unsubscribes were equal at 3 each. Spam reports were 0 in both.

Why we are careful: the gap is 6 purchases. With numbers this small, a gap like that can happen by chance. No analysis report with a significance result was in the files, so we cannot say it is significant at 98%.

What the data can't tell us:
- Revenue: the file has no revenue figures, so we can't say how much extra money Variant A made.
- Extra bags per day: the partner actions file has no rows, so we have no expected extra bags.
- Conversion check: Braze shows 24 and 30 conversions, but with the partner actions file empty and no transaction file, we could not match them to real purchases or partner actions.
- Variant A's subject line is blank in the file, so we can't say what it was. Control's was "Lunch bags are back near you".
- Only DE (B2C) is in the data. No other market was in the files.
- The file has dates up to 16 Nov, which is after today (14 Nov). Please check the export before relying on the last days.

What to watch: whether Variant A's lead holds with more data or a repeat run, whether the analysis report shows significance at 98%, and whether the partner action and revenue data arrive so we can check the conversions.

## Slack version

*Braze test recap, 10 to 16 Nov (draft)*
- B2C DE lunch bags subject line test: Variant A is ahead of Control, but no significance test was run, so no winner call. One week only.
- Purchases: Variant A 30 vs Control 24 (+6), conversion rate 0.61% vs 0.49% (lift +25%, against deliveries 4,928 vs 4,930). Clicks 180 vs 150 (click rate 3.65% vs 3.04%, +20%).
- Opens 45.5% vs 42.6% include machine opens, so not used to judge. Unsubscribes 3 vs 3.
- Not available: revenue (none in file), expected extra bags (partner actions file is empty), so conversions could not be checked. Only DE in the data. Variant A's subject line is blank in the file.
- Watch: does the lead hold on a repeat or with more data? Dates run to 16 Nov, past today, so check the export.
