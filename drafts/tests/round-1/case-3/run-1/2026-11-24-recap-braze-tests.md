# Draft: weekly Braze test recap (not sent, for approval)

Week: send on Tue 17 Nov 2026, attribution 17 to 23 Nov. One test this week.

---

## Email

Subject: Braze test recap, 17-23 Nov: subject line test is not a winner

**The result**
The "Only 3 dinner bags left near you" subject line (Variant A) bought more bags overall, but it is not a winner. Do not roll it out. The overall lift is real-looking but comes from one market only, and the markets disagree.

**B2C subject line test, Winter dinner bags (cmp_b2c_7703)**
Both versions went to 5,000 people in each of DE, FR and NL. 4,900 per market got the email (14,700 per version). Rates below are conversions (Surprise Bag purchases) divided by emails delivered.

| | Control ("Fresh dinner bags near you tonight") | Variant A ("Only 3 dinner bags left near you") | Lift of A vs Control |
|---|---|---|---|
| Overall | 100 purchases (0.68%) | 130 purchases (0.88%) | +30% |
| DE | 20 (0.41%) | 60 (1.22%) | +200% |
| FR | 50 (1.02%) | 40 (0.82%) | -20% |
| NL | 30 (0.61%) | 30 (0.61%) | 0% |

- Overall, Variant A got 30 more purchases out of the same number of emails. The data team says that lift is significant at 95% confidence but not at 98%. Our rule needs 98% to call a winner, so it is not one.
- The markets point in different directions. DE is far ahead, FR is behind, NL is flat. DE alone explains the gap: without DE, Control has 80 purchases and Variant A has 70. The data team says the FR drop is not significant on its own. For DE they say "clearly ahead", but the report gives no confidence figure for it.
- Revenue: Control EUR 477.50, Variant A EUR 607.60 (+27%). No orders were refunded. The revenue difference follows the purchase count, since every bag in a market costs the same.
- Opens: unique opens (these include machine opens from Apple Mail Privacy Protection) were 6,150 for Control (41.8% of deliveries) and 6,300 for Variant A (42.9%). Machine opens were 2,760 and 2,820 of those. Opens are too unreliable and too close to say anything, so this recap does not use them to judge the test.
- Clicks: 441 for Control (3.0%) and 450 for Variant A (3.1%). Basically the same.
- Unsubscribes: 6 for each version. Spam reports: 0.

**What to watch**
- Do not roll out Variant A. Keep testing.
- A follow-up test in DE alone is worth considering, since that is where the lift is.
- Why FR went the other way is open. Nothing in the files explains it.
- Limits: this is one week of data. I ran no significance test myself; the 95% and 98% statements come from the data team's report.

**Data check**
Braze conversions match the transactions file: 230 purchases in both (Control 100, Variant A 130), and the same split per market. Revenue in Braze matches the transaction amounts: EUR 1,085.10 in both. There was no B2B campaign this week, so the partner actions file is empty, as expected.

---

## Slack version

*Braze test recap, 17-23 Nov: subject line test (Winter dinner bags)*
- Not a winner, don't roll out. Variant A ("Only 3 bags left") had 130 purchases vs 100 for Control (0.88% vs 0.68% of deliveries, +30%), significant at 95% but not our 98% bar.
- Markets disagree: DE 60 vs 20 (+200%), FR 40 vs 50 (-20%), NL 30 vs 30 (flat). DE drives the whole lift.
- Revenue: EUR 607.60 vs EUR 477.50. Opens are similar (42.9% vs 41.8%, includes machine opens), so not used to judge.
- Braze and transaction numbers match. One week only, no test run by me. Next: keep testing, maybe a DE follow-up.
