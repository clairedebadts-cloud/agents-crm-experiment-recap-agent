Variant B is ahead of Control by 12% on purchases, but it is not a winner at the 98% rule, so the advice is to retest and not roll out.
Variant A is ahead in all three markets and the B2B Variant A is ahead overall, but neither has a significance test.
The draft (email, then Slack) is saved at drafts/tests/round-3/case-3/run-1/2026-11-14-recap-braze-tests.md, and nothing was sent.

Couldn't find or check:
- Analysis report: it covers only Variant B against Control in B2C. It has no test for Variant A (B2C), none for the B2B test, and no revenue figure.
- Revenue: left out of the recap. Braze revenue counts refunded orders and the report gives no revenue figure, so there is no agreed number.
- Transactions check: only the total row count (2,209) was matched to Braze purchases. I did not count rows per variant or per market, and did not sum amount_eur against revenue.
- Partner actions check: matched per day and per variant (178 and 188 conversions). I did not count rows per market.
- Instructions inside files: none found.
- Files and columns: nothing else missing. The Braze file, transactions file, partner actions file and README are all present, and the columns needed for the recap are all there.
