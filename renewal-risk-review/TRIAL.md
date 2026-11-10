# Renewal risk review: a trial run on the invented example

- **Product:** Claude, run in Claude Code
- **Model:** Claude Opus 5.5 (model ID claude-opus-5-5)
- **Date:** 2026-11-09

The inputs were the invented example in `public/example.md`: its settings, warning signs, verdict rule and next steps, contract list, owners' notes and last month's review. No client data was used.

This record replaces the record of an earlier run on the same day. After that run a reviewer asked for changes: the starter list and the default settings were moved into the instruction block, rules were added for checking each account against last month, for plays carried out by two people, for an owner who is also the reviewer, for signs read from notes, for a blank notice date on a contract that renews on signature, for citing a note in a record-gap question, for steps belonging to accounts that have left the window, and for the date style. The invented company's warning signs, verdict rule and next steps were also rewritten so that they are its own rather than the starter list, and its watch response time changed from 14 to 10 days. The earlier run is not comparable with this one, so its page is not kept here.

## How the run was made

The session that revised the template started a new session of the same model with no tools, no access to the folder and no earlier conversation. Its instructions were the fenced instruction block followed by the output format, exactly as the template says to paste them. Its one message was the example's inputs, sections 1 to 5, with a one-line request to prepare the review. It never saw the example's output, this record or the earlier trial. The run was blind.

The example's published output was worked out from the inputs by the session that revised the template, and written up after this run.

## What came out

The page below is the run's reply, unedited.

