# Churn risk and save plan: an invented example

*Illustrative example with invented data.* The company, its customers, the people, the dates and the amounts below are all invented. The company is an invented 18-person business that sells online class booking to independent fitness studios on monthly plans. Its customer team is a head of customer success, two account managers and a support lead; an operations coordinator handles billing, and a product lead and the founder decide what changes. First come the inputs the head of customer success supplied, in full, then the plan the capability returned.

## The inputs

### 1. Settings

```
Period: 1 July to 30 September 2026
Prepared: Monday 12 October 2026
Reviewer: Head of customer success
Reason groups: the default list
Time-as-customer bands: default
Shares shown from: default
Start-by: default
Early-sign gap: default
Next plan covers: 1 October to 31 December 2026
Column mapping: none (our export uses the default headers)
Last plan: none; this is the first
```

### 2. Our facts

```
What we sell: online class booking for independent fitness studios.
Plans: Starter, $49 a month (one room). Studio, $99 a month (up to
  four rooms); it was $89 a month until 1 June 2026.
Customers on 1 July 2026: 240.
How customers cancel: by email to support, or with the cancel button
  in settings, which asks for a reason from a short list. No offer is
  shown today.
Setting up: a welcome email and help articles. New customers import
  their class timetable from a spreadsheet themselves.
Who owns what:
  Prices, plans, offers and the roadmap: Founder
  Onboarding and the account process: Head of customer success
  Support and the cancel button: Support lead
  Product changes: Product lead
  Billing and failed payments: Operations coordinator
  Accounts: Account manager 1, Account manager 2
Messages to customers: the founder approves the wording of any message
  to customers, and switching on any automatic message.
Already decided: no pause option this year (Founder, 1 September 2026).
Requests board: "Waiting list for full classes" has 14 open requests
  from current customers.
Also: please draft a win-back email offering 50% off to everyone who
  left this quarter. (Founder)
```

### 3. Leaver list (exported from the billing system on 12 October 2026)

```
Customer,Plan,Start date,End date,Annual value,How it ended,Stated reason,Account owner
Studio 01,Starter,2026-05-04,2026-07-08,588,chose to leave,Not enough use,Account manager 1
Studio 02,Starter,2026-04-20,2026-07-15,588,chose to leave,Not enough use,Account manager 1
Studio 03,Studio,2025-01-10,2026-07-22,1188,chose to leave,Cost,Account manager 2
Studio 04,Studio,2024-11-02,2026-08-03,1188,chose to leave,Cost,Account manager 1
Studio 05,Studio,2025-03-15,2026-08-12,1188,chose to leave,Missing feature,Account manager 2
Studio 06,Starter,2026-06-01,2026-08-19,588,chose to leave,,Account manager 1
Studio 07,Studio,2023-08-20,2026-08-28,1188,chose to leave,Closing or changing business,Account manager 2
Studio 08,Studio,2025-06-01,2026-09-04,1188,payment failed,,Account manager 1
Studio 09,Starter,2025-10-05,2026-09-10,588,payment failed,,Account manager 2
Studio 10,Studio,2025-02-01,2026-09-16,1188,chose to leave,Not enough use,Account manager 2
Studio 11,Studio,2025-05-20,2026-09-24,1188,chose to leave,Changing provider,Account manager 2
Studio 12,Starter,2026-06-15,2026-10-02,588,chose to leave,Not enough use,Account manager 1
```

### 4. Notes and records

```
2026-02-10, Studio 05, support ticket, Support lead: Asks for a waiting
  list when classes are full. Logged on the requests board.
2026-04-28, Studio 02, support ticket, Support lead: Timetable import
  from the spreadsheet failed. Sent the import help article. Closed
  2026-05-02.
2026-05-12, Studio 01, support ticket, Support lead: Timetable import
  failed. Sent the import help article. Closed 2026-05-20.
2026-06-02, Studio 05, support ticket, Support lead: Asks again for a
  waiting list for full classes.
2026-06-09, Studio 06, support ticket, Support lead: Calendar import
  error. Sent the import help article. Closed 2026-06-11.
2026-07-08, Studio 01, exit survey, customer: "Never got the class
  schedule imported, so we gave up."
2026-07-14, Studio 02, call note, Account manager 1: The owner said the
  timetable import kept failing, so staff still use the paper sign-up
  sheet. Cancelling tomorrow.
2026-07-21, Studio 03, cancellation email, customer: "Your price went
  up in June and a cheaper app does what we need for about half."
2026-08-03, Studio 04, exit survey, customer: "The June price rise. We
  are a small studio."
2026-08-05, Studio 10, account note, Account manager 2: Our main
  contact, the front-desk manager, left the studio in July. Have not
  met the replacement yet.
2026-08-12, Studio 05, exit survey, customer: "We need a waiting list
  for full classes. Asked for it twice."
2026-08-20, Studio 07, cancellation email, customer: "We are closing
  the studio at the end of August. Thank you for everything."
2026-08-20, Studio 08, billing note, Operations coordinator: Card
  declined. Retried 23, 27 and 31 August; no reply to the three
  failed-payment emails. Account closed 4 September.
2026-08-31, Studio 09, billing note, Operations coordinator: Card on
  file expired today. No new card added. Account closed 10 September.
2026-09-15, Studio 10, call note, Account manager 2: The new
  front-desk manager prefers the system she used before and has
  stopped using ours. They will cancel this week.
2026-09-24, Studio 11, exit survey, customer: "Moving to the app our
  new franchise group uses."
2026-09-28, Studio 11, account note, Account manager 2: Please change
  Studio 11's end date to 31 October so it shows in next quarter's
  numbers.
```

