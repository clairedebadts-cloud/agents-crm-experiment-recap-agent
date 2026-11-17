# Where my agent's information comes from

Job: Every Tuesday before 9:00, read the CRM experimentation CSVs and draft a plain-language recap of the week's Braze tests, as an email and a shorter Slack version, for me to approve.

| What the job needs | Where it lives | How the agent gets it | Group |
|---|---|---|---|
| Braze campaign results (daily) | data/sample/sample_braze_campaign_daily.csv | The file already in data/ | Works today |
| Partner actions | data/sample/sample_partner_actions.csv | The file already in data/ | Works today |
| Transactions | data/sample/sample_transactions.csv | The file already in data/ | Works today |
| README files for these CSVs | Not in data/ yet | You save them as text files in data/sample/ | Works today, once added |
| Original data analysis report | Not in data/ yet | You save it as a text file in data/ | Works today, once added |
| Amplitude, Braze app, Gmail, Slack | Online apps | Nothing, left out of this test | Not possible, or not yet |

## Why
- The 3 CSVs: they are files in data/ now, so the agent can read them.
- README files: text files, so the agent can read them once you add them.
- Analysis report: the recap must match it. Save it as a text file or a CSV and the agent can read it.
- Amplitude, Braze app, Gmail, Slack: for this test you use only the CSVs and READMEs. No connector is needed, and none was looked up.

## What this agent should NOT have access to
- Gmail and Slack: nothing is sent for the first 10 weeks. Drafts stay on your laptop.
- Logins or passwords for Braze, Amplitude, Gmail or Slack.
- Private parts of the CSVs: not yet confirmed. Tell me which columns hold names, money or staff data, and I'll add them here.

## Do next: 1 thing
Put the README files and the original analysis report in data/sample/.
