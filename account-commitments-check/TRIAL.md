# Account commitments check: tried once on its invented example

- **Product:** Claude, run in Claude Code
- **Model:** Claude Sonnet 5.5 (`claude-sonnet-5-5`)
- **Date:** 2026-11-10

The inputs are the invented example in [example.md](example.md) (Customer A, Maya, Tom, Ines and Paul). No client data was used. The run was a single attempt by a model that did not write the template. It followed the instruction block and the output format in `member/template.md` and read the example's output only after producing its own.

## Inputs used

The "What the person supplies" section of [example.md](example.md): the settings (account, period 1 September to 16 November 2026, today Monday 16 November 2026, next conversation Thursday 19 November 2026, default 21-day gap), the four people, the three-item draft agenda, four sources (two meetings, two emails) and two follow-through records.

## What came out

```
ACCOUNT COMMITMENTS CHECK: Customer A

For: Maya, account manager. Next conversation: Thursday 19 November 2026. Period: 1 September 2026 to 16 November 2026. Prepared: Monday 16 November 2026.

Sources used:
S1 Tuesday 15 September 2026, meeting, "Quarterly check-in".
S2 Monday 28 September 2026, email, Maya to Ines.
S3 Tuesday 29 September 2026, email, Ines to Maya.
S4 Tuesday 20 October 2026, meeting, "Support review call".
R1 Monday 5 October 2026, record, ticket 3318.
R2 Friday 6 November 2026, record, release 4.12.
Left out: none.

Coverage: 4 sources, 15 September to 20 October, and 2 follow-through records. Gap over 21 days: 20 October to 16 November (27 days), no source. Referred to, not supplied: Tom's call with Customer A's finance team on 3 November (S4).

Commitments: 7 (ours 3, theirs 3, side not stated 1). Open 3, done 3, unclear 1. Past due: 2.

OUR COMMITMENTS

C2 Maya to confirm the price for the extra 30 seats. Made 15 September (S1: "before the end of September"). Due Wednesday 30 September (read as). Status: DONE. Evidence: S2, 28 September, Maya's email to Ines with the prices attached. Terms: price; check against the agreement. Suggested owner: Maya. Nothing further.

C5 Maya to send the dispatcher training options. Made 20 October (S4: "I'll send you the training options this week"); first raised in soft wording on 15 September (S1: "we'll try to find a time", for a training session). Due Friday 23 October (read as). Status: OPEN, PAST DUE. Evidence: none; no source or record shows it done. That is not evidence it was not done. Suggested owner: Maya.

C3 Tom to ship the fix for the slow route-report export. Made 15 September (S1: "will ship by 15 October"). Due Friday 6 November, changed from Thursday 15 October by Tom (S4), who owes the work. Status: DONE. Evidence: R2, 6 November, "Route-report export fix released to all customers." Suggested owner: Tom. Nothing further.

THEIR COMMITMENTS

C1 Ines to send the list of depot users who need accounts. Made 15 September (S1: "by 25 September"). Due Friday 2 October, changed from Friday 25 September by Ines (S3: "The list will come to you on Friday"), agreeing to the date Maya asked for in S2. Status: DONE. Evidence: R1, 5 October, "Depot user list received from Ines (depot-users.xlsx)." Suggested owner: Ines. Nothing further.

C6 Ines to name a second administrator. Made 20 October (S4: "We'll name a second administrator next week"). Due Friday 30 October (read as). Status: OPEN, PAST DUE. Evidence: none; no source or record shows it done. That is not evidence it was not done. Suggested owner: Ines.

C4 Paul to find out whether the single sign-on certificate renews in November. Made 15 September (S1). Due: not stated. Status: OPEN. Evidence: none; no source or record shows it done. Suggested owner: Paul.

SIDE NOT STATED

C7 The September invoice to be corrected to show the right purchase order number. Made 20 October (S4); the notes do not say who said it. Due: not stated. Status: UNCLEAR, side not stated. Evidence: none; no source or record shows it done. Suggested owner: Maya, to establish whose it is.

NOT ON THE DRAFT AGENDA
Draft agenda supplied: 3 items (Renewal timeline; Dispatch module demo; Seat usage). Open or unclear items with no matching agenda line: C5, C6, C4, C7.

DECISIONS FOR MAYA: 4
1. C5, ours, past due since Friday 23 October. S4 has you saying you would send the dispatcher training options that week, and no source or record shows they were sent. Complete it, renegotiate the date, or leave it?
2. C6, theirs, past due since Friday 30 October. In S4 Ines said Customer A would name a second administrator the next week, and no source or record shows a name given. Chase it, renegotiate the date, or leave it?
3. C4, theirs, no due date. In S1 Paul said he would find out whether the single sign-on certificate renews in November, and no source records an answer. Chase it, renegotiate the date, or leave it?
4. C7, side not stated. The notes of S4 say the September invoice will be corrected but not who said it; you, Tom and Ines attended. Whose is it first?

Draft for Maya's review. Nothing has been sent to Customer A and no record has been changed.
```

## What was observed

Every required part of the format was produced, and no stop condition was met on these inputs: the headers matched, the dates were all present, no source held a password or a dispute, and no one asked for a message to the customer.

