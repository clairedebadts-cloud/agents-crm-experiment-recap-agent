# Draft: Braze tests recap, 6-12 Oct 2026, Kornblume example (not sent)

Source: data/examples/example-1-kornblume/ (3 CSVs and the README). Invented data. Rates are against deliveries. Week = send on Tue 6 Oct, plus 7 days of results. No analysis report was in data/, so the numbers could not be checked against one.

## Email

Subject: Braze tests, week of 6 Oct: Variant A is ahead in both tests

Hi,

Here is the recap of last week's two Braze tests.

**Result: Variant A is ahead in both tests, and the B2C gap is large. Nothing is called a winner: there is no analysis report and no significance test, and it is one week of data.**

**B2C subject line test (Autumn bread bags, DE and NL)**
Variant A, "Last 2 bread bags near you", had 150 purchases (0.85% of delivered emails). Control, "Fresh bread bags near you today", had 88 (0.50%). That is 70% more purchases for Variant A.
Revenue was 817.20 EUR for Variant A and 464.80 EUR for Control, before refunds (3 refunded orders for Variant A, none for Control). Revenue per delivered email was 0.046 EUR against 0.026 EUR, 76% more.
Clicks were 3.78% against 3.00% (+26%). Open rates were 42.0% and 41.0%. Opens include machine opens, so they say little. Unsubscribes were 12 and 8, both very low.

**B2B weekend pickup window test (partner stores, DE and NL)**
Variant A, "Stores like yours add 3 bags on Saturdays", got 6.97% clicks against 5.66% for Control (+23%). Stores added a weekend window 36 times against 28: 2.61% against 2.03%. Stores expect about 77 extra bags a day from Variant A and 59 from Control, expected and not sold.

**What to watch**
- One week, no significance test. The B2B gap (36 against 28) is small and could be chance.
- The data is invented, per its README.
- Braze purchases match the transactions file (238 rows) and windows added match the partner actions file (64 rows).

## Slack

*Braze tests, 6-12 Oct: Variant A ahead in both*
- B2C subject line: A had 150 purchases (0.85%) vs 88 for Control (0.50%), +70%. Revenue before refunds 817.20 EUR vs 464.80 EUR.
- B2B weekend window: A had 36 stores add a window vs 28 (+29%). Clicks 6.97% vs 5.66% (+23%). Stores expect 77 extra bags a day (A) vs 59.
- Opens (42.0% vs 41.0%) include machine opens, so we don't judge on them.
- One week, no significance test, no analysis report to check against.
