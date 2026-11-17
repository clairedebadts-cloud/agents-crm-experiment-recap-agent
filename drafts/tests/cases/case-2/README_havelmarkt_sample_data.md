# Havelmarkt Greens sample data (invented)

Made-up data for testing a CRM recap agent. Havelmarkt is an invented company. It is not real Braze data.

Week covered: send on Tuesday 27 October 2026 at 17:00, then 7 days of attribution (27 October to 2 November).
Markets: DE.

## Campaigns

| campaign_id | Segment | Test | Variants |
|---|---|---|---|
| cmp_b2c_6602 | B2C (app users) | Subject line test, Harvest veg bags | Control, Variant A (scarcity) |

## Files

**havelmarkt_braze_campaign_daily.csv**: one row per date, campaign, market and variant, the way a Braze campaign analytics export looks.
- sends, deliveries, hard_bounces, soft_bounces: only on the send day (27 Oct), 0 after that
- unique_opens: all unique opens, including machine opens
- machine_opens: opens triggered by Apple Mail Privacy Protection (part of unique_opens, not on top of it)
- unique_clicks, unsubscribes, spam_reports: new events on that day
- primary_conversions: B2C = a Surprise Bag purchase
- revenue_eur: B2C only, the sum of amount_eur in havelmarkt_transactions.csv for that day

**havelmarkt_transactions.csv**: one row per B2C purchase attributed to the email. Includes bags, unit_price_eur, amount_eur, store_type, platform, first_purchase and refunded. Revenue in the daily file includes refunded orders (refunded = True).

**havelmarkt_partner_actions.csv**: one row per B2B conversion. No B2B campaign this week, so it only has the header row.

## Totals that must reconcile
- Rows in havelmarkt_transactions.csv = sum of primary_conversions for B2C
- Sum of amount_eur = sum of revenue_eur
- Rows in havelmarkt_partner_actions.csv = sum of primary_conversions for B2B
