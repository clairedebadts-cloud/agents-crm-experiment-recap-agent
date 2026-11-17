# Braze test recap, week of 2026-11-10 to 2026-11-16 (DRAFT, not sent)

Source: bergwind_braze_campaign_daily.csv (case-4). No analysis report, README or transaction file was found. The partner actions file has a header and no rows.

## Email

**To:** (not set)
**Subject:** Braze test recap: cold-weather lunch bags subject line test

Hi,

**Result:** Variant A did better than Control on clicks and conversions, but the numbers are small and this is one week with no significance test, so treat it as a lead and not a proven win.

**B2C | Cold-weather lunch bags | Subject line test (DE, 5,000 sends per variant)**
All rates are against deliveries (emails that arrived), not sends.

| | Control | Variant A |
|---|---|---|
| Deliveries | 4,930 | 4,928 |
| Clicks (unique) | 150 (3.04%) | 180 (3.65%) |
| Conversions | 24 (0.49%) | 30 (0.61%) |
| Unique opens | 2,100 (42.6%) | 2,240 (45.5%) |
| Unsubscribes | 3 (0.06%) | 3 (0.06%) |

- Clicks: Variant A's click rate is about 20% higher than Control's (3.65% vs 3.04%).
- Conversions: Variant A's conversion rate is about 25% higher (0.61% vs 0.49%). That is 6 more conversions (30 vs 24), a small gap.
- Opens: 45.5% vs 42.6%. Open counts include machine opens (automatic opens by mail software, not people), so I am not calling a winner on opens. Machine opens were 910 for Control and 964 for Variant A. Without them, opens are 1,190 (24.1%) vs 1,276 (25.9%).
- Unsubscribes: the same, 3 each. No concern.
- Revenue: the file has no revenue figures, so there is no revenue comparison.
- Subject lines: Control was "Lunch bags are back near you". The file does not show Variant A's subject line.

**What to watch**
- Whether Variant A's lead holds in a second week. 6 extra conversions could be chance.
- Get Variant A's subject line and the revenue figures into the file.
- The conversion check could not be done (see below).

**What the data can't tell us:** one week only, no significance test run, no revenue.

**Data issues to flag**
- I could not check Braze conversions (54 in total: 24 + 30) against transaction and partner action rows. The partner actions file is empty and there is no transaction file.
- The file has rows dated 2026-11-15 and 2026-11-16, which are after the date this draft was written (2026-11-14). Please check the dates. All figures above include those rows.

## Slack version

*Braze test recap, 10-16 Nov (draft)*
- Lunch bags subject line test (DE): Variant A beat Control on clicks, 3.65% vs 3.04% (about +20%), and on conversions, 0.61% vs 0.49% (about +25%, 30 vs 24). Rates are against deliveries.
- Opens 45.5% vs 42.6% include machine opens, so no winner on opens. Unsubscribes equal at 3 each.
- Caveat: one week, no significance test, small numbers. No revenue in the file, and Variant A's subject line is missing.
- Could not check conversions against partner actions: that file is empty. Some rows are dated after today, so please check.
