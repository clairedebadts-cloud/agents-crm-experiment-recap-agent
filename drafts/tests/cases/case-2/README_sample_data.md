# Sample data (synthetic)

Made-up data for testing a CRM recap agent. It is not real company or Braze data.

Week covered: send on Tuesday 3 November 2026 at 17:00, then 7 days of attribution (3 to 9 November).
Markets: DE, FR, NL.

## Campaigns

| campaign_id | Segment | Test | Variants |
|---|---|---|---|
| cmp_b2c_2645 | B2C (app users) | Subject line test, Winter dinner bags | Control, Variant A (scarcity), Variant B (emoji + price) |
| cmp_b2b_0871 | B2B (partner stores) | Ask stores to add a second pickup window | Control, Variant A (earnings angle) |

## Files

**sample_braze_campaign_daily.csv**: one row per date, campaign, market and variant, the way a Braze campaign analytics export looks.
- sends, deliveries, hard_bounces, soft_bounces: only on the send day (3 Nov), 0 after that
- unique_opens: all unique opens, including machine opens
- machine_opens: opens triggered by Apple Mail Privacy Protection (part of unique_opens, not on top of it)
- unique_clicks, unsubscribes, spam_reports: new events on that day
- primary_conversions: B2C = a Surprise Bag purchase. B2B = a store adds a second pickup window
- revenue_eur: B2C only, the sum of amount_eur in sample_transactions.csv for that day. Always 0 for B2B

**sample_transactions.csv**: one row per B2C purchase attributed to the email. Includes bags, unit_price_eur, amount_eur, store_type, platform, first_purchase and refunded. Revenue in the daily file includes refunded orders (refunded = True).

**sample_partner_actions.csv**: one row per B2B conversion. extra_bags_per_day is what the store expects to list in the new slot.

## Totals that must reconcile
- Rows in sample_transactions.csv = sum of primary_conversions for B2C
- Sum of amount_eur = sum of revenue_eur
- Rows in sample_partner_actions.csv = sum of primary_conversions for B2B