```
RENEWAL RISK REVIEW: November 2026

For: Head of customer success. Run date 2 November 2026. Window: 2 November 2026 to 2 March 2027 (120 days). Lead time: 60 days.
Sources: contract list, CRM export of 2 November 2026, 8 rows; warning signs: your organization's; owners' notes; last month's review, run 1 October 2026.
Not supplied: nothing.
In the window: 7 accounts, 173,100; 1 without a value. At risk 3, 109,500. Watch 2, 21,600. Steady 2, 42,000 (1 without a value). Outside the window: Customer E (contract end 31 March 2027).

AT RISK: 3

Customer A. Owner: Account manager 1. Contract end 31 December 2026. Notice by 30 November 2026. Renews automatically. Annual value 18,000. Deadline 30 November 2026; start by 1 October 2026, passed.
Signs: New decision-maker (heavy): Contact change "yes"; the note of 14 October 2026 from Account manager 1 says a new operations manager now signs off on software and the owner has not met them. Quiet (light): Last contact 8 September 2026, 55 days before the run date. Open tickets (light): Open issues "2"; the note of 14 October 2026 from Account manager 1 says two mobile app sync problems are still open. Usage down (light): Usage trend "down". Price pressure is absent. Context: Auto-renews (Renews "auto"). Unknown: none.
Next steps: 6.
1. Account manager 1 phones the main contact. Owner: Account manager 1. Due: 9 November 2026. (Quiet; the same step was carried from last month)
2. Account manager 1 arranges an introduction meeting with the new decision-maker. Owner: Account manager 1. Due: 9 November 2026. (New decision-maker)
3. The support lead resolves the 2 open tickets and tells Account manager 1 when they are closed. Owner: Support lead. Due: 9 November 2026. (Open tickets)
4. Account manager 1 runs a usage check-in with the customer's main users. Owner: Account manager 1. Due: 9 November 2026. (Usage down)
5. The Head of customer success calls the customer's senior contact. Owner: Head of customer success. Due: 9 November 2026. (Rule: any account at risk)
6. Account manager 1 books the renewal meeting. Owner: Account manager 1. Due: 9 November 2026. (Rule: start-by passed and Renewal opened "no")

Customer G. Owner: Head of customer success. Contract end 10 February 2027. Notice by 11 December 2026. Renews automatically. Annual value 64,000. Deadline 11 December 2026; start by 12 October 2026, passed.
Signs: Usage down (light): Usage trend "down"; the note of 29 October 2026 from the Head of customer success says logins have dropped since the customer's busy season ended. The start-by date has passed, so the rule makes this account at risk. Quiet, New decision-maker, Open tickets and Price pressure are absent. Context: Auto-renews (Renews "auto"). Unknown: none.
Next steps: 3. The account owner is also the reviewer, so every step stays with the Head of customer success.
1. The Head of customer success runs a usage check-in with the customer's main users. Owner: Head of customer success. Due: 9 November 2026. (Usage down)
2. The Head of customer success calls the customer's senior contact. Owner: Head of customer success. Due: 9 November 2026. (Rule: any account at risk)
3. The Head of customer success books the renewal meeting. Owner: Head of customer success. Due: 9 November 2026. (Rule: start-by passed and Renewal opened "no")

Customer D. Owner: Account manager 2. Contract end 15 December 2026. Notice by none. Renews on signature. Annual value 27,500. Deadline 15 December 2026; start by 16 October 2026, passed.
Signs: New decision-maker (heavy): Contact change "yes". Price pressure (heavy): the note of 20 October 2026 from Account manager 2 says the customer's finance director is reviewing all software spend for next year and wants to see our price against two alternatives. Quiet, Open tickets and Usage down are absent. Context: none. Unknown: none.
Next steps: 3.
1. Account manager 2 arranges an introduction meeting with the new decision-maker. Owner: Account manager 2. Due: 9 November 2026. (New decision-maker)
2. Account manager 2 prepares the renewal case with the Head of customer success before price is discussed. Owner: Account manager 2. Due: 9 November 2026. (Price pressure)
3. The Head of customer success calls the customer's senior contact. Owner: Head of customer success. Due: 9 November 2026. (Rule: any account at risk)

WATCH: 2

Customer C. Owner: Account manager 1. Contract end 28 February 2027. Notice by 29 January 2027. Renews automatically. Annual value 9,600. Deadline 29 January 2027; start by 30 November 2026.
Signs: Open tickets (light): Open issues "1". Quiet, New decision-maker, Usage down and Price pressure are absent. Context: Auto-renews (Renews "auto"). Unknown: none.
Next steps: 1.
1. The support lead resolves the open ticket and tells Account manager 1 when it is closed. Owner: Support lead. Due: 12 November 2026. (Open tickets)

Customer H. Owner: Account manager 1. Contract end 20 February 2027. Notice by none. Renews on signature. Annual value 12,000. Deadline 20 February 2027; start by 22 December 2026.
Signs: Quiet (light): Last contact 31 August 2026, 63 days before the run date. New decision-maker, Open tickets, Usage down and Price pressure are absent. Context: none. Unknown: none.
Next steps: 1.
1. Account manager 1 phones the main contact. Owner: Account manager 1. Due: 12 November 2026. (Quiet)

STEADY: 2

Customer F. Owner: Account manager 2. Deadline 15 January 2027; start by 16 November 2026. Annual value not stated. Context: Auto-renews (Renews "auto"). Unknown: none. See record gaps.

Customer B. Owner: Account manager 2. Deadline 31 January 2027; start by 2 December 2026. Annual value 42,000. Context: none. Unknown: none.

CALENDAR
* 30 November 2026: Customer A, at risk, 18,000, start by 1 October 2026, passed.
* 11 December 2026: Customer G, at risk, 64,000, start by 12 October 2026, passed.
* 15 December 2026: Customer D, at risk, 27,500, start by 16 October 2026, passed.
* 15 January 2027: Customer F, steady, not stated, start by 16 November 2026. See record gaps.
* 29 January 2027: Customer C, watch, 9,600, start by 30 November 2026.
* 31 January 2027: Customer B, steady, 42,000, start by 2 December 2026.
* 20 February 2027: Customer H, watch, 12,000, start by 22 December 2026.

EXPANSION SIGNS: 2
* Customer G, at risk: Expansion talks "yes". The note of 29 October 2026 from the Head of customer success says the customer asked about adding the inventory module for its second depot. For the Head of customer success to consider. The owner decides whether to raise it before the renewal is settled.
* Customer B, steady: Expansion talks "yes". For Account manager 2 to consider.

RECORD GAPS: 2
* Customer F: Notice by (31 January 2027) is after the contract end (15 January 2027). Used: the contract end, 15 January 2027, as the deadline. Question for the Operations coordinator: which date is correct, the contract end of 15 January 2027 or the notice date of 31 January 2027? The note of 30 October 2026 from Account manager 2 reports that the customer asked to move the contract end to 31 January. That note is cited here only and was not used to settle the dates. Whether the contract can change is a question for the Operations director.
* Customer F: Annual value is blank. Used: not stated, and the account is counted separately from the totals. Question for the Operations coordinator: what is the annual value of this contract?

SINCE LAST MONTH
Changed:
* Customer A, watch to at risk.
* Customer C, steady to watch.
* Customer D, steady to at risk.
* Customer G, steady to at risk.
* Customer F had no change and stays steady.

New in the window: Customer B, Customer H. Left the window or the list: none.
Carried: Account manager 1 phones the main contact of Customer A, owner Account manager 1, due 15 October 2026, not reported done. This step is repeated in this month's next steps.

NOTES TO CHECK:
* "Their office manager asked us to change the contract end to 31 January so it matches their notice date." Source: note of 30 October 2026 from Account manager 2, Customer F. This was left undone. Changing the record is for the Operations coordinator. Whether the contract end can change is for the Operations director.

Prepared for Head of customer success. Nothing has been sent, no customer has been contacted and no record has been changed.
```

