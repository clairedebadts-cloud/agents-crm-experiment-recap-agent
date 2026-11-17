Variant A is ahead in both tests, but neither result is proven (one week, no significance test).
The app test has A ahead of Control by 33% on purchases; the store test is a small 8% gap.
The draft, email then Slack version, is saved in `drafts/tests/round-3/case-1/run-1/2026-11-14-recap-braze-tests.md` (nothing sent).

Not found or not done:
- Transaction amounts vs Braze revenue: I did not add up the 2,209 amounts by variant, so that check is open. Row counts match (2,209 purchases, 366 window additions). Revenue per variant matches the analysis report.
- Expected extra bags (357 and 378): taken from the analysis report, not re-added from `sample_partner_actions.csv`.
- Refund amounts: not worked out, so revenue is before refunds only, as in the report.
- Significance test: none exists. The analysis report says none was run, so there is no winner.
- Files and columns: no file or column is missing, no test has missing data, and no file told me to do anything.
- Not read, as instructed: `data/examples/` and the other `data/` files. Checks on the open files showed one mismatch with the report's reading: in the store test, Variant A is ahead only in NL and slightly behind in DE and FR. I put this in both texts.
