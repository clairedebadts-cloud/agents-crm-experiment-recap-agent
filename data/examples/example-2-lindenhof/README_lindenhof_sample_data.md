# Lindenhof Kitchens sample data (invented)

Made-up data for testing a CRM recap agent. Lindenhof is an invented company. It is not real Braze data.

Week covered: send on Tuesday 13 October 2026 at 17:00, then 7 days of attribution (13 to 19 October).
Markets: DE.

## Campaigns

| campaign_id | Segment | Test | Variants |
|---|---|---|---|
| cmp_b2c_3208 | B2C (app users) | Subject line test, Evening soup bags | Control, Variant A (price), Variant B (scarcity) |

## Files

**lindenhof_braze_campaign_daily.csv**: one row per date, campaign, market and variant, the way a Braze campaign analytics export looks.
- sends, deliveries, hard_bounces, soft_bounces: only on the send day (13 Oct), 0 after that
- unique_opens: all unique opens, including machine opens
- machine_opens: opens triggered by Apple Mail Privacy Protection (part of unique_opens, not on top of it)
- unique_clicks, unsubscribes, spam_reports: new events on that day
- primary_conversions: B2C = a Surprise Bag purchase
- revenue_eur: B2C only, the sum of amount_eur in lindenhof_transactions.csv for that day

**lindenhof_transactions.csv**: one row per B2C purchase attributed to the email. Includes bags, unit_price_eur, amount_eur, store_type, platform, first_purchase and refunded. Revenue in the daily file includes refunded orders (refunded = True).

**lindenhof_partner_actions.csv**: one row per B2B conversion. No B2B campaign this week, so it only has the header row.

## Totals that must reconcile
- Rows in lindenhof_transactions.csv = sum of primary_conversions for B2C
- Sum of amount_eur = sum of revenue_eur
- Rows in lindenhof_partner_actions.csv = sum of primary_conversions for B2B