## What was observed

**Every required part was produced:** header, at risk, watch, steady, calendar, expansion signs, record gaps, since last month, notes to check and the closing line. Nothing in the inputs should make it stop, and it did not stop. The inputs have no missing required column, no unmatched header, no duplicate row, no unreadable date, no notice received and no request for a price, so none of the stop conditions was tested.

**Compared with the published example:** the verdicts, deadlines, start-by dates, values, totals, order, calendar, next steps with their owners and due dates, expansion signs, record gaps, changes since last month, the carried step and the note to check all match. Customer C's change from steady to watch, which the earlier run missed, was listed.

**The new rules, where the example reaches them:**
- Customer G's owner is also the reviewer; the run kept every step under that one role and said so.
- The two plays that name two roles (open tickets; price pressure) were owned by the first role named: the support lead and the account owner.
- Customer D and Customer H have no notice date and renew on signature; the run wrote "Notice by none" and raised no record gap.
- Price pressure, a sign read from notes, was treated as absent on accounts with no note that shows it, not as unknown.
- The note about Customer F's contract end was cited in the record-gap question and not used to settle the date.
- Dates were written in full, though the export uses YYYY-MM-DD.

**Departures from the format, none of which changes a result:**
- It listed the absent signs on each account ("Price pressure is absent"). The format asks only for the signs found, the context signs and the unknown ones.
- Under Since last month it added a line saying Customer F had not changed. The format asks only for the changes.
- It added "(1 without a value)" to the steady total, and Customer E's contract end beside its name in the header.
- In the record-gap question and the note to check it added that whether the contract can change is for the operations director. That is a fair pointer to the contracts role, but goes beyond the format.
- It wrote amounts without a currency, as the export does. The example does the same.

**Facts not in the inputs:** none found. Every date and total can be worked out from the inputs, and every note quoted is in the notes. The 55 and 63 days since last contact are computed, and are correct.

**A second, shorter check of the fallback.** The same fresh-session setup was run once more with section 2 (the warning signs, verdict rule and next steps) left out of the inputs. The header read "warning signs: starter list, not yet set by your organization", and the run used the starter signs, verdict rule and plays from the instruction block alone. Under the starter list's 60-day threshold, Customer A's 55 days without contact is not a sign, and the run treated it as absent; the verdicts came out the same, with one fewer next step for Customer A. It added a sentence before the page saying the starter list was used. That run's page is not reproduced here.

**Where the instructions still left a choice:** whether to show absent signs, and whether to mention accounts whose verdict did not change. The run chose to show both; the example shows neither.

**Edited after the recorded run (2026-11-09).** The template was edited after this run, which was not repeated. The instruction block and the procedure now say to show only the signs found, the context signs and the unknown ones, and to list under Since last month only the accounts whose verdict changed, which settles the choice above in the example's favour. They also now stop when no contract list is supplied, repeat in the block that context signs never cancel a risk sign under the starter verdict, and add a record gap when the notice date has passed on a contract that renews automatically. The output format, the example's inputs and the page above are unchanged.

**Shortcomings of the trial itself:** one recorded run and one fallback check, one model, one invented example. The model that ran it is the same model as the session that revised the template, in a fresh session. It shows the template can be followed to the same answer from the pasted instructions alone; it does not show how it behaves on a messy real export, a notice-received case or a missing column.