The counts were checked against the lines: 3 ours, 3 theirs, 1 side not stated; 3 done, 3 open, 1 unclear; 2 past due (C5 and C6).

Differences from the published example:

- The example leaves out the "Left out:" line, which the output format requires. This run printed "Left out: none."
- The format fixes the sentence "That is not evidence it was not done." The example rewords it for each item ("they were not sent", "none was given"). This run used the fixed sentence.
- For items with no evidence the format says "none; no source or record shows it done". The example prints only "none" for C4 and C7. This run printed the full form.
- In the decision about C7 the example says "you and Tom were both present". Ines also attended the 20 October call, so this run named all three.
- The example adds "three days after the agreed date" to C1. That is true of the inputs (agreed 2 October, received 5 October), but the template does not ask for it, so this run left it out.
- Wording of the status and decision lines differs slightly. The facts, the numbering, the order of the lines, the counts, the coverage line and the agenda result are the same.

Every fact in this output and in the example comes from the inputs. The only derived facts are the weekday names, the day counts and the dates read from relative wording, each of which follows a stated rule.

Where the template was ambiguous, and what was decided:

1. **"Nothing further."** The format shows it in brackets without saying when to print it. It was printed on items marked done and left off the others, as the example does.
2. **A bare weekday.** Ines wrote "on Friday". Step 6 covers "this week", "next week", "end of the month" and "tomorrow" but not a bare weekday. Context settled it (Maya had asked for Friday 2 October), and it was not marked "read as".
3. **Merging a soft and a firm statement (C5).** The soft wording in S1 was about finding a time for a training session, and the firm statement in S4 was about sending training options. Those are related but arguably not the same action. The template and its acceptance test 4 say to merge, so they were merged, with the original wording named.
4. **A commitment with nobody named (C7).** "The invoice will be corrected" names no person or side, while step 3 defines a commitment as something a named person or side will do. It was listed, as acceptance test 7 expects, and the side was not guessed even though invoices are usually ours.
5. **Notes are not quotes.** Most of S1 and S4 is a note-taker's summary, not spoken words, but the format asks for a "short quote". The note text was used as the quote.
6. **Undated open items (C4).** Nothing says how to treat an open item with no due date; it cannot be past due. It was listed as open and raised in the decisions.
7. **A gap of exactly 21 days.** S3 to S4 is 21 days, and the rule says "more than 21", so it was not reported. A reader could expect it to be.
8. **A meeting that was a future booking.** Tom's 3 November call was upcoming when S4 was written and is past by the prepared date. It was reported as referred to, not supplied.
9. **The instruction block is shorter than the template.** The block does not give the defaults of 21 days and the default owners, and does not repeat the rule for a dispute in a source (put it first in the decisions) or for two sources giving different dates. Someone who pastes only the block will lose these. This run took the 21 days from the example's settings.

The run took one pass and needed no questions to the person.

Changed after the run recorded above, and not run again. The output and the observations above are as recorded and describe the template and the example as they stood at the run:

- **The pasted instructions** now carry the defaults (the account manager as default owner for our side, the customer's day-to-day contact for theirs, a gap length of 21 days) and the rules that were only in the procedure: a dispute, complaint or threat to cancel goes first under the decisions; two sources with different dates for one promise; a record dated before the commitment does not count as done; a missing next-conversation date gives "next conversation not set" and skips the agenda check; "tomorrow" is a relative date; the no-evidence wording; "Left out: none."
- **The five open ambiguities** now have a sentence each in the template and the pasted instructions: "Nothing further." ends a DONE line and no other; a bare weekday is a stated date when the thread names the date, otherwise read as the first such weekday after the source date and marked "read as"; a note-taker's summary is the quote; an open item with no due date offers "agree a date" in place of "renegotiate the date"; a gap of exactly the gap length is not reported. Where the run had decided these the same way, nothing in the example changed.
- **Merging a soft and a narrower firm promise (C5).** The template now says a later firm promise to take a related, narrower action counts as firming up the soft one. The example's single line for C5 stands.
- **The example** now follows the output format as this run did: a "Left out: none." line, the fixed sentence "That is not evidence it was not done.", the full no-evidence wording for C4 and C7, all three attendees in the decision on C7, and the template's options in the decisions on C4 ("agree a date") and C7 ("Whose is it first?").
- **Further minor fixes after review, not run again.** The example now follows the format's fixed no-evidence wording for C5 and C6 as well, writes C1's date change in the format's form without the added "three days after the agreed date", and offers the template's plain options in the decision on C5. The template and the pasted instructions now say that a promise with nobody named is listed with the side not stated, that a shared promise goes under the side that will do the work (the format has no "both" section), that a promise which cannot be put as one action is unclear, and that coverage also reports a gap from the start of the period to the first source and a meeting that was only booked when mentioned and has since passed. The output format's empty-section placeholder now matches the "None." rule. Ambiguities 4 and 8 above are now answered in the template; the recorded output and observations are unchanged, and the example's facts, counts and order are unchanged.
- **The template** now names the sales call preparation brief among the different pieces of work, and its customization line about records is about what the person gathers and pastes in. The profile states this trial.

