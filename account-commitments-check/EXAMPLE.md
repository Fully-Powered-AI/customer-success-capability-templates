# Account commitments check: an invented example

*Illustrative example with invented data.* An invented 40-person software company prepares for a conversation with Customer A, an invented 120-person logistics firm. The people are invented too: Maya, our account manager; Tom, our support lead; Ines, Customer A's operations director; Paul, Customer A's IT lead.

## What the person supplies

**Settings.** Account: Customer A. Period: 1 September to 16 November 2026. Today: Monday 16 November 2026. Next conversation: Thursday 19 November 2026. Account manager: Maya. Gap length: the default, 21 days.

**People.** Maya, our side, account manager. Tom, our side, support lead. Ines, Customer A, operations director. Paul, Customer A, IT lead.

**Draft agenda for 19 November.** Renewal timeline. Dispatch module demo. Seat usage.

**Source 1.** Meeting, Tuesday 15 September 2026, "Quarterly check-in". Attendees: Maya, Tom, Ines, Paul. Notes:
- Ines said Customer A will send the list of depot users who need accounts by 25 September.
- Maya said she will confirm the price for the extra 30 seats before the end of September.
- Tom said the fix for the slow route-report export is in testing and will ship by 15 October.
- Paul will find out whether the single sign-on certificate renews in November.
- Ines would like a training session for dispatchers. Maya said "we'll try to find a time".

**Source 2.** Email, Monday 28 September 2026, Maya to Ines: "Hi Ines, the prices for the extra 30 seats are attached. Could you send the depot user list by Friday 2 October? We had it down for the 25th, and we need it to set up the accounts."

**Source 3.** Email, Tuesday 29 September 2026, Ines to Maya: "Thanks Maya. The list will come to you on Friday."

**Source 4.** Meeting, Tuesday 20 October 2026, "Support review call". Attendees: Maya, Tom, Ines. Notes:
- Tom said the route-report export fix has slipped; the new date is 6 November.
- Ines said "We'll name a second administrator next week."
- Maya said "I'll send you the training options this week."
- The September invoice will be corrected to show the right purchase order number.
- Tom has a call with Customer A's finance team on 3 November.

**Follow-through records.** Export with the headers Date, Reference, What happened:
- 2026-10-05, Ticket 3318: "Depot user list received from Ines (depot-users.xlsx)."
- 2026-11-06, Release 4.12: "Route-report export fix released to all customers."

## What comes out

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

C2 Maya to confirm the price for the extra 30 seats before the end of September. Made 15 September (S1: "before the end of September"). Due Wednesday 30 September (read as). Status: DONE. Evidence: S2, 28 September, email with the prices attached. Terms: price; check against the agreement. Suggested owner: Maya. Nothing further.

C5 Maya to send the dispatcher training options. Made 20 October (S4: "I'll send you the training options this week"); first raised 15 September (S1) as "we'll try to find a time", which was soft wording. Due Friday 23 October (read as). Status: OPEN, PAST DUE. Evidence: none; no source or record shows it done. That is not evidence it was not done. Suggested owner: Maya.

C3 Tom to ship the fix for the slow route-report export. Made 15 September (S1: "will ship by 15 October"). Due Friday 6 November, changed from Thursday 15 October by Tom (S4), the person who owes it. Status: DONE. Evidence: R2, 6 November, "Route-report export fix released to all customers." Suggested owner: Tom. Nothing further.

THEIR COMMITMENTS

C1 Ines to send the list of depot users who need accounts. Made 15 September (S1: "by 25 September"). Due Friday 2 October, changed from Friday 25 September by Ines (S3: "The list will come to you on Friday"), agreeing to the date Maya asked for in S2. Status: DONE. Evidence: R1, 5 October, "Depot user list received from Ines (depot-users.xlsx)." Suggested owner: Ines. Nothing further.

C6 Ines to name a second administrator. Made 20 October (S4: "next week"). Due Friday 30 October (read as). Status: OPEN, PAST DUE. Evidence: none; no source or record shows it done. That is not evidence it was not done. Suggested owner: Ines.

C4 Paul to find out whether the single sign-on certificate renews in November. Made 15 September (S1). Due: not stated. Status: OPEN. Evidence: none; no source or record shows it done. Suggested owner: Paul.

SIDE NOT STATED

C7 The September invoice to be corrected to show the right purchase order number. Made 20 October (S4); the notes do not say who said it. Due: not stated. Status: UNCLEAR, side not stated. Evidence: none; no source or record shows it done. Suggested owner: Maya, to establish whose it is.

NOT ON THE DRAFT AGENDA
Draft agenda supplied: 3 items (Renewal timeline; Dispatch module demo; Seat usage). Open or unclear items with no matching agenda line: C5, C6, C4, C7.

DECISIONS FOR MAYA: 4
1. C5, ours, past due since Friday 23 October. You said you would send the dispatcher training options that week and no record shows they went. Complete it, renegotiate the date, or leave it?
2. C6, theirs, past due since Friday 30 October. Ines said Customer A would name a second administrator the following week and no record shows a name. Chase it, renegotiate the date, or leave it?
3. C4, theirs, no due date. Paul said he would find out whether the single sign-on certificate renews in November and no source records an answer. Chase it, agree a date, or leave it?
4. C7, side not stated. The notes of the 20 October call do not say who promised the invoice correction; you, Tom and Ines were all present. Whose is it first?

Draft for Maya's review. Nothing has been sent to Customer A and no record has been changed.
```
