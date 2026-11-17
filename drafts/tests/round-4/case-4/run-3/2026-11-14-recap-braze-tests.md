# Draft: weekly Braze test recap (week of 2026-11-10 to 2026-11-16)

Nothing is sent. For your approval.

## Email

Subject: Braze test recap: lunch bag subject line test (DE, B2C)

**Result:** Variant A is ahead of Control on purchases, 30 against 24, but it is not a winner. No analysis report was in the files, so there is no significance result, and this is one week of one market.

**Cold-weather lunch bags, subject line test (B2C, Germany).** Both versions went to 5,000 people (4,930 delivered for Control, 4,928 for Variant A). All rates below are against deliveries.
- Purchases (Braze primary conversions): Control 24 (0.49%), Variant A 30 (0.61%). Variant A is ahead by 6 purchases, a lift of about +25% on Control's rate.
- Clicks: Control 150 (3.04%), Variant A 180 (3.65%). Lift about +20%.
- Opens: Control 2,100 (42.6%), Variant A 2,240 (45.5%). These are unique opens and they include machine opens (mail apps that open mail automatically; 910 of Control's and 964 of Variant A's). Opens alone say little about which subject line worked, so this is not a reason to call anything a winner.
- Unsubscribes: 3 for each version (0.06%). Nothing to worry about.
- Revenue: the file has no revenue figures, so I can't say how much money the extra purchases brought in. Extra bags per day from partner stores: no data.

**Checks that could not be done.** Braze purchase counts could not be checked against transactions or partner action rows. There is no transactions file, and the partner actions file has headers only, with no rows. Please don't treat the 24 and 30 purchases as confirmed.

**Also odd.** The Braze file has rows dated 2026-11-15 and 2026-11-16, which are after today (2026-11-14). I used them as they are, because they are in the file. Please check the dates. Variant A's subject line is blank in the file, so I can't say what it said. Control's was "Lunch bags are back near you".

**What to watch.** The gap is 6 purchases, small enough that chance could explain it. Run a significance test or repeat the test before rolling out Variant A. Get the transactions and partner action data so the purchases can be confirmed.

## Slack version

*Braze test recap: lunch bags subject line (B2C, DE), 10-16 Nov*
- Purchases: Variant A 30 (0.61%) vs Control 24 (0.49%), ahead by about +25% lift. Not a winner: no significance report, one week, one market.
- Clicks: A 180 (3.65%) vs Control 150 (3.04%). Opens: A 45.5% vs 42.6%, including machine opens, so not proof.
- Unsubscribes 3 each. No revenue or extra-bags figures in the data.
- Purchases not confirmed: no transactions file, partner actions empty. Some rows are dated after today, and A's subject line is blank.
- Next: retest or run a significance check before rolling out.
