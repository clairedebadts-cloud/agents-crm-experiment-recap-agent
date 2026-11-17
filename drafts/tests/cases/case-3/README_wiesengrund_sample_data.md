# Wiesengrund Foods sample data (invented)

Made-up data for testing a CRM recap agent. Wiesengrund is an invented company. It is not real Braze data.

Week covered: send on Tuesday 17 November 2026 at 17:00, then 7 days of attribution (17 to 23 November).
Markets: DE, FR, NL.

## Campaigns

| campaign_id | Segment | Test | Variants |
|---|---|---|---|
| cmp_b2c_7703 | B2C (app users) | Subject line test, Winter dinner bags | Control, Variant A (scarcity) |

## Files

**wiesengrund_braze_campaign_daily.csv**: one row per date, campaign, market and variant, the way a Braze campaign analytics export looks.
- sends, deliveries, hard_bounces, soft_bounces: only on the send day (17 Nov), 0 after that
- unique_opens: all unique opens, including machine opens
- machine_opens: opens triggered by Apple Mail Privacy Protection (part of unique_opens, not on top of it)
- unique_clicks, unsubscribes, spam_reports: new events on that day
- primary_conversions: B2C = a Surprise Bag purchase
- revenue_eur: B2C only, the sum of amount_eur in wiesengrund_transactions.csv for that day

**wiesengrund_transactions.csv**: one row per B2C purchase attributed to the email. Includes bags, unit_price_eur, amount_eur, store_type, platform, first_purchase and refunded. Revenue in the daily file includes refunded orders (refunded = True).

**wiesengrund_partner_actions.csv**: one row per B2B conversion. No B2B campaign this week, so it only has the header row.

## Totals that must reconcile
- Rows in wiesengrund_transactions.csv = sum of primary_conversions for B2C
- Sum of amount_eur = sum of revenue_eur
- Rows in wiesengrund_partner_actions.csv = sum of primary_conversions for B2B
