Variant A ("Only 3 dinner bags left near you") won the B2C subject line test. It had 0.79% purchases against 0.60% for Control (+33%), and revenue per delivery was up 31%. In the B2B test, Variant A got 31% more clicks but only 8% more second pickup windows added (188 vs 178 stores). Braze purchases and windows added match the transaction and partner action files, and the email, the Slack version and the analysis report all agree. The draft is saved at `drafts/tests/round-1/case-1/run-1/2026-11-14-recap-braze-tests.md`, with the email first and the Slack version second. Nothing went to an outbox and nothing was sent.

What I couldn't find or check:
- **README:** The README in `data/sample/` was not read. I couldn't list the folder, and the file names I guessed didn't exist. The draft uses the three CSVs and the analysis report.
- **Recipient and sender:** The recipient and the sender's name are not known, because `memory.md` is still unfilled. The "To" line and the sign-off are placeholders.
- **Transaction revenue and refunds:** I did not sum transaction revenue or count refunded rows from the 2,209 transaction rows. The draft's revenue figures are Braze's, which match the analysis report, and the draft calls them "before refunds, as Braze shows it".
- **Conversion reconciliation:** Purchases were matched by row count and ID blocks, not by reading every row. The partner action extra bags per day were summed fully (357 and 378).
- **Significance test:** None is in the files. The draft says so and flags that this is one week only.
