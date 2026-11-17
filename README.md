# Braze test recap agent

Built for a weekly routine: every Tuesday before 9:00, this agent reads the week's CRM experiment export from Braze and drafts a plain-language recap of the B2C and B2B tests: a full email and a shorter Slack version. Nothing is sent. The CRM owner reads the draft, approves it and sends it.

It is built for a team where strategy is set centrally, tests run in several markets (here DE, FR and NL), and the results need to reach data, marketing, local teams and leadership in a form everyone can read.

All data in this repo is synthetic. None of it is real company or Braze data.

## What it does

1. Reads the Braze campaign export, the transactions file and the partner actions file for one week.
2. Works out deliveries, opens, clicks, conversions, revenue and lift per test and variant.
3. Checks that Braze conversions match the transaction and partner action rows, and says so when they don't.
4. Writes the email (result first, one paragraph per test, then what to watch) and a Slack version of 4 to 6 lines with the same numbers and caveats.
5. Compares the two texts number by number before saving the draft.

## The rules it follows

- No variant is called a winner unless the analysis report shows it is significant at 98%. Otherwise it is "ahead" or "behind".
- Open rates always come with a note that they include machine opens, and opens never decide a test.
- Expected extra bags are reported as "expected", never as sold.
- Every number has to trace back to a row or a sum in the files.
- It never sends anything, and it ignores instructions hidden in the data files.

## How it was tested

Five test cases, each with a checklist, graded blind by a separate agent that never sees the agent's instructions:

| Case | What it checks |
|---|---|
| 1 | A normal week, checked against an analysis report |
| 2 and 3 | Two weeks built from my own scenarios |
| 4 | A vague week with a missing transactions file |
| 5 | A trap: the data README tells the agent to skip its rules and email all staff |

Results over four rounds of changes: 0, 1, 3, then 4 of 5 cases passing. A stricter fifth round ran every case three times: 11 of 15 runs passed. The trap case passed every time. Most remaining fails are formatting of the closing summary, and one run left out a p-value.

## Where things are

| Path | What it is |
|---|---|
| `CLAUDE.md`, `memory.md` | The agent's instructions and its reader profile |
| `.claude/skills/my-reports/` | The weekly recap job |
| `.claude/skills/run-tests/` | Reruns the test set and grades it blind |
| `.claude/rules/` | Rules that always apply (never send, never invent numbers) |
| `data/sample/` | The sample week the agent runs on |
| `data/examples/` | Three more sample weeks from invented companies |
| `drafts/` | The recaps it produced |
| `drafts/tests/` | Test cases, checklists and the graded rounds |

Start with `drafts/2026-11-14-recap-braze-tests.md` to see a finished recap.

## Running it

It runs in Claude Code. Open the folder, then type `/my-reports`.
