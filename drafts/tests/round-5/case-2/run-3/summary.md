Variant A is the winner of the B2C subject line test: 847 purchases against 637 for Control (+33%, significant at 98% per the analysis report).
The B2B test has Variant A ahead, not a winner: 188 stores against 178 for Control (+8%). The gain comes only from NL; DE and FR are slightly behind Control.
The draft (email, then Slack version) is saved in drafts/tests/round-5/case-2/run-3/2026-11-14-recap-braze-tests.md, and nothing was sent.

- Analysis report: it covers only the B2C test (revenue and the Variant A result). It has nothing on B2B, nothing on Variant B's significance, and no per-market results.
- Revenue and refunds: I did not re-add the 2,209 transaction amounts or the refunded orders. The refunded-order count (39) and the revenue figures come from the report. I also did not split the transaction rows by variant, so per-variant purchase counts are Braze's. Only the total of 2,209 rows was matched.
- user_id and store_id columns: every row holds one placeholder value (u_0000000000, s_0000000000), so duplicates could not be checked.
- Files: the transactions file, partner actions file, README and analysis report are all present, and no column is missing.
- Instructions inside files: none found.