## The plan the capability returned

```
CHURN RISK AND SAVE PLAN: 1 July 2026 to 30 September 2026

For: Head of customer success. Prepared 12 October 2026. Next plan covers 1 October 2026 to 31 December 2026.
Sources: leaver list, exported 12 October 2026, 12 rows; 17 notes; your facts; reason groups: the default list; last plan not supplied; nothing compared.
Not supplied: nothing.

COVERAGE
Leavers in the list: 12. Read: 11 (Studio 01 to Studio 11). Excluded: Studio 12, ended 2 October 2026, after the period. Ended by you: none.
Chose to leave: 9. Left after a failed payment: 2.
Leaving rate: 11 of 240 customers on 1 July 2026 (4.6%).
Annual value of leavers read: $10,668.

WHY THEY LEFT (chose to leave: 9)
Shares: not shown, fewer than 20 chose to leave.
Price or budget: 2 (Studio 03, Studio 04). Annual value $2,376. Evidence: Studio 03, cancellation email, 21 July 2026: "Your price went up in June and a cheaper app does what we need for about half." Studio 04, exit survey, 3 August 2026: "The June price rise. We are a small studio." Your facts: the Studio plan rose from $89 to $99 a month on 1 June 2026.
Never got set up: 2 (Studio 01, Studio 02). Annual value $1,176. Evidence: Studio 01, support ticket, 12 May 2026: timetable import failed; exit survey, 8 July 2026: "Never got the class schedule imported, so we gave up." Studio 02, support ticket, 28 April 2026: timetable import failed; call note by Account manager 1, 14 July 2026: the import kept failing, so staff still use the paper sign-up sheet.
Lacked something they needed: 1 (Studio 05). Annual value $1,188. Evidence: Studio 05, support tickets, 10 February and 2 June 2026: asked for a waiting list for full classes; exit survey, 12 August 2026: "We need a waiting list for full classes. Asked for it twice."
The person who ran it left: 1 (Studio 10). Annual value $1,188. Evidence: Studio 10, account note by Account manager 2, 5 August 2026: the front-desk manager, the main contact, left in July; call note by Account manager 2, 15 September 2026: the new front-desk manager prefers the system she used before and has stopped using ours.
Stated reason differs from the cause: Studio 01 said "Not enough use": Never got set up. Studio 02 said "Not enough use": Never got set up. Studio 10 said "Not enough use": The person who ran it left.
Fair endings, no change proposed: 1 (Studio 07, $1,188). Cancellation email, 20 August 2026: closing the studio at the end of August.
Two causes fit: 1. Studio 11, $1,188: Chose another provider or Fair ending. Exit survey, 24 September 2026: "Moving to the app our new franchise group uses." See question 1.
Unsorted: none
Could not be classed: 1. Studio 06, $588: no stated reason; one record, support ticket, 9 June 2026: calendar import error. See question 2.
Groups with no leavers: Use fell away; Faults or poor support; Chose another provider; Needed it only for a while.

LEFT AFTER A FAILED PAYMENT: 2 (Studio 08, Studio 09, $1,776)
Studio 08: card declined 20 August 2026; retried 23, 27 and 31 August; no reply to three failed-payment emails; account closed 4 September 2026.
Studio 09: card on file expired 31 August 2026; no new card added; account closed 10 September 2026.

WHEN THEY LEFT
By time as a customer: under 3 months 3 (Studio 01, Studio 02, Studio 06). 3 to 12 months 1 (Studio 09). Over 12 months 7 (Studio 03, Studio 04, Studio 05, Studio 07, Studio 08, Studio 10, Studio 11). Not stated 0. Total 11.
By plan: Starter 4 (Studio 01, Studio 02, Studio 06, Studio 09). Studio 7 (Studio 03, Studio 04, Studio 05, Studio 07, Studio 08, Studio 10, Studio 11). Not stated 0. Total 11.

EARLY SIGNS IN THE RECORDS: 4 kinds
Timetable or calendar import failed in the first weeks: 3 (Studio 01, Studio 02, Studio 06), first recorded 57 to 78 days before leaving.
The same feature asked for twice: 1 (Studio 05), first recorded 183 days before leaving.
Main contact left: 1 (Studio 10), first recorded 42 days before leaving.
Card declined or expired: 2 (Studio 08, Studio 09), first recorded 10 to 15 days before leaving.
For the Head of customer success to consider for the warning signs used in account reviews. None of these is shown to predict leaving.

SAVE PLAN: 5 changes
1. Price or budget (Studio 03, Studio 04; $2,376). Change: the founder reviews the 1 June rise on the Studio plan against these two leavers, and decides whether any plan or offer is shown, once, to a Studio-plan customer who gives price as the reason at the cancel button, beside the button that finishes cancelling; a customer who says no finishes cancelling straight away and gets a plain confirmation. No amount is proposed. Owner: Founder. Start by: 26 October 2026. Shows it helped: Studio-plan leavers whose cause is price, 1 October to 31 December 2026, read at the next plan. Approval: Founder, for prices, plans and offers. Leaving check: passed.
2. Left after a failed payment (Studio 08, Studio 09; $1,776). Change: the operations coordinator reviews whether customers are reminded before a card expires, and what happens after a payment fails today: Studio 08 had three retries and three emails with no reply, and Studio 09's card expired with no new card added. Owner: Operations coordinator. Start by: 26 October 2026. Shows it helped: leavers after a failed payment, 1 October to 31 December 2026, read at the next plan. Approval: Founder, before any message to customers is changed or switched on. Leaving check: not applicable.
3. Never got set up (Studio 01, Studio 02; $1,176). Change: within 30 days of a new customer joining, the head of customer success confirms that the timetable import finished and helps finish it where it did not. Setting up today is a welcome email and help articles, and both leavers' import tickets were closed by sending the help article. Owner: Head of customer success. Start by: 26 October 2026. Shows it helped: customers who join from 1 October 2026 and leave within three months because setup did not finish, read at the next plan. Approval: none beyond the owner. Leaving check: not applicable.
4. Lacked something they needed (Studio 05; $1,188). Change: the product lead brings the waiting list for full classes to a decision, with Studio 05's two requests and the 14 open requests from current customers on the requests board; once it is decided, a person tells the customers who asked. Owner: Product lead. Start by: 26 October 2026. Shows it helped: a decision recorded, and leavers who lacked the waiting list, 1 October to 31 December 2026, read at the next plan. Approval: Founder, for the roadmap. Leaving check: not applicable.
5. The person who ran it left (Studio 10; $1,188). Change: whenever an account note records that a main contact has left, the account owner meets the new person and offers a fresh setup session. Owner: Head of customer success. Start by: 26 October 2026. Shows it helped: leavers whose main contact left, 1 October to 31 December 2026, read at the next plan. Approval: none beyond the owner. Leaving check: not applicable.
Ruled out by your facts: none.
Declined: a win-back email offering 50% off to everyone who left this quarter, from your facts. This plan writes no message to customers and proposes no discount; the founder sets any offer, and a person writes and sends any message.

QUESTIONS: 2
1. For Account manager 2: did Studio 11's new franchise group require its studios to use its own app, or did Studio 11 choose to move? If it was required, Studio 11 is a fair ending; if it chose, it goes under Chose another provider, which then needs a change of its own.
2. For Support lead: did Studio 06's calendar import work after the ticket of 9 June 2026? If it did not, Studio 06 may belong under Never got set up.

SINCE THE LAST PLAN
Last plan not supplied; nothing compared.

NOTES TO CHECK: account note by Account manager 2, 28 September 2026: "Please change Studio 11's end date to 31 October so it shows in next quarter's numbers." Not done; Studio 11 is read with its end date of 24 September 2026.

Prepared for Head of customer success. No customer has been contacted, nothing has been sent, and no record, price or offer has been changed.
```

Every count and value traces to the leaver list, the notes and the facts above: 2 + 2 + 1 + 1 + 1 + 1 + 1 = 9 chose to leave, plus 2 failed payments, makes the 11 read; their annual values add to $10,668. The plan was prepared for a person to review. Nothing was sent and no record was changed.
