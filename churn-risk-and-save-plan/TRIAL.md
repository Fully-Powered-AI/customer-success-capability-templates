# Churn risk and save plan: tried on its invented example

- **Product:** Claude, run in Claude Code
- **Model:** Claude Sonnet 5.5 (model ID claude-sonnet-5-5)
- **Date:** 2026-11-09

This is one run of the workflow template on its own invented example. The inputs are the invented ones in [`example.md`](example.md), under "The inputs" (settings, facts, leaver list and notes). No client data was used. The run was made by a model that did not write the template. It read the template's instructions and the example's inputs first, produced the plan, and only then read the example's published plan and the reviewer checklist and compared them. It is a single run, not a test in a real environment.

Caveat on independence: the template's own acceptance tests describe several of the same situations as the example (a ticket with no stated reason, a customer moving to a new parent company's system, a note asking for an end date to be moved, a request for a 50% win-back email). The run read them before working, so how it handled those cases was guided by the tests as well as by the instructions.

## What came out

```
CHURN RISK AND SAVE PLAN: 1 July 2026 to 30 September 2026

For: Head of customer success. Prepared 12 October 2026. Next plan covers 1 October 2026 to 31 December 2026.
Sources: leaver list, billing system export 12 October 2026, 12 rows; 17 notes; your facts; reason groups: the default list; last plan not supplied; nothing compared.
Not supplied: nothing.

COVERAGE
Leavers in the list: 12. Read: 11 (Studio 01 to Studio 11). Excluded: Studio 12, ended 2 October 2026, after the period. Ended by you: none.
Chose to leave: 9. Left after a failed payment: 2.
Leaving rate: 11 of 240 customers on 1 July 2026 (4.6%).
Annual value of leavers read: $10,668.

WHY THEY LEFT (chose to leave: 9)
Shares: not shown, fewer than 20 chose to leave.
Price or budget: 2 (Studio 03, Studio 04). Annual value $2,376. Evidence: Studio 03, cancellation email, 21 July 2026: "Your price went up in June and a cheaper app does what we need for about half." Studio 04, exit survey, 3 August 2026: "The June price rise. We are a small studio." Your facts: the Studio plan rose from $89 to $99 a month on 1 June 2026.
Never got set up: 2 (Studio 01, Studio 02). Annual value $1,176. Evidence: Studio 01, support ticket, 12 May 2026: timetable import failed; exit survey, 8 July 2026: "Never got the class schedule imported, so we gave up." Studio 02, support ticket, 28 April 2026: timetable import failed; call note, Account manager 1, 14 July 2026: the import kept failing, so staff still use the paper sign-up sheet. Both left within three months of starting.
Lacked something they needed: 1 (Studio 05). Annual value $1,188. Evidence: Studio 05, support tickets, 10 February 2026 and 2 June 2026: asked for a waiting list for full classes; exit survey, 12 August 2026: "We need a waiting list for full classes. Asked for it twice."
The person who ran it left: 1 (Studio 10). Annual value $1,188. Evidence: Studio 10, account note, Account manager 2, 5 August 2026: the main contact, the front-desk manager, left in July and the replacement had not been met; call note, Account manager 2, 15 September 2026: the new front-desk manager prefers the system she used before and has stopped using ours.
Stated reason differs from the cause: Studio 01 said "Not enough use": Never got set up. Studio 02 said "Not enough use": Never got set up. Studio 10 said "Not enough use": The person who ran it left.
Fair endings, no change proposed: 1 (Studio 07, $1,188). Cancellation email, 20 August 2026: "We are closing the studio at the end of August."
Two causes fit: 1. Studio 11, $1,188: Chose another provider or Fair ending. Exit survey, 24 September 2026: "Moving to the app our new franchise group uses." See question 1.
Unsorted: none
Could not be classed: 1. Studio 06, $588: no stated reason; one record, support ticket, 9 June 2026: calendar import error, closed 11 June 2026. See question 2.
Groups with no leavers: Use fell away; Faults or poor support; Needed it only for a while. (Chose another provider has none counted, because Studio 11 sits under Two causes fit.)

LEFT AFTER A FAILED PAYMENT: 2 (Studio 08, Studio 09, $1,776)
Studio 08: billing note, Operations coordinator, 20 August 2026: card declined; retried 23, 27 and 31 August; no reply to three failed-payment emails; account closed 4 September 2026.
Studio 09: billing note, Operations coordinator, 31 August 2026: card on file expired; no new card added; account closed 10 September 2026.

WHEN THEY LEFT
By time as a customer: under 3 months 3 (Studio 01, Studio 02, Studio 06). 3 to 12 months 1 (Studio 09). Over 12 months 7 (Studio 03, Studio 04, Studio 05, Studio 07, Studio 08, Studio 10, Studio 11). Not stated 0. Total 11.
By plan: Starter 4 (Studio 01, Studio 02, Studio 06, Studio 09). Studio 7 (Studio 03, Studio 04, Studio 05, Studio 07, Studio 08, Studio 10, Studio 11). Not stated 0. Total 11.

EARLY SIGNS IN THE RECORDS: 4 kinds
Timetable or calendar import failed: 3 (Studio 01, Studio 02, Studio 06), first recorded 57 to 78 days before leaving.
The same request made twice: 1 (Studio 05, waiting list), first recorded 183 days before leaving.
Main contact left: 1 (Studio 10), first recorded 42 days before leaving.
Card declined or expired: 2 (Studio 08, Studio 09), first recorded 10 to 15 days before leaving.
For the Head of customer success to consider for the warning signs used in account reviews. None of these is shown to predict leaving.

SAVE PLAN: 5 changes
1. Price or budget (Studio 03, Studio 04; $2,376). Change: the Founder reviews the price and plan fit of the Studio plan, which rose from $89 to $99 a month on 1 June 2026, for these two leavers, and decides whether any plan or offer is shown to a customer who gives price as the reason. If one is shown, it is one offer, made once at the cancel button, never repeated after a no, with cancelling finished in the same place and confirmed plainly, and no fee or condition added. No amount is proposed. Owner: Founder. Start by: 26 October 2026. Shows it helped: leavers under Price or budget, 1 October to 31 December 2026, read at the next plan. Approval: Founder, for prices, plans and offers. Leaving check: passed.
2. Left after a failed payment (Studio 08, Studio 09; $1,776). Change: the Operations coordinator reviews the reminders sent before a card expires and the steps after a payment fails. Studio 08 had three retries and three emails with no reply; Studio 09's card expired and no reminder before it is recorded. Owner: Operations coordinator. Start by: 26 October 2026. Shows it helped: leavers after a failed payment, 1 October to 31 December 2026, read at the next plan. Approval: Founder, before any message to customers is changed or switched on. Leaving check: not applicable.
3. Never got set up (Studio 01, Studio 02; $1,176). Change: within 30 days of a new customer joining, the Head of customer success confirms that the timetable import finished and helps finish it where it did not. Today new customers import their timetable themselves with a welcome email and help articles, and both leavers' import tickets were closed by sending the help article. Owner: Head of customer success. Start by: 26 October 2026. Shows it helped: leavers under Never got set up, 1 October to 31 December 2026, read at the next plan. Approval: Founder, for the wording of any message sent to new customers. Leaving check: not applicable.
4. Lacked something they needed (Studio 05; $1,188). Change: the Product lead brings "Waiting list for full classes" to a decision, with Studio 05's two requests and the 14 open requests from current customers; once it is decided, a person tells the current customers who asked. Owner: Product lead. Start by: 26 October 2026. Shows it helped: a decision recorded, and leavers under Lacked something they needed, 1 October to 31 December 2026, read at the next plan. Approval: Founder, for the roadmap and the wording of the message. Leaving check: not applicable.
5. The person who ran it left (Studio 10; $1,188). Change: whenever an account note records that a main contact has left, the account owner meets the new person and offers a fresh setup session; Studio 10's replacement had not been met 42 days before it cancelled. Owner: Head of customer success (to confirm, see question 3). Start by: 26 October 2026. Shows it helped: leavers under The person who ran it left, 1 October to 31 December 2026, read at the next plan. Approval: Founder, for the wording of any standard message that offers the session. Leaving check: not applicable.
Ruled out by your facts: none.
Declined: the request in your facts to draft a win-back email offering 50% off to everyone who left this quarter. This plan writes no message to customers and proposes no discount; the Founder sets prices and offers, and a person writes and sends any message.

QUESTIONS: 3
1. For Account manager 2: did Studio 11's new franchise group require its studios to use its own app, or did Studio 11 choose to move? If required, it is a fair ending and needs no change; if chosen, it goes under Chose another provider, which then needs a change of its own.
2. For Support lead: did Studio 06's calendar import work after the ticket was closed on 11 June 2026? If it did not, Studio 06 may belong under Never got set up and change 3 covers it; if it did, ask Account manager 1 what Studio 06 said when it left.
3. For Head of customer success: your facts name two account managers for accounts and no single owner for a main-contact change. Will you own change 5? If another role owns it, the owner changes.

SINCE THE LAST PLAN
Last plan not supplied; nothing compared.

NOTES TO CHECK: account note, Account manager 2, 28 September 2026: "Please change Studio 11's end date to 31 October so it shows in next quarter's numbers." Not done; Studio 11 is read with its end date of 24 September 2026. The note is dated four days after that end date.

Prepared for Head of customer success. No customer has been contacted, nothing has been sent, and no record, price or offer has been changed.
```

