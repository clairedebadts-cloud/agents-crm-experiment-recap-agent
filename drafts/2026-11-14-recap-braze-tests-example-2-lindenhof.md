# Draft: Braze tests recap, 13-19 Oct 2026, Lindenhof example (not sent)

Source: data/examples/example-2-lindenhof/ (3 CSVs and the README). Invented data. Rates are against deliveries. Week = send on Tue 13 Oct, plus 7 days of results. No analysis report was in data/, so the numbers could not be checked against one.

## Email

Subject: Braze tests, week of 13 Oct: Variant B ahead, but Braze and the transactions file don't match

Hi,

Here is the recap of last week's Braze test. Please read the first point before using the numbers.

**Heads-up: the two sources disagree.** Braze reports 190 purchases and 961.80 EUR. The transactions file has 184 rows and 924.00 EUR. 6 purchases and 37.80 EUR are missing from it: 2 for Control, 1 for Variant A, 3 for Variant B. All figures below are from Braze, so treat them as provisional.

**Result: Variant B is ahead, by a small margin. Nothing is called a winner: there is no analysis report and no significance test, and it is one week of data.**

**B2C subject line test (Evening soup bags, DE)**
Purchases from Braze: Variant B 70 (0.74% of delivered emails), Variant A 64 (0.68%), Control 56 (0.60%). Variant B is 24% above Control and Variant A is 14% above.
Revenue from Braze: Variant B 352.80 EUR, Variant A 327.60 EUR, Control 281.40 EUR. Revenue per delivered email was 0.037 EUR, 0.035 EUR and 0.030 EUR. Revenue includes refunded orders.
Clicks: 3.49% for B, 3.31% for A, 3.10% for Control. Open rates were 43.0%, 44.0% and 40.0%. Opens include machine opens, so we don't judge on them. Unsubscribes were 6, 8 and 7.

**What to watch**
- Fix the 6 missing purchases first. The gaps between variants are small (56, 64 and 70), so the order could change.
- One week, no significance test.
- The data is invented, per its README.

## Slack

*Braze tests, 13-19 Oct: B ahead, but the sources don't match*
- Braze says 190 purchases and 961.80 EUR. The transactions file has 184 rows and 924.00 EUR. 6 are missing.
- By Braze: B had 70 purchases (0.74%), A 64 (0.68%), Control 56 (0.60%). B +24%, A +14%.
- Braze revenue (includes refunds): B 352.80 EUR, A 327.60 EUR, Control 281.40 EUR.
- The gaps are small, so treat them as provisional. One week, no significance test, no analysis report.
