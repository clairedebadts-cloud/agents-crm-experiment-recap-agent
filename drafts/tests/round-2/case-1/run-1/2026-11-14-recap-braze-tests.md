# DRAFT for approval. Nothing has been sent.

Week: send Tuesday 3 Nov 2026, 17:00, plus 7 days of results (3 to 9 Nov). Markets: DE, FR, NL.

---

## Email

**To:** [to be filled in by you]
**Subject:** Braze test recap, 3-9 Nov: Variant A is ahead in both tests

Hi all,

**The result in short.** In both tests Variant A is ahead of Control. In the app-user email (B2C), the "Only 3 dinner bags left near you" subject line led to 33% more purchases than Control. In the store email (B2B), the earnings-angle email got 8% more stores to add a second pickup window, a small gap. This is one week of data and no significance test was run, so Variant A is not a winner in either test. "Ahead" is as far as the numbers go.

**B2C: subject line test, Winter dinner bags (DE, FR, NL).** All rates are against deliveries (emails that arrived), not sends.
- Control ("New Surprise Bags near you tonight"): 106,798 delivered, 637 purchases, 0.60% conversion rate, EUR 3,839.46 revenue (EUR 0.036 per delivery).
- Variant A ("Only 3 dinner bags left near you"): 106,796 delivered, 847 purchases, 0.79%, EUR 5,028.24 (EUR 0.047 per delivery).
- Variant B ("Rescue tonight's dinner for EUR 4.50", with emoji): 108,518 delivered, 725 purchases, 0.67%, EUR 4,245.38 (EUR 0.039 per delivery).
- Against Control: Variant A has 33% more purchases and 31% more revenue per delivery. Variant B has 12% more purchases and 9% more revenue per delivery.
- By market, Variant A is ahead of Control in all three: DE 0.81% vs 0.60%, FR 0.80% vs 0.58%, NL 0.74% vs 0.63%. Variant B is ahead in DE (0.68%) and FR (0.68%) and level with Control in NL (0.62% vs 0.63%).
- Opens: Control 43.9%, Variant A 44.9%, Variant B 48.2%. These are unique opens and include machine opens (Apple Mail Privacy Protection), which are about 47% of opens in every variant. Variant B's higher open rate therefore tells us little, and opens alone don't decide the test. Purchases do.
- Unsubscribes: Control 162, Variant A 167, Variant B 176 (about 0.15% to 0.16% of deliveries each), so no real difference.
- Revenue is before refunds, the same way Braze shows it. The data team's report uses the same figure, so there is no gap to explain.

**B2B: second pickup window test (stores in DE, FR, NL).**
- Control ("Add a second pickup window to your store"): 8,248 delivered, 178 stores added a window, 2.16% conversion rate, 5.78% clicked.
- Variant A ("Stores like yours sell 2 more bags a day with an evening slot"): 8,101 delivered, 188 stores added a window, 2.32%, 7.58% clicked.
- Against Control: clicks +31%, conversions +8%. The conversion gap is small (10 more stores). Variant A got far more clicks, but that turned into only a few more windows.
- Stores say they expect to list 357 extra bags per day (Control) and 378 (Variant A). These are what stores expect to list, not bags sold.
- By market (my own split of the Braze file, not in the data team's report): NL is where Variant A is ahead (46 vs 26 stores, 3.23% vs 1.78%). In DE (68 vs 72 stores, 2.18% vs 2.31%) and FR (74 vs 80, 2.08% vs 2.18%) Variant A is slightly behind Control. The numbers per market are small, so this may be chance.
- Unsubscribes: 4 (Control) and 5 (Variant A).

**Checks.** Braze conversions match the other files. B2C: 2,209 purchase rows in the transactions file = 637 + 847 + 725. B2B: 366 rows in the partner actions file = 178 + 188. The figures also match the data team's analysis report.

**What to watch.**
- One week only, and no significance test was run. Variant A is ahead, nothing more. Ask the data team for a test before we change the default subject line.
- Variant A's lead holds in all three B2C markets, which is a good sign. Check again next send.
- For B2B, the extra clicks did not turn into many more windows. The NL gain may be the whole story, so look at DE and FR before rolling out the earnings angle.
- Do not read Variant B's higher open rate as a better result. About 47% of opens are machine opens.

Best,
[name]

---

## Slack version

*Braze tests 3-9 Nov (one week, no significance test, so Variant A is "ahead", nothing more):*
*B2C subject lines (rates vs deliveries):* purchases Control 637 (0.60%), Variant A 847 (0.79%), Variant B 725 (0.67%). Lift vs Control: A +33%, B +12%. Revenue EUR 3,839.46 / 5,028.24 / 4,245.38 before refunds; per delivery A +31%, B +9%.
*B2C by market:* A is ahead of Control in DE, FR and NL (0.81/0.80/0.74% vs 0.60/0.58/0.63%). B is ahead in DE and FR (0.68% each), level in NL (0.62%).
*B2C opens:* 43.9% / 44.9% / 48.2% include machine opens (about 47% of opens), so they don't decide the test.
*B2B second pickup window:* stores that added one: Control 178 (2.16%), Variant A 188 (2.32%), lift +8%, a small gap. Clicks 5.78% vs 7.58% (+31%). Expect 357 vs 378 extra bags a day (what stores plan to list, not sold). A is ahead in NL (46 vs 26 stores) and slightly behind in DE (68 vs 72) and FR (74 vs 80).
*Next:* ask the data team for a significance test before changing anything. Braze counts match the transaction and partner files.
