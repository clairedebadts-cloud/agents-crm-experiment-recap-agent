# Draft: weekly Braze test recap (week of 3-9 Nov 2026)

Status: draft for approval. Nothing has been sent.

---

## Email

**Subject:** Braze tests 3-9 Nov: Variant B ahead of Control, not a winner, retest

Hi,

**The result.** In the winter dinner bags subject line test, Variant B (emoji + price) got more bag purchases than Control, but it is not a winner. Per delivered email, 0.668% bought a bag with B against 0.597% with Control, a lift of +12%. The data team's test says that is significant at 95% but not at the 98% we require (p = 0.036). By market: DE +12.3% (not significant, p = 0.18), FR +17.2% (not significant, p = 0.053), NL -0.7% (flat, p = 0.96). The data team recommends a retest and no roll-out.

All rates below are against deliveries (emails that arrived), not sends. Lift means a variant's rate against Control's, as a percentage. Data covers one week: sent Tuesday 3 Nov at 17:00, plus 7 days of attribution (3-9 Nov), in DE, FR and NL.

**B2C: subject line test, Winter dinner bags (cmp_b2c_2645).**

| | Deliveries | Purchases | Purchases per delivery | Revenue after refunds |
|---|---|---|---|---|
| Control | 106,798 | 637 | 0.597% | EUR 3,712.33 |
| Variant A (scarcity) | 106,796 | 847 | 0.793% | EUR 4,956.08 |
| Variant B (emoji + price) | 108,518 | 725 | 0.668% | EUR 4,216.50 |

- Variant B vs Control: +12% overall; DE +12.3%, FR +17.2%, NL -0.7%. Not significant at 98%, so B is ahead, not a winner. FR looks strongest and NL shows no gain, so the markets do not behave the same way.
- Variant A vs Control: +33.0% overall, and ahead in all three markets. The analysis report only covers Variant B, so no significance test exists for A. A is ahead, nothing more can be said yet.
- Opens (these include machine opens, so they say little about real interest): Control 43.9%, A 44.9%, B 48.2% of deliveries. Do not read B's higher open rate as a result.
- Clicks: Control 3,336 (3.12% of deliveries), A 3,922 (3.67%), B 3,516 (3.24%). Unsubscribes: Control 162, A 167, B 176 (about 0.15-0.16% each).
- Revenue is after refunds. The analysis report gives no revenue figure, so I took the daily revenue in the Braze file and removed the orders marked refunded in the transactions file. Braze shows EUR 4,245.38 for Variant B because it counts refunded orders (Control and A are higher there for the same reason).

**B2B: ask stores to add a second pickup window (cmp_b2b_0871).**

| | Deliveries | Stores that added a window | Per delivery | Extra bags per day they expect |
|---|---|---|---|---|
| Control | 8,248 | 178 | 2.16% | 357 |
| Variant A (earnings angle) | 8,101 | 188 | 2.32% | 378 |

Variant A is ahead of Control by +7.5% overall, but it is behind in two of three markets: DE 68 vs 72 stores (-5.7%), FR 74 vs 80 (-4.5%), NL 46 vs 26 (+81.8%). The overall gain comes from NL, which is the smallest market (about 1,400 deliveries per variant). No significance test exists for this test, so treat A as ahead, not proven. Stores expect roughly 2 extra bags per day each in both variants.

**Checks.**
- B2C: the transactions file has 2,209 purchase rows and Braze shows 2,209 purchases in total. They match. I did not recount the rows per variant and market.
- B2B: the partner actions file has 366 rows and Braze shows 366 conversions (Control 178, Variant A 188). They match in total and per variant per day.
- Not fully checked: I did not re-add all 2,209 purchase amounts to compare with the Braze revenue total. I relied on the README, which says the daily revenue is the sum of the purchase amounts. I counted the refunded orders by hand from the file: 39 in total (Control 20, A 13, B 6). Please treat those counts as needing a second look.

**What to watch.**
- Retest Variant B before any roll-out, as the data team recommends. Ask for the retest to report DE, FR and NL separately.
- Ask the data team to test Variant A too. It is ahead on purchases and clicks, but only B was analysed.
- One week only. A single send can be luck, and the NL B2B result rests on small numbers.
- B has the most unsubscribes (176 vs 162 for Control). The gap is small, but keep an eye on it in the retest.

Thanks,
[draft for approval]

---

## Slack version

*Braze tests 3-9 Nov (draft, not sent)*
- B2C subject line: Variant B is ahead of Control, not confirmed. 725 vs 637 purchases, 0.668% vs 0.597% of deliveries, +12% (significant at 95%, not at our 98%). DE +12.3%, FR +17.2%, NL -0.7%: the markets differ. Retest, do not roll out.
- Revenue after refunds: B EUR 4,216.50, Control EUR 3,712.33, A EUR 4,956.08. Braze shows EUR 4,245.38 for B because it counts refunded orders.
- Variant A: 847 purchases, +33.0% vs Control, ahead in all three markets. The analysis report covers only B, so A is untested.
- B2B second pickup window: Variant A 188 vs Control 178 stores (2.32% vs 2.16%, +7.5%): DE -5.7%, FR -4.5%, NL +81.8%. Stores expect 378 vs 357 extra bags a day. Ahead, not proven, no significance test.
- Purchase and partner counts match Braze (revenue total not re-added). One week only. Next step: retest B, do not roll out.
