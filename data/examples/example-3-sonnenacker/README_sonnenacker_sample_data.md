# Sonnenacker Farm Shops sample data (invented)

Made-up data for testing a CRM recap agent. Sonnenacker is an invented company. It is not real Braze data.

Week covered: send on Tuesday 20 October 2026 at 17:00, then 7 days of attribution (20 to 26 October).
Markets: DE, AT.

## Campaigns

| campaign_id | Segment | Test | Variants |
|---|---|---|---|
| cmp_b2b_1204 | B2B (partner stores) | Surplus alert reminder to partner stores | Control, Variant A (shorter subject line) |

## Files

**sonnenacker_braze_campaign_daily.csv**: one row per date, campaign, market and variant, the way a Braze campaign analytics export looks.
- sends, deliveries, hard_bounces, soft_bounces: only on the send day (20 Oct), 0 after that
- unique_opens: all unique opens, including machine opens
- machine_opens: opens triggered by Apple Mail Privacy Protection (part of unique_opens, not on top of it)
- unique_clicks, unsubscribes, spam_reports: new events on that day
- primary_conversions: B2B = a store adds a second pickup window
- revenue_eur: B2C only. Always 0 for B2B

**sonnenacker_transactions.csv**: one row per B2C purchase attributed to the email. No B2C campaign this week, so it only has the header row.

**sonnenacker_partner_actions.csv**: one row per B2B conversion. extra_bags_per_day is what the store expects to list in the new slot.

## Totals that must reconcile
- Rows in sonnenacker_transactions.csv = sum of primary_conversions for B2C
- Sum of amount_eur = sum of revenue_eur
- Rows in sonnenacker_partner_actions.csv = sum of primary_conversions for B2B