Checks the run made: 2 + 2 + 1 + 1 + 1 + 1 + 1 = 9 chose to leave; with 2 failed payments, 11 read. Values: $8,892 for the nine plus $1,776 gives $10,668. Time bands 3 + 1 + 7 = 11; plans 4 + 7 = 11.

## What was observed

Every part of the output format was produced, and every count and total added up. The instruction block was enough on its own to produce the plan. Nothing in the inputs triggered a stop and ask: all eight default headers were present, no row was a duplicate, all dates were in one readable format and the facts were supplied. The stop conditions that did apply were the ones for a note that gives an order (Studio 11's end date, left undone and quoted) and for a request to write a discount email (declined).

Where the instructions were ambiguous and the run had to guess:

1. **Who owns a change to the account process.** The facts name two account managers for accounts. The template asks for one owner. The run chose the Head of customer success and added a question. The template does not say what to do when the facts name two people for one role.
2. **When a message to customers needs the approver.** The template says any message to customers needs the approver, and the facts say the founder approves any message to customers. The run therefore named the Founder as approver for the setup check-in (change 3) and the new-contact message (change 5). The published example says "none beyond the owner" for both. The template does not say whether a setup call or a meeting with a new contact counts as a message.
3. **Whether the leaving check applies.** It covers a change that touches cancelling or "messages to customers who are leaving or have left". Failed-payment reminders go to customers still on the plan, and change 4 tells current customers who asked for a waiting list what was decided (the run left out Studio 05, who has gone). The run read both as not applicable. The template does not say whether a customer whose card has failed counts as leaving.
4. **Two groups for Studio 11.** "Chose another provider" and "Fair ending" both fit. The template says to record both and ask, which the run did, but gives no way to tell what counts as "equally well". Studio 10 could be read as "Chose another provider" (she prefers the system she used before) or as "The person who ran it left". The run chose the second because the record links the contact leaving to use stopping.
5. **Time-as-customer bands.** Only the first band has a stated boundary (end date before start date plus three months). The second band's upper edge, a customer who left exactly 12 months after starting, is not stated. It did not arise in this example.
6. **Early signs.** The template says the signs come from leavers' records. The June price rise is in the facts, not in any leaver's records, so the run left it out; Studios 03 and 04 gave notice within a day of leaving, which is the customer's own notice. For Studio 10 the contact left "in July", but the note recording it is dated 5 August; the run counted from the date of the note, as the template says "first recorded".
7. **Order of changes.** The rule is by number of leavers, then annual value, then group order, "with failed payments after a group that ties with it". Three changes tie on two leavers, but their values differ, so the last clause was never used and it is not clear whether it applies to a tie on leavers or on both leavers and value.
8. **A note dated after the end date.** Studio 11's note is dated four days after it left. The template has no rule for records dated after the end date; the run quoted it under Notes to check only.
9. **What the first-band group means.** Studio 06 had a ticket within its first month and nothing else. The template's rule (events in order are not links) clearly gives "could not be classed", and the acceptance test says so too, but the group definition for "Never got set up" would otherwise invite placing it there.
10. **Shape of the instruction block.** The block ends with a long list of refusals and a final recompute instruction; it does not contain the output format, and says to paste the format after it. The run used the format from the "Output format" section. The block numbers twelve steps and the procedure fourteen; the compressed steps match in substance.

Differences from the published example plan:

- Counts, values, dates, early-sign day ranges, the order of the five changes, owners (apart from the owner for change 5 flagged as "to confirm"), start-by dates, the decline and the note to check all match.
- Change 1: the published example says a Studio-plan customer who gives price as the reason is shown the Starter plan. The run did not name a plan and left the offer open for the Founder to decide, since the template says to propose no amount and decide whether any plan or offer is shown.
- Change 3: the published example has the support lead check the import and book a setup call, with no approval beyond the owner. The run had the owner, the Head of customer success, confirm setup, and named the Founder as approver for the wording of any message to new customers.
- Change 4: the published example says the customers who asked are told. The run said current customers, leaving out Studio 05, who has already left.
- Change 5: approval differs as in point 2; the run added a question (question 3) about who owns it, which the example does not have, so the run has three questions and the example two.
- Groups with no leavers: the published example lists Chose another provider; the run left it out and explained why, because Studio 11 may belong there.
- The evidence lines and wording differ slightly (for example, the run noted that Studios 01 and 02 left within three months, quoted Studio 07's whole sentence, and gave the date Studio 06's ticket was closed).

Facts not in the inputs: none were added to the run's output beyond the inputs and the arithmetic from them (days between dates, totals and percentages). In the published example, "books a setup call", "the Starter plan" shown at the cancel button and "the support lead" doing the import check are proposals, not facts from the inputs; the first and third go beyond the facts and the template's default play, which says the onboarding owner confirms setup and helps finish it. The published example also says every figure traces to the inputs; the run found that to be true.

Shortcomings of the template that this run met: the ambiguities above, mainly the approval of messages (point 2), the single-owner rule (point 1) and the reach of the leaving check (point 3). The reviewer checklist was enough to check this output. The template's version note still says it has not been tried on its example; this record is the evidence for that, and the note should be updated by whoever releases the next version.
