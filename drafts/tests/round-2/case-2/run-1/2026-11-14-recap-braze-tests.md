# Braze test recap, week of 27 Oct to 2 Nov 2026 (DRAFT, not sent)

## Email

**To:** (you approve first)
**Subject:** Braze test recap: "Only 4 veg bags left" is ahead of the control, but it is one week

Hi,

The "Only 4 veg bags left near you" subject line (Variant A) is ahead of the control, "Harvest veg bags near you". More people bought a Surprise Bag: 26 purchases against 20. It is not a winner: the data team ran no significance test, and this is one week of data, so it could still be chance.

**B2C subject line test, Harvest veg bags (DE, app users, sent Tue 27 Oct, 7 days of results)**
Both versions went to 4,000 people. 3,940 emails arrived for Control and 3,945 for Variant A. All rates below are against those delivered emails.
- Purchases: Control 20 (0.51% of delivered), Variant A 26 (0.66%). That is 30% more purchases for Variant A.
- Revenue, refunded orders left out: Control 99.00 EUR, Variant A 126.00 EUR, together 225.00 EUR. Per delivered email that is 0.025 EUR for Control and 0.032 EUR for Variant A, 27% more for Variant A.
- Refunded orders: Control 2 (9.00 EUR), Variant A 3 (18.00 EUR). Braze shows 252.00 EUR because it counts these 5 refunded orders (27.00 EUR). We use 225.00 EUR, the data team's number.
- Clicks: Control 120 (3.0%), Variant A 151 (3.8%).
- Opens: Control 1,660 (42.1%), Variant A 1,750 (44.4%). These include machine opens (Apple Mail Privacy Protection opens, not real people): 775 for Control and 819 for Variant A. We do not judge the subject lines on opens.
- Unsubscribes: 2 for each. Spam reports: 0 for each.

**Checks:** Braze purchases (20 and 26) match the 46 rows in the transactions file, and Braze revenue (108.00 and 144.00 EUR, 252.00 in total) matches the transactions file. All numbers match the data team's report.

**B2B:** no B2B campaign this week. The partner actions file is empty, so there are no expected extra bags to report.

**What to watch**
- One week, one market (DE), and a small number of purchases (46 in total). A gap of 6 purchases is easy to get by chance. Repeating the test would tell us more.
- No significance test was run, so we cannot call a winner.
- Refunds were higher for Variant A (3 of 26 orders, against 2 of 20). Check whether the scarcity subject line brings more regretted orders.

## Slack

*Braze test, 27 Oct to 2 Nov (DE, B2C subject line, harvest veg bags)*
- Variant A ("Only 4 veg bags left") is ahead of Control: 26 purchases against 20 (0.66% vs 0.51% of delivered), a lift of +30%.
- Revenue without refunds: 126.00 EUR vs 99.00 EUR, 225.00 EUR in total (0.032 vs 0.025 EUR per delivered email, +27%). Braze shows 252.00 EUR because it counts 5 refunded orders (27.00 EUR).
- Opens are 44.4% vs 42.1% but include machine opens, so we don't judge on them. Clicks 3.8% vs 3.0%. Unsubscribes 2 vs 2.
- No B2B test this week, so no expected extra bags.
- One week, no significance test, only 46 purchases: not proven, so repeat before we rely on it.
