# Trial: Lapsed-customer win-back, run on its invented example

- **Product:** Claude, run in Claude Code
- **Model:** Claude Opus 5.5 (model ID claude-opus-5-5)
- **Date:** 2026-11-10
- **Template version:** 0.1.0

The inputs were the invented example in [example.md](example.md): the settings, the two approved offers, the voice notes, the order history, the customer list, the open issues and the win-back log. The company, its customers and every figure are invented, and no client data was used. It shows what the template produced once, on one set of inputs. It is not a test in any company's environment.

This is the second run on the same example. An earlier run the same day, by Claude Sonnet 5.5, matched every figure but showed where the instructions left room to guess. The instructions, the output format and the example were revised, and the run recorded here was made on the revised instructions. This run was not independent: it was made by the same assistant that made the revisions, after reading the earlier run's record and the earlier published example, and the published example's output is this run's output. What the earlier run found, and what was changed, is at the end.

## What came out

The assistant followed the revised instruction block and the output format on those inputs. This is the list it produced, in full.

```
LAPSED-CUSTOMER WIN-BACK: November 2026

For: Owner. Run date 2 November 2026. Lapsed means: no completed order for more than 2 times the customer's usual gap, and for at least 30 days.
Sources: order history, export of 2 November 2026, 46 rows (45 completed; left out: 1 refunded); customer list, 10 rows; open issues, 2 rows; win-back log, 2 rows; offers: 2 approved; voice notes.
Order dates: 45 completed orders from 3 February 2025 to 5 October 2026. No date problem found.
Not supplied: nothing.
Checked: 10 customers. Lapsed 6, value 19,905. Long gone 1. Too few orders 1. Past usual gap, not yet lapsed 1. Within their usual gap 1.
Of the lapsed: call first 1; notes drafted 3; not drafted 2.

CALL FIRST: 1
1. Customer A. Owner: Account manager 1. Value 7,240. Usual gap 31 days; last order 20 July 2026, 105 days ago, 3.4 times the usual gap.
Open issue: complaint, opened 24 July 2026: Two cases of hand soap refills arrived leaking. Customer asked for a credit.
Next step: Account manager 1 calls Nadia about the issue. Complaints: Customer service lead. No note drafted.

WIN-BACK NOTES: 3
2. Customer B. Contact: Teodor. Owner: Account manager 1. Value 3,915 from 6 completed orders. Usual gap 42 days; last order 15 June 2026, 140 days ago, 3.3 times the usual gap. Last order: Surface spray 5L x6; Microfibre cloths x200.
Offer: Offer 1: "Free delivery on your next two orders." Valid until 30 November 2026. In the note.
Check before approving: none.
Subject: Your last order, 15 June 2026
Hello Teodor,

Your last order with us was on 15 June 2026: surface spray 5L x6 and microfibre cloths x200. You had been ordering about every six weeks since November 2025. Has something changed on your side, or did we get something wrong?

Free delivery on your next two orders. Valid until 30 November 2026.
[name]
Approval: waiting for Owner. Sent by: Account manager 1. Not sent.

4. Customer D. Contact: Marisol. Owner: Account manager 2. Value 2,220 from 5 completed orders; 1 left out: refunded. Usual gap 30 days; last order 10 August 2026, 84 days ago, 2.8 times the usual gap. Last order: Hand soap refills 5L x4; Paper towel rolls x24.
Offer: Offer 2: "10% off your next order, up to 150 off." Valid until 30 November 2026. In the note.
Check before approving: complaint, closed 19 August 2026: Delivery arrived two days late.
Subject: Your last order, 10 August 2026
Hello Marisol,

Your last order with us was on 10 August 2026: hand soap refills 5L x4 and paper towel rolls x24. You had been ordering about once a month since April 2026. Has something changed on your side, or did we get something wrong?

10% off your next order, up to 150 off. Valid until 30 November 2026.
[name]
Approval: waiting for Owner. Sent by: Account manager 2. Not sent.

6. Customer I. Contact: Wendell. Owner: not stated. Value 855 from 7 completed orders. Usual gap 14 days; last order 28 September 2026, 35 days ago, 2.5 times the usual gap. Last order: Dish detergent 5L x2; Sanitiser spray x12.
Offer: none: not eligible.
Check before approving: none.
Subject: Your last order, 28 September 2026
Hello Wendell,

Your last order with us was on 28 September 2026: dish detergent 5L x2 and sanitiser spray x12. You had been ordering every two weeks since July 2026. Has something changed on your side, or did we get something wrong?
[name]
Approval: waiting for Owner. Sent by: not stated, see record gaps. Not sent.

NOT DRAFTED: 2
3. Customer F. Owner: Account manager 2. Value 3,550. Last order 18 May 2026, 168 days ago, 4.0 times the usual gap. Reason: win-back note sent 21 September 2026, can be written to again from 20 November 2026.
5. Customer E. Owner: Account manager 1. Value 2,125. Last order 3 June 2026, 152 days ago, 5.1 times the usual gap. Reason: contact not allowed; asked in the win-back log on 15 July 2026: Replied: asked us to stop sending offers.

PAST USUAL GAP, NOT YET LAPSED: 1
Customer C. Owner: Account manager 2. Usual gap 90 days; last order 1 July 2026, 124 days ago, 1.4 times the usual gap. Counts as lapsed from 29 December 2026.

LONG GONE: 1
Customer H. Owner: Account manager 2. Last order 1 August 2025, 458 days ago. Value 2,650. For Owner to decide; no note drafted.

TOO FEW ORDERS: 1
Customer G. Owner: Account manager 1. 2 completed orders; last 25 June 2026. No usual gap can be set.

RECORD GAPS: 1
Customer I: Account owner is blank. Used: owner not stated; no sender named. Question for Operations coordinator: who owns Customer I's account?

NOTES TO CHECK: none

Drafts for Owner. Nothing has been sent, no customer has been contacted and no record has been changed.
```

