# Draft: weekly recap of the Braze tests (week of 3-9 Nov 2026)

Status: draft for approval. Nothing is sent.

## Email

Subject: Braze test recap, 3-9 Nov: Variant A is ahead in both tests, but not a winner yet

Hi,

**The result:** In the shopper email (B2C), the "Only 3 dinner bags left near you" subject (Variant A) is ahead of Control. In the store email (B2B), the "earnings" message (Variant A) is only slightly ahead, and only because of the Netherlands. This is one week of data and no significance test was run, so Variant A is ahead but not a winner. The next step is to retest, not to roll out.

All rates are against deliveries (emails that arrived), not sends. Conversions are purchases (B2C) or second pickup windows added (B2B). Lift is a variant's rate against Control's. Data: send on Tue 3 Nov at 17:00, then 7 days of attribution (3-9 Nov), markets DE, FR and NL together.

**B2C subject line test (Winter dinner bags, DE + FR + NL)**
- Control ("New Surprise Bags near you tonight"): 637 purchases from 106,798 deliveries = 0.60%. Revenue EUR 3,839.46, or EUR 0.036 per delivery.
- Variant A ("Only 3 dinner bags left near you"): 847 purchases from 106,796 deliveries = 0.79%. Revenue EUR 5,028.24, or EUR 0.047 per delivery. That is +33% purchases and +31% revenue per delivery against Control.
- Variant B ("Rescue tonight's dinner for EUR 4.50", with emoji): 725 purchases from 108,518 deliveries = 0.67%. Revenue EUR 4,245.38, or EUR 0.039 per delivery. That is +12% purchases and +9% revenue per delivery against Control.
- Revenue is before refunds, so it includes orders that were later refunded. I have not counted how many were refunded.
- By market, Variant A is ahead of Control in all three: DE 0.81% vs 0.60% (+35%), FR 0.80% vs 0.58% (+38%), NL 0.74% vs 0.63% (+18%). Variant B is ahead in DE (0.68%, +12%) and FR (0.68%, +17%) but level with Control in NL (0.62%, -1%). The markets differ in size (NL is about a sixth of deliveries), so the NL numbers are the least certain.
- Opens: Control 43.9%, Variant A 44.9%, Variant B 48.2% of deliveries. These are unique opens and include machine opens (Apple Mail Privacy Protection), which are about 47% of opens in every variant. Variant B's higher open rate did not turn into more purchases than A, and opens alone do not decide the test.

**B2B second pickup window test (partner stores, DE + FR + NL)**
- Control ("Add a second pickup window to your store"): 178 windows added from 8,248 deliveries = 2.16%. Stores expect about 357 extra bags a day.
- Variant A ("Stores like yours sell 2 more bags a day with an evening slot"): 188 windows added from 8,101 deliveries = 2.32%. Stores expect about 378 extra bags a day. That is +8% windows added against Control, which is a small gap. Clicks are higher: 7.58% vs 5.78% of deliveries (+31%).
- Extra bags per day are what stores expect to list, not bags sold.
- By market the picture is mixed. Variant A is behind Control in DE (2.18% vs 2.31%, -6%) and FR (2.08% vs 2.18%, -5%), and well ahead in NL (3.23% vs 1.78%, +82%, from 46 vs 26 windows). The whole overall gap comes from NL, a small market, so treat it with care.

**Do the sources agree?**
- B2C purchases: Braze shows 2,209 purchases in total, and sample_transactions.csv has 2,209 rows. They match.
- B2B windows: Braze shows 366 windows added (178 + 188), and sample_partner_actions.csv has 366 rows. They match.
- Revenue and extra bags: the figures above are Braze's daily revenue added up by variant and market, which agree with the analysis report. I did not add up amount_eur row by row in the transactions file, and I did not add up extra_bags_per_day row by row in the partner file, so those two sums are not independently confirmed.
- The analysis report and the Braze file agree on every number I compared.

**What to watch**
- One week only, and no significance test was run. A is ahead and B is behind A, but Variant A is not a winner in either test.
- Retest the Variant A subject line before rolling it out. The B2C lift is similar in DE and FR and smaller in NL.
- Retest the B2B message before rolling it out: the +8% gap is small, and A is behind Control in DE and FR.
- Check refunds on the B2C purchases, since revenue here is before refunds.

This is a draft for you to read and approve. I have not sent it.

## Slack version

**Braze tests 3-9 Nov: A is ahead in both, not confirmed**
- B2C subject test (DE+FR+NL, rates vs deliveries): purchases Control 637, A 847 (0.79% vs 0.60%, +33%; revenue per delivery +31%), B 725 (+12%). Revenue before refunds: EUR 3,839.46 / 5,028.24 / 4,245.38. A is ahead in all 3 markets; B is level with Control in NL.
- Opens (incl. machine opens, about 47%) are higher for B at 48.2% vs 43.9% Control, but this does not decide the test.
- B2B second pickup window: Control 178 windows (2.16%), A 188 (2.32%), +8%, a small gap. Stores expect 357 vs 378 extra bags a day (not bags sold). A is behind in DE (-6%) and FR (-5%), ahead only in NL (+82%, small numbers).
- Purchase counts (2,209) and window counts (366) match the transaction and partner files. Revenue and extra-bag sums were not re-added row by row.
- One week, no significance test, markets differ: A is ahead, nothing confirmed. Retest before rolling out.
