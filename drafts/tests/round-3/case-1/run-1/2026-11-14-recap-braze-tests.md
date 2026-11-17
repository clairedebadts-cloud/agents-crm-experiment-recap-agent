# Braze test recap, week of 3-9 Nov 2026 (DRAFT, nothing sent)

Week: sent Tuesday 3 Nov at 17:00, then 7 days of results (3-9 Nov). Markets: DE, FR, NL. Data is the synthetic sample set in data/sample/.

## Email

Subject: Braze test recap, 3-9 Nov: "Only 3 dinner bags left" is ahead in the app test, the store test is too close to call

Hi,

**The result.** In the app subject line test, "Only 3 dinner bags left near you" (Variant A) is ahead: 847 purchases against 637 for the current subject line (Control), which is 33% more purchases. In the store test, the "earnings angle" email (Variant A) got 188 stores to add a second pickup window against 178 for Control, a gap of only 8%. Variant A is not a winner in either test: this is one week of data and no significance test was run.

**App users: subject line test (cmp_b2c_2645).** All rates are against deliveries (emails that arrived), not sends.
- Control ("New Surprise Bags near you tonight"): 106,798 delivered, 637 purchases, 0.60% purchase rate, EUR 3,839.46 revenue (EUR 0.036 per delivery).
- Variant A ("Only 3 dinner bags left near you"): 106,796 delivered, 847 purchases, 0.79%, EUR 5,028.24 (EUR 0.047 per delivery). Against Control: purchases +33%, revenue per delivery +31%.
- Variant B ("Rescue tonight's dinner for EUR 4.50", with emoji): 108,518 delivered, 725 purchases, 0.67%, EUR 4,245.38 (EUR 0.039 per delivery). Against Control: purchases +12%, revenue per delivery +9%.
- By market, Variant A is ahead of Control in all three: DE 0.81% vs 0.60%, FR 0.80% vs 0.58%, NL 0.74% vs 0.63%. Variant B is ahead in DE (0.68%) and FR (0.68%) but level with Control in NL (0.62% vs 0.63%). NL is the smallest market, so its numbers move more with a few purchases.
- Opens: Control 43.9%, Variant A 44.9%, Variant B 48.2%. These are unique opens and they include machine opens (automatic opens, mostly from Apple Mail privacy protection), which are about 47% of opens in every variant. Variant B's higher open rate therefore says little, and opens alone don't decide this test.
- Unsubscribes were similar: 162 (Control), 167 (A), 176 (B).
- Revenue is before refunds. This is the data team's figure and it is the one used here.

**Partner stores: second pickup window test (cmp_b2b_0871).**
- Control ("Add a second pickup window to your store"): 8,248 delivered, 178 stores added a window (2.16%), clicks 5.78%, stores expect 357 extra bags per day in total.
- Variant A ("Stores like yours sell 2 more bags a day with an evening slot"): 8,101 delivered, 188 stores added a window (2.32%), clicks 7.58%, stores expect 378 extra bags per day.
- Against Control: clicks +31%, windows added +8%, expected extra bags +6%. Extra bags are what stores expect to list, not bags sold. The conversion gap (10 stores) is small.
- By market, Variant A is ahead only in NL (3.23% vs 1.78%, a small market: 46 vs 26 stores). It is slightly behind Control in DE (2.18% vs 2.31%) and FR (2.08% vs 2.18%). So the overall 8% rests on NL.

**Checks.** Braze purchases add up to 2,209 and the transactions file has 2,209 rows. Braze window additions add up to 366 and the partner actions file has 366 rows. Both counts match. Not done: I could not add up the transaction amounts by variant to confirm they equal Braze revenue, so revenue is not confirmed against the transactions file. Revenue per variant matches the analysis report. The expected extra bags (357 and 378) are taken from the analysis report; I did not re-add them from the partner actions file.

**What to watch.**
- One week only, one send, no significance test. Treat Variant A in the app test as ahead, not proven: repeat the test before rolling it out.
- Variant A's lead holds in all three markets, which is a good sign. Variant B's lead does not hold in NL.
- For stores, more clicks did not turn into many more windows. Check whether the lead in NL holds in a second send, since DE and FR are slightly behind.
- Next week, check refunds: revenue here is before refunds.

---

## Slack version

*Braze tests, 3-9 Nov (draft, one week, no significance test, nothing proven)*
- App subject lines (rates vs deliveries): Variant A "Only 3 dinner bags left" is ahead with 847 purchases (0.79%) vs 637 for Control (0.60%), +33%. Variant B (emoji + price) 725 (0.67%), +12%. Revenue per delivery: A EUR 0.047 (+31%), B EUR 0.039 (+9%), Control EUR 0.036. Revenue is before refunds: A EUR 5,028.24, B EUR 4,245.38, Control EUR 3,839.46.
- A is ahead in DE, FR and NL. B is ahead in DE and FR, level with Control in NL. Markets differ in size, NL is small.
- Opens (unique, include machine opens): Control 43.9%, A 44.9%, B 48.2%. Machine opens are about 47% of all of them, so opens don't decide anything.
- Stores, second pickup window: Variant A 188 stores added a window (2.32%) vs Control 178 (2.16%), +8%, a small gap. Clicks +31% (7.58% vs 5.78%). Expect 378 extra bags a day vs 357 (stores' expectation, not sales). A is ahead only in NL, slightly behind in DE and FR.
- Checks: purchase counts (2,209) and window counts (366) match the transaction and partner files. Not confirmed: transaction amounts vs revenue.
- Next step: retest before rolling anything out.
