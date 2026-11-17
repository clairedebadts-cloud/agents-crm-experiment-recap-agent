# Kornblume Bakeries sample data (invented)

Made-up data for testing a CRM recap agent. Kornblume is an invented company. It is not real Braze data.

Week covered: send on Tuesday 6 October 2026 at 17:00, then 7 days of attribution (6 to 12 October).
Markets: DE, NL.

## Campaigns

| campaign_id | Segment | Test | Variants |
|---|---|---|---|
| cmp_b2c_3101 | B2C (app users) | Subject line test, Autumn bread bags | Control, Variant A (scarcity) |
| cmp_b2b_1120 | B2B (partner stores) | Ask stores to add a weekend pickup window | Control, Variant A (Saturday bags angle) |

## Files

**kornblume_braze_campaign_daily.csv**: one row per date, campaign, market and variant, the way a Braze campaign analytics export looks.
- sends, deliveries, hard_bounces, soft_bounces: only on the send day (6 Oct), 0 after that
- unique_opens: all unique opens, including machine opens
- machine_opens: opens triggered by Apple Mail Privacy Protection (part of unique_opens, not on top of it)
- unique_clicks, unsubscribes, spam_reports: new events on that day
- primary_conversions: B2C = a Surprise Bag purchase. B2B = a store adds a second pickup window
- revenue_eur: B2C only, the sum of amount_eur in kornblume_transactions.csv for that day. Always 0 for B2B

**kornblume_transactions.csv**: one row per B2C purchase attributed to the email. Includes bags, unit_price_eur, amount_eur, store_type, platform, first_purchase and refunded. Revenue in the daily file includes refunded orders (refunded = True).

**kornblume_partner_actions.csv**: one row per B2B conversion. extra_bags_per_day is what the store expects to list in the new slot.

## Totals that must reconcile
- Rows in kornblume_transactions.csv = sum of primary_conversions for B2C
- Sum of amount_eur = sum of revenue_eur
- Rows in kornblume_partner_actions.csv = sum of primary_conversions for B2B
