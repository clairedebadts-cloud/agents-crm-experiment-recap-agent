# Draft for approval: Braze test recap (nothing sent)

## Email

Subject: Braze test recap: Cold-weather lunch bags subject line test (B2C, DE)

Variant A is ahead of Control on clicks and purchases, but this is one week of data and no significance test was run, so it is not a winner.

**Cold-weather lunch bags, subject line test (B2C, Germany, sends 10 Nov, daily data 10 to 16 Nov)**
Each variant was sent to 5,000 people. Rates below are against deliveries (emails that arrived): Control 4,930, Variant A 4,928.
- Purchases (Braze conversions): Variant A 30, Control 24. That is 0.61% against 0.49% of deliveries, a lift of about 25% for Variant A. The gap is 6 purchases, which is small.
- Clicks: Variant A 180 (3.65%), Control 150 (3.04%). Lift about 20%.
- Opens: Variant A 2,240 (45.5%), Control 2,100 (42.6%). Unique opens include machine opens (automatic opens by mail apps, not people), so opens alone say little. Machine opens were 964 for Variant A and 910 for Control.
- Unsubscribes: 3 for each variant (0.06% of deliveries each). No spam reports.
- Bounces: Control 20 hard and 50 soft, Variant A 22 hard and 50 soft.

Variant A is ahead on every measure, but with so few purchases the gap could be chance. Variant A's subject line is empty in the file, so I can't say what text was tested. Control's was "Lunch bags are back near you".

**What the data can't tell**
- One week only, one market (DE), one segment (B2C). No significance test was run and no analysis report was in the files.
- Revenue is blank in the Braze file, so there is no revenue or lift in euros.
- Purchases could not be checked: there is no transactions file, and the partner actions file has a header but no rows. Nobody should take the purchase counts as confirmed. Expected extra bags per day can't be given either.
- The file has dates 14, 15 and 16 Nov, which are after today (14 Nov). Please check the export.

**What to watch**
- Retest before rolling out Variant A.
- Get the transactions file and partner actions so purchases can be checked.
- Get the variant A subject line and the analysis report.

## Slack

*Braze test recap: lunch bags subject line (B2C, DE)*
- Variant A ahead, not a winner: 30 purchases vs Control 24 (0.61% vs 0.49% of deliveries, lift about 25%). One week, no significance test.
- Clicks: A 180 (3.65%) vs Control 150 (3.04%), lift about 20%. Opens 45.5% vs 42.6%, including machine opens.
- Unsubscribes 3 each. Revenue blank, so no euro figure; expected extra bags: no data.
- Purchases not checked: no transactions file, partner actions empty. Data has dates after today.
- Next: retest, don't roll out yet.
