# Draft: Braze tests recap, 3-9 Nov 2026 (not sent)

Source: data/sample/ (3 CSVs and the README). Rates are against deliveries. Week = send on Tue 3 Nov, plus 7 days of results. No analysis report was in data/, so the numbers could not be checked against one.

## Email

Subject: Braze tests, week of 3 Nov: Variant A is ahead in both tests

Hi,

Here is the recap of last week's two Braze tests.

**Result: Variant A is ahead in both tests. Nothing is called a winner: there is no analysis report and no significance test, and it is one week of data.**

**B2C subject line test (Winter dinner bags, DE, FR, NL)**
Variant A, "Only 3 dinner bags left near you", had 847 purchases (0.79% of delivered emails). Control had 637 (0.60%) and Variant B had 725 (0.67%). That is 33% more purchases for Variant A than Control, and 12% more for Variant B.
Revenue was 5,028.24 EUR for Variant A, 3,839.46 EUR for Control and 4,245.38 EUR for Variant B. This is before refunds: Braze counts refunded orders (20 for Control, 13 for Variant A, 6 for Variant B). Revenue per delivered email was 0.047 EUR, 0.036 EUR and 0.039 EUR.
Variant B had the most opens (48.2%, against 44.9% for A and 43.9% for Control). Opens include machine opens, about 47% of them, so they don't decide the test. Clicks were 3.67% for A, 3.12% for Control and 3.24% for B.

**B2B second pickup window test (partner stores, DE, FR, NL)**
Variant A, "Stores like yours sell 2 more bags a day with an evening slot", got 7.58% clicks against 5.78% for Control, 31% more. Stores added a second pickup window 188 times against 178: 2.32% against 2.16%, a small gap. Stores expect about 378 extra bags a day from Variant A and 357 from Control. Those are expected bags, not bags sold.

**What to watch**
- One week, no significance test. The B2B gap (188 against 178) could be chance.
- The README says this is synthetic sample data, not real Braze data.
- Braze purchases match the transactions file (2,209 rows) and the windows added match the partner actions file (366 rows).

## Slack

*Braze tests, 3-9 Nov: Variant A ahead in both*
- B2C subject line: A had 847 purchases (0.79%) vs 637 for Control (0.60%) and 725 for B (0.67%). A +33%, B +12%.
- B2C revenue before refunds: A 5,028.24 EUR, Control 3,839.46 EUR, B 4,245.38 EUR.
- B2B second window: A had 188 stores add a window vs 178 (+8%). Clicks 7.58% vs 5.78% (+31%). Stores expect 378 extra bags a day (A) vs 357.
- B had the most opens (48.2%), but opens include about 47% machine opens.
- One week, no significance test, no analysis report to check against.
