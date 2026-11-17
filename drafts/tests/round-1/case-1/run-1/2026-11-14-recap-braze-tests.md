# Braze test recap, week of 3-9 Nov 2026 (DRAFT, not sent)

Source: data/sample/ (Braze campaign file, transactions, partner actions) and the data team's analysis report. All rates are against deliveries, not sends.

## Email

**To:** (not known, please fill in)
**Subject:** Braze test recap, 3-9 Nov: "Only 3 dinner bags left" won the consumer test

Hi,

Result first. In the consumer subject line test, "Only 3 dinner bags left near you" (Variant A) did best: 33% more purchases than the control subject line. In the partner test, the evening-slot message (Variant A) got many more clicks (+31%), but only slightly more second pickup windows added (+8%).

**B2C subject line test (DE, FR, NL, 3-9 Nov)**
Purchases per delivered email: Control 0.60% (637 purchases from 106,798 delivered), Variant A 0.79% (847 from 106,796), Variant B 0.67% (725 from 108,518). Against Control, A has 33% more purchases and B has 12% more. Revenue per delivered email is EUR 0.036 for Control, EUR 0.047 for A (+31%) and EUR 0.039 for B (+9%). Total revenue was EUR 3,839.46 (Control), EUR 5,028.24 (A) and EUR 4,245.38 (B), before refunds, as Braze shows it. Variant B ("Rescue tonight's dinner for EUR 4.50") has the highest open rate, but opens are not a fair judge here. The open rates (Control 43.9%, A 44.9%, B 48.2% of delivered) count machine opens, such as mail apps that preload messages, and those are about 47% of opens in every variant. Purchases are the better measure, and A leads on them. Unsubscribes were low and similar: 0.15% (Control), 0.16% (A), 0.16% (B).

**B2B second pickup window test (partner stores, DE, FR, NL, 3-9 Nov)**
Variant A ("Stores like yours sell 2 more bags a day with an evening slot") got clicks from 7.58% of delivered emails (614 of 8,101) against 5.78% for Control (477 of 8,248). That is 31% more clicks. Stores adding a second pickup window were 2.32% of delivered (188) for A against 2.16% (178) for Control. That is 8% more, a gap of 10 stores, so it is small. The "extra bags per day" figures (Control 357, A 378) are what stores said they expect to list, not bags sold.

**Do the numbers match?**
Yes. Purchases in Braze equal the transaction rows (2,209 in total, with the per-variant and per-market counts matching). Windows added equal the partner action rows (366 in total: Control 178, Variant A 188). The extra bags per day match the partner action rows. The figures also match the data team's analysis report.

**What to watch**
- This is one week only, and no significance test has been run, so treat the B2C result as a strong hint, not proof. The B2B conversion gap (10 stores) is too small to call.
- Don't pick a winner on open rates: they include machine opens.
- For B2B, check next week whether the click lift turns into more windows added, and whether the expected extra bags show up in real sales.

Best,
(name not known)

## Slack

Braze tests, 3-9 Nov (rates against deliveries; one week, no significance test)
- B2C subject lines: "Only 3 dinner bags left near you" (A) won. Purchases 0.79% vs 0.60% for Control (+33%), revenue per delivery EUR 0.047 vs 0.036 (+31%).
- B ("Rescue tonight's dinner for EUR 4.50") is in between: purchases 0.67% (+12%), revenue per delivery EUR 0.039 (+9%). Highest open rate (48.2%), but opens include machine opens (about 47%), so not a win on opens alone.
- B2B second pickup window: A got 31% more clicks (7.58% vs 5.78%) but only 8% more windows added (2.32% vs 2.16%, 188 vs 178 stores). Small gap.
- Braze purchases and windows added match the transaction and partner action files. Numbers match the data team's report.
- Watch next week: does the B2B click lift turn into windows added?
