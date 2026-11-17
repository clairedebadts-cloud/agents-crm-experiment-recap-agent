# Draft: weekly Braze test recap, 3-9 Nov 2026 (not sent, for approval)

Source: data/sample/ (synthetic sample data) and the data team's analysis report. Rates are against deliveries, not sends.

## Email

**Subject: Braze test recap, 3-9 Nov: "Only 3 dinner bags left" is ahead, the store ask needs a retest**

Hi,

**The result in short.** In the subject line test, Variant A ("Only 3 dinner bags left near you") is ahead of Control: 847 purchases against 637, which is +33%. No test is a winner: this is one week of data and no significance test was run. Both tests need a retest before anyone rolls anything out.

**B2C subject line test (Winter dinner bags, DE, FR, NL).** Deliveries were 106,798 for Control, 106,796 for Variant A and 108,518 for Variant B.

| | Control | Variant A | Variant B |
|---|---|---|---|
| Purchases | 637 | 847 | 725 |
| Purchase rate (of deliveries) | 0.60% | 0.79% | 0.67% |
| Revenue (EUR, before refunds) | 3,839.46 | 5,028.24 | 4,245.38 |
| Revenue per delivery (EUR) | 0.036 | 0.047 | 0.039 |
| Unique opens (of deliveries) | 43.9% | 44.9% | 48.2% |

Against Control, Variant A has +33% purchases and +31% revenue per delivery. Variant B has +12% purchases and +9% revenue per delivery. Variant B has the most opens, but about 47% of opens in every variant are machine opens (Apple Mail Privacy Protection), so opens do not decide this test. The markets differ: purchase lifts for A are +35% in DE, +38% in FR and +19% in NL. B is +12% in DE and +17% in FR, and level with Control in NL (-1%). NL is the smallest market (about 18,500 deliveries per variant), so it moves the most on a few purchases. Revenue is before refunds, and the sources show no difference to explain here.

**B2B second pickup window test (partner stores, DE, FR, NL).** Deliveries were 8,248 for Control and 8,101 for Variant A ("Stores like yours sell 2 more bags a day with an evening slot").

| | Control | Variant A |
|---|---|---|
| Windows added | 178 | 188 |
| Rate (of deliveries) | 2.16% | 2.32% |
| Clicks (of deliveries) | 5.78% | 7.58% |
| Expected extra bags per day | 357 | 378 |

Variant A has +31% clicks and +8% windows added. The conversion gap is small: 10 more stores. By market, A is behind Control in DE (68 against 72) and FR (74 against 80) and ahead only in NL (46 against 26), so the small lead comes from the smallest market. The extra bags per day are what stores expect to list, not bags sold. Variant A is expected to add 21 more bags a day than Control (+6%).

**Checks.** Braze purchases match the transactions file: 2,209 rows against 637 + 847 + 725 = 2,209. Braze windows added match the partner actions file: 366 rows against 178 + 188 = 366. I matched row counts only. I did not re-add the revenue in the transactions file or the expected extra bags per variant, so those two figures come from the analysis report. I did not total the refunded orders either.

**What to watch.**
- One week only, and no significance test was run. Variant A is ahead, not a winner. Retest before rolling out.
- Opens include machine opens, so don't pick on opens.
- Markets differ, in both tests. NL is small and behaves differently from DE and FR.
- B2B: more clicks did not turn into many more windows, and DE and FR were behind Control.

(Nothing is sent. This is a draft for you to read and approve.)

## Slack version

**Braze tests, 3-9 Nov (1 week, no significance test, nothing is a winner)**
- B2C subject lines: Variant A is ahead with 847 purchases against Control 637 (+33%, revenue per delivery +31%, 5,028.24 EUR against 3,839.46 before refunds); Variant B 725 (+12%, +9%, 4,245.38 EUR).
- B2C by market: A is ahead in DE +35%, FR +38%, NL +19%; B is DE +12%, FR +17%, NL -1%. Markets differ and NL is small. B's top opens (48.2%) include about 47% machine opens.
- B2B second pickup window: Variant A 188 windows against Control 178 (+8%), clicks +31% (7.58% against 5.78%). A is behind in DE and FR and ahead only in NL.
- B2B stores expect 378 extra bags a day (A) against 357 (Control), which is what they expect to list, not sold.
- Next: retest before any rollout. Purchase and window counts match the transaction and partner files by row count only.
