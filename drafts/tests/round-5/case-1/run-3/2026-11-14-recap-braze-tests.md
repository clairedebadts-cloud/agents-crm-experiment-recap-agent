# Draft: Braze test recap, week of 3-9 Nov 2026 (not sent, for approval)

Sources: data/sample/ (Braze daily export, transactions, partner actions, README) and the data team's analysis report. Rates are against deliveries. Synthetic sample data, per the README.

## Email

**Subject:** Braze tests recap, 3-9 Nov: Variant A is ahead in both tests, but nothing is proven yet

Hi,

Short version: Variant A is ahead of Control in both tests. In the bag subject line test the gap is clear in every market. In the partner store test it is small and comes from one market. We have one week of data and no significance test, so Variant A is not a winner yet. Next step: retest before rolling anything out.

**B2C subject line test, Winter dinner bags (DE, FR, NL)**
Variant A ("Only 3 dinner bags left near you") is ahead. Purchases: Control 637, Variant A 847, Variant B 725. Against deliveries that is 0.60% for Control, 0.79% for A and 0.67% for B. So A has 33% more purchases than Control and B has 12% more. Revenue per delivery: Control EUR 0.036, A EUR 0.047 (+31%), B EUR 0.039 (+9%). Revenue: Control EUR 3,839.46, A EUR 5,028.24, B EUR 4,245.38. This revenue is before refunds, so refunded orders are included. By market, A's purchase rate is ahead of Control by 35% in DE, 38% in FR and 19% in NL. B is ahead by 12% in DE and 17% in FR, and level in NL (1% behind). Variant B has the highest open rate (48.2%, against 43.9% for Control and 44.9% for A), but opens include machine opens (about 47% of unique opens in every variant), so opens alone say nothing about which subject line worked better. Deliveries were 106,798 (Control), 106,796 (A) and 108,518 (B). Unsubscribes were 162, 167 and 176.

**B2B test, ask stores to add a second pickup window (DE, FR, NL)**
Variant A (the earnings angle) is slightly ahead. Stores that added a window: Control 178, Variant A 188 (2.16% against 2.32% of deliveries, +8%). Clicks are further apart: 5.78% for Control and 7.58% for A (+31%). More clicks did not turn into many more windows. Stores say they expect to list 378 extra bags a day with A against 357 with Control. Those are expected bags, not bags sold. The markets point different ways: in NL, A is well ahead (3.23% against 1.78%), but in DE (2.18% against 2.31%) and FR (2.08% against 2.18%) it is slightly behind. The overall +8% comes from NL, and the NL group is small (1,423 and 1,462 deliveries). Unsubscribes were 4 (Control) and 5 (A).

**Checks on the numbers**
- Purchases: Braze shows 2,209 purchases (637 + 847 + 725) and the transactions file has 2,209 rows. They match. I counted rows in total, not per variant.
- Store actions: Braze shows 366 windows added (178 + 188) and the partner actions file has 366 rows. They match.
- Not done: I did not add up the amount column in the transactions file or count the refunded orders, so the revenue figures come from the analysis report and the Braze daily file, and I can't say how much of it was refunded. The expected extra bags (357 and 378) are the analysis report's figures, not re-added by me.

**What to watch**
- This is one week, one send, and no significance test was run. Treat "ahead" as a lead, not a result.
- Retest Variant A against Control in the B2C test, and check if the lead holds in NL, where it is smallest.
- For B2B, look at NL separately before deciding: the lead there is not seen in DE or FR.
- Look at purchases and revenue per delivery, not opens.

## Slack version

*Braze tests 3-9 Nov: A is ahead in both, nothing proven*
- B2C subject test: purchases Control 637, A 847, B 725 (0.60% / 0.79% / 0.67% of deliveries). A is ahead: +33% purchases, +31% revenue per delivery (EUR 0.047 vs 0.036); B +12% and +9%. Revenue before refunds: EUR 3,839.46 / 5,028.24 / 4,245.38.
- By market, A is ahead in DE +35%, FR +38%, NL +19%; B +12%, +17%, level in NL (-1%). Markets differ, read each alone. B's top open rate (48.2%) includes ~47% machine opens, so it doesn't decide.
- B2B second window: added Control 178, A 188 (2.16% vs 2.32%, +8%), clicks +31% (5.78% vs 7.58%); stores expect 378 vs 357 extra bags a day (expected, not sold). A is ahead only in NL (3.23% vs 1.78%), behind in DE and FR.
- One week, no significance test: no variant is proven. Retest, don't roll out.
- Checks: 2,209 purchases and 366 windows match the transaction and partner rows; revenue amounts and refunds not re-added by me.