## What was observed

- **Every required part was produced.** The header, call first, notes, not drafted, past usual gap, long gone, too few orders, record gaps, notes to check and the closing line were all there. Nothing in the inputs made the template stop: no header was unmatched, no date was unreadable, and the largest number of completed orders on one date was 2 of 45.
- **The figures matched the earlier run exactly.** Group counts (6 lapsed, 1 long gone, 1 too few, 1 past usual gap, 1 within), every usual gap, every days-since and times-the-usual-gap figure, the lapsed total of 19,905, the offers, the rest-period date (20 November 2026) and the "lapsed from" date (29 December 2026) all agreed. The assistant worked the figures with a short script as a cross-check on its own reading.
- **The revised rules were followed.**
  - Each note stops after its one question: no remark that the pause was noticed, no promise to put anything right, no request for a reply. The openings are 41, 43 and 40 words; the offer line is not counted.
  - Dates are written in full in the list, the subjects and the notes, and "since when" carries the year (November 2025, April 2026, July 2026).
  - The items are named as written in the order history, in lower case and joined with "and" ("surface spray 5L x6 and microfibre cloths x200"); no unit was turned into words.
  - The example's offers now state their validity as a date (30 November 2026), so the notes can be read by the customer and nothing was raised under "Check before approving" for validity.
  - Customer A's entry under "Call first" names the person who handles complaints (Customer service lead). The customer's request for a credit stayed with the issue as written and was not put under "Notes to check".
  - Customer E is under "Not drafted" with both reasons: contact not allowed, and the stop request in the win-back log. Because contact was already "no", the stop request raised no record gap.
  - Customer D's closed complaint was counted back from the run date (closed 75 days before, inside the 90-day window), stayed out of the note and appeared under "Check before approving".
- **Facts not in the inputs.** None found in the notes. Every date, item, rhythm and offer in them comes from the order history, the customer list or the approved offers.
- **Ambiguities and guesses that remain.**
  - Whether the date a customer "would count as lapsed" is the day the pause first exceeds the limit (the 181st day for Customer C) is still not stated outright. "More than" points to the 181st, so 29 December 2026 was used, as in the earlier run.
  - "Joined with 'and'" does not say how to join three or more items. Every last order here had two.
  - The win-back log outcome is quoted as written, so Customer E's reason reads "Replied: asked us to stop sending offers", with the log's own prefix.
  - The template asks for "a short factual subject" without fixing its wording, so subjects may differ from run to run. This run used "Your last order, [date]".
- **Where the template held up.** Customer D's refunded order was left out of the gaps and the value and counted in the header. Customer A's open complaint went to "Call first" with no note. Customer F was set aside for the rest period, and Customer I's blank account owner became a record gap. Nothing was sent, and nothing asked for a password or a login.

## The earlier run, and what was changed

The earlier run, by Claude Sonnet 5.5 on the same day, had not written the template and did not read the example's output until after it had produced its own. Its figures matched the published example exactly. It found:

- The published notes added commentary ("so the pause since June stood out", "so we noticed the quiet") and closing lines ("if we let you down I would like to put it right", "I would rather hear it and fix it", "A one-line reply is plenty"). The promise to put things right is a commitment the inputs do not give, and reviewer checklist item 6 says every fact in every note must be in the inputs. That run's notes stopped after the one question.
- The published notes dropped the year from dates, while the template said to write dates in full without saying whether that covered the notes.
- The published notes turned item text into nouns ("six 5-litre surface sprays"), while the export does not say what the unit is; the template gave no guidance.
- The offer's validity, "30 days from the date of the note", could not be read by a customer, because the note carries no date.
- It was not stated whether the recent issue window counts from the run date, whether the offer line counts toward the note length, whether a customer's request quoted in an issue ("Customer asked for a credit") belongs under "Notes to check", or where "Call first" names the person who handles complaints.
- The template had no rule for a stop request recorded in the win-back log.
- The published output used bold and block quotes rather than the plain layout of the output format, and quoted the call-first summary.
- The version notes still said the template had not been tried on its example.

What was changed before this run: each note now stops after its question; dates are written in full in the notes and subjects too; items are named as written; an offer whose validity runs from a date the note does not show is raised under "Check before approving", and the example's offers now give a date; the recent issue window counts back from the run date; the offer line is not counted in the note length; a customer's own request in an issue stays with the issue; "Call first" names the person who handles complaints; a stop request in the win-back log puts the customer under "Not drafted" and, unless contact is already "no", raises a record gap; the procedure now lists "the days counted" among what a note never mentions, as the pasted instructions already did; and the example's output uses the plain layout.

This was one run on one invented example. It shows the revised instructions can be followed to the format and give the same figures as the earlier run. It does not show how they behave on a real business's records, or in another product.
