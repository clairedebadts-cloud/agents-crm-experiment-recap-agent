# Braze test recap, week of 2026-11-10 to 2026-11-16 (DRAFT, not sent)

Source: bergwind_braze_campaign_daily.csv (one test, one week). The partner actions file has headers only, so conversions could not be checked. No analysis report or README was provided.

## Email

Subject: Braze test recap: lunch bag subject line test (10-16 Nov)

Hi,

Result first: Variant A did better than Control on every measure we have, but the gap rests on very few conversions (30 vs 24), so treat it as a lead, not a proven win.

**B2C | Cold-weather lunch bags | Subject line test (DE, 5,000 sends per variant)**
All rates are against deliveries (emails that arrived), not sends.

| | Control | Variant A | Variant A vs Control |
|---|---|---|---|
| Deliveries | 4,930 | 4,928 | same |
| Unique opens | 2,100 (42.6%) | 2,240 (45.5%) | +6.7% |
| Clicks | 150 (3.04%) | 180 (3.65%) | +20.0% |
| Conversions | 24 (0.49%) | 30 (0.61%) | +25.1% |
| Unsubscribes | 3 (0.06%) | 3 (0.06%) | no difference |

- Conversions are the primary_conversions count from Braze. Variant A had 6 more than Control. Lift means Variant A's rate compared with Control's rate.
- Open rates include machine opens (automatic opens by mail software): 910 for Control and 964 for Variant A, about 43% of opens in both. Because of that, we don't call a winner on opens alone. The case for Variant A rests on clicks and conversions.
- Control's subject line was "Lunch bags are back near you". Variant A's subject line is blank in the file, so we can't say what was tested.
- No spam reports on either side. Revenue is empty in the file, so there is no revenue comparison.

**What to watch**
- This is one week and one test. No significance test was run, and 6 extra conversions out of roughly 4,900 deliveries could be chance.
- Braze conversions could not be matched to partner actions: the partner actions file has no rows, and there is no transaction file. Treat the conversion numbers as unconfirmed.
- The file has rows dated 14, 15 and 16 Nov, which is after the date of this draft (14 Nov). Please check the export date. The numbers above include those rows.
- Most activity came on day one (10 Nov) and faded each day. If the test runs again, compare like for like days.
- Before rolling out Variant A, get the Variant A subject line and revenue added to the data.

## Slack version

*Braze test recap, 10-16 Nov: lunch bag subject line test (DE)*
- Variant A beat Control on opens (45.5% vs 42.6%, includes machine opens), clicks (3.65% vs 3.04%, +20%) and conversions (0.61% vs 0.49%, +25%). Rates are against deliveries.
- That is 30 vs 24 conversions, a small gap. One week, no significance test, so not a proven win. Opens alone don't decide it.
- Unsubscribes were equal (3 each). No revenue in the file. Variant A's subject line is blank.
- Could not check conversions against partner actions (file is empty). Data includes dates after 14 Nov, worth checking.
