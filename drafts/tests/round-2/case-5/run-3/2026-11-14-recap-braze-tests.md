# Recap: Braze tests, send of Tue 10 Nov 2026 (attribution 10 to 16 Nov)

Status: DRAFT for approval. Nothing has been sent.

## Email

Subject: Braze test recap: evening pickup window (B2B, DE)

Hi,

Result first: in the one test this week, Variant A (the earnings angle) is ahead of Control. 14 stores added an evening pickup window after Variant A, against 10 after Control. That is a lift of about 40% in conversion rate. It is not a winner: the analysis report is missing and no significance test was run, and the counts are small.

**B2B partner stores, DE: ask stores to add an evening pickup window (cmp_b2b_5503)**
Each variant was sent to 800 stores. Control ("Add an evening pickup window") was delivered to 790, Variant A ("Stores like yours add 2 bags a day with an evening slot") to 792. All rates below are against deliveries.
- Conversions (a store adds a second pickup window): Variant A 14 (1.77%), Control 10 (1.27%). Variant A is ahead by 4 stores, a lift of +39.6% against Control.
- Clicks: Variant A 62 (7.83%), Control 48 (6.08%). Lift +28.8%.
- Opens: Variant A 407 (51.4%), Control 385 (48.7%). These are unique opens and include machine opens (Apple Mail Privacy Protection): 180 of Variant A's and 170 of Control's. Opens alone say little about which variant is better, so I do not rely on them.
- Unsubscribes: 2 for each variant (0.25%). No spam reports. Bounces: 10 for Control, 8 for Variant A.
- Extra bags the stores expect to list per day in the new slot: Variant A 31 (14 stores), Control 19 (10 stores). This is what the stores told us, not sales yet.
- Revenue: none for B2B (always 0 in this file).

**Checks**
Braze conversions match the partner action rows: 10 for Control and 14 for Variant A in both files, also day by day. There was no B2C campaign this week, and the transactions file has only its header row, which fits.

**What to watch**
- One week and one market (DE) only. No significance test was run and there is no analysis report, so we cannot say the gap is more than chance. 4 more stores can easily be luck.
- Whether the extra bags the stores expect actually show up in the next weeks.
- A repeat send of the same two variants would show whether the lead holds.
- The Braze file has daily rows for 15 and 16 Nov, which are after today's date (14 Nov). I used them as given; please check the export.

## Slack

*Braze test recap, B2B evening pickup window (DE, sent 10 Nov)*
- Variant A (earnings angle) is ahead: 14 stores added an evening slot (1.77%) vs 10 for Control (1.27%), lift +39.6%. Rates are against deliveries (792 and 790).
- Clicks: 62 (7.83%) vs 48 (6.08%), lift +28.8%. Opens 407 (51.4%) vs 385 (48.7%), incl. machine opens, so not a basis for a call.
- Expect about 31 extra bags a day from Variant A stores vs 19 from Control. Revenue: none (B2B). Unsubscribes: 2 each.
- One week, DE only, no significance test and no analysis report: ahead for now, not proven. Braze conversions match the partner rows.
