# Braze test recap, week of 10 to 16 Nov 2026 (DRAFT, nothing sent)

## Email

Subject: Braze test recap: cold-weather lunch bags subject line test (B2C, DE)

Hi,

Result first: Variant A is ahead of Control on every measure, but this is one week with no significance test, so it is not a winner. Treat it as a lead, not a result.

**Cold-weather lunch bags, subject line test (B2C, Germany, sent 10 Nov, 5,000 sends per variant)**
Variant A had 30 purchases from 4,928 delivered emails (0.61%). Control had 24 from 4,930 (0.49%). That is a lift of about 25% against Control, or 6 more purchases. Clicks were 180 for Variant A (3.65%) and 150 for Control (3.04%), a lift of about 20%. Unique opens were 2,240 (45.5%) against 2,100 (42.6%). Unique opens include machine opens (964 for Variant A, 910 for Control), so we do not judge the test on opens. All rates are against deliveries, not sends. Unsubscribes were 3 for each variant, with no spam reports. Hard bounces were 22 for Variant A and 20 for Control.

**What the data can't tell us**
- It is one week and one market (B2C, DE). No significance test was run and there is no analysis report, so we cannot say the gap is more than chance. With 24 against 30 purchases, it easily could be.
- Revenue is empty in the Braze file, so there are no revenue figures and no expected extra bags.
- The purchase counts are not confirmed. The partner actions file has headers but no rows, and there is no transactions file, so Braze conversions could not be checked against transaction or partner action rows.
- The subject line text is blank for Variant A, so we cannot say what was tested against "Lunch bags are back near you".
- The file has rows dated 15 and 16 Nov, which is after today (14 Nov). These rows are included in the totals above. They need checking before anyone relies on the numbers.

**What to watch**
- Rerun the test, or let it run longer, before changing anything. Do not roll out Variant A yet.
- Get the transactions and partner action rows so the purchase counts can be confirmed.
- Get the Variant A subject line and an analysis report with significance.

## Slack

Braze recap, lunch bags subject line test (B2C, DE, 10 to 16 Nov):
- Variant A is ahead, but not a winner: 30 purchases (0.61%) vs Control 24 (0.49%), about +25% lift. Rates are against deliveries (4,928 vs 4,930).
- Clicks: 180 (3.65%) vs 150 (3.04%), about +20%. Opens 2,240 vs 2,100 include machine opens, so ignore them for the call. Unsubscribes 3 vs 3.
- One week, one market, no significance test or analysis report. No revenue in the file, so no expected extra bags.
- Purchases not confirmed: no transactions file, partner actions file is empty. Also, rows dated 15 and 16 Nov are in the future and need checking.
- Next: retest and get the missing files, don't roll out yet.
