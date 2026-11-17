# Braze test recap: week of 27 Oct to 2 Nov 2026 (DRAFT, not sent)

Source: Braze export, transactions file, data team analysis report. One test this week. All rates are against deliveries (emails that arrived), not sends.

## Email

**Subject:** Braze test recap: "Only 4 veg bags left near you" beat the control on purchases

Hi,

**Result:** The scarcity subject line (Variant A) led to more purchases than the control. 26 purchases against 20, a conversion rate of 0.66% against 0.51%. That is 30% more purchases per delivered email. The numbers are small, so treat it as a promising sign, not proof.

**B2C subject line test, Harvest veg bags (DE, app users, campaign cmp_b2c_6602)**
Sent Tuesday 27 Oct at 17:00, with 7 days of purchases counted. Control ("Harvest veg bags near you") was delivered to 3,940 people and Variant A ("Only 4 veg bags left near you") to 3,945. Control had 20 purchases (0.51%). Variant A had 26 purchases (0.66%), 6 more. Revenue after taking out refunded orders was 99.00 EUR for Control and 126.00 EUR for Variant A. Per delivered email that is 0.025 EUR against 0.032 EUR, so Variant A earned 27% more per delivery.

**About the revenue number:** Braze shows 252.00 EUR in total (108.00 Control, 144.00 Variant A). That includes 5 refunded orders worth 27.00 EUR (2 for Control, 9.00 EUR; 3 for Variant A, 18.00 EUR). We use the 225.00 EUR figure without refunds, as the data team report does. The Braze purchase counts (20 and 26) include those refunded orders too, so the 0.51% and 0.66% rates do as well.

**Opens and clicks (secondary):** Unique opens were 1,660 for Control (42.1%) and 1,750 for Variant A (44.4%). These include machine opens, mostly Apple Mail Privacy Protection, which were about 47% of opens in both variants (775 and 819). So we don't call a winner on opens. Clicks: 120 for Control (3.05%) and 151 for Variant A (3.83%). Unsubscribes were 2 in each variant. No spam reports.

**Checks:** Braze purchases match the transactions file (20 and 26 rows). Braze revenue matches the transactions file (108.00 and 144.00 EUR). There was no B2B campaign, so the partner actions file is empty, as expected.

**What to watch:**
- This is one week and one send. No significance test was run, so the gap (6 purchases) could be chance.
- Scarcity wording ("only 4 left") should be true when sent. Worth checking the claim matched real stock.
- Repeat the test, or run it on another segment, before making Variant A the default.

## Slack

*Braze test recap, 27 Oct to 2 Nov (rates vs deliveries)*
- Subject line test, Harvest veg bags (DE, B2C): Variant A "Only 4 veg bags left near you" beat Control.
- Purchases: 26 vs 20. Conversion 0.66% vs 0.51% (+30%). Deliveries 3,945 vs 3,940.
- Revenue without refunds: 126.00 vs 99.00 EUR, 0.032 vs 0.025 EUR per delivery (+27%). Total 225.00 EUR. Braze shows 252.00 EUR because it counts 5 refunded orders (27.00 EUR).
- Opens (44.4% vs 42.1%) include machine opens (about 47%), so not used to pick a winner.
- Caution: one week, small numbers, no significance test.
