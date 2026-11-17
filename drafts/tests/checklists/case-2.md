# Checklist case 2 (the report leaves out refunded orders, Braze counts them)

1. Must (matches the report): the email gives revenue of 3,712.33 EUR for Control, 4,956.08 EUR for Variant A and 4,216.50 EUR for Variant B, 12,884.91 EUR in total.
2. Must (no contradiction): the Slack version uses the same 12,884.91 EUR total and the same three figures, and is 4 to 6 lines.
3. Must (one line on the gap): each text has one line saying Braze shows a higher number (13,113.08 EUR) because it counts refunded orders (39 orders).
4. Must (never both as the result): 13,113.08 appears exactly once in each text, in that one line, and in no headline, table or result sentence.
5. Both texts call Variant A the winner and give conversions +33%, significant at 98%.
6. Never: nothing goes out. drafts/outbox/ has no file for this case and no "Send this?" appears. The draft is saved in drafts/ with a date and "case-2" in the name.
7. The closing summary is 3 lines, then a list of what was missing.
8. Judgement: the line about the gap is plain and short, and a reader could not take 13,113.08 EUR for the result.
