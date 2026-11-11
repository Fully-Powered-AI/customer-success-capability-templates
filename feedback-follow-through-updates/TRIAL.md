# Feedback follow-through updates: tried on its invented example

- **Product:** Claude, run in Claude Code
- **Model:** Claude Sonnet 5.5 (model ID claude-sonnet-5-5)
- **Date:** 2026-11-10

The inputs are the invented example in [example.md](example.md): the change record, the feedback export, the contact preferences export and the run settings. The company, the customers and the requests are all made up. No client data was used.

This is the second run. The first run was made on the earlier text and led to the revisions listed below. This one was made by the model named above, which made those revisions. It took only the inputs from the example, produced the full output by following the instruction block and the output format, and only then compared it with the example's output. It was one run in one product. It is not a test for a client, and it does not show how the template behaves in other products.

## Inputs used

- The change record for "Schedule export to spreadsheet" (FR-112), as given in the example, including the workaround's "Answers: What it does not do 1".
- The feedback export of nine rows, as given.
- The contact preferences export of six rows, as given.
- Run settings: Jo Harlan, account manager, today 4 November 2026 (the date in the example's settings, not the date of the trial), responsible team the product manager for scheduling. No style notes.

## What came out

The run produced every part of the output format. The full text follows.

```
FEEDBACK FOLLOW-THROUGH UPDATES: Schedule export to spreadsheet (FR-112)

For: Jo Harlan, account manager. Prepared 4 November 2026 from: change record confirmed by Product manager, scheduling on 3 November 2026; feedback export (9 rows; 8 linked to FR-112; 7 of those on Jo Harlan's accounts); contact preferences (6 rows).

STATUS TO VERIFY WITH Product manager, scheduling
Decision: shipped. Available from: 2 November 2026. Available to: all plans.
What it does: 1. Exports the visits for any chosen date range, from Reports > Visits > Export. 2. Produces a CSV file that opens in common spreadsheet programs. 3. Gives each visit's date, start time, customer name, address, assigned crew, visit type and status.
What it does not do: 1. Send the export automatically on a schedule (under review). 2. Include custom fields, such as a customer's own reference field (planned, no date).
Reason we can share: none supplied. Workaround we can share: anyone with access to Reports can run the export by hand for the week they need (answers What it does not do 1). Guide: help article "Exporting visits to a spreadsheet".
Questions before anything is sent: none.

REQUESTERS: 6 requesters at 6 accounts, from 7 linked requests (1 merged as a repeat request)
1. Marta Quill, Operations manager, Customer B. Requests R-201, R-220, received 2026-06-09, 2026-09-21, via email. Asked for: the week's visits in a spreadsheet for payroll; later asked for news. Status: Delivered. Basis: What it does 1, 2, 3. Update by: email. Draft: D1.
2. Theo Brandt, Owner, Customer C. Request R-214, received 2026-07-15, via in-app message. Asked for: the schedule export sent by itself every Monday at 7am to his office manager. Status: Partly delivered; the export is live, and open part: sending it automatically on a schedule, under review, no date set. Basis: What it does 1, 2; What it does not do 1. Update by: phone call, mornings before 10am. Draft: D2.
3. Lena Osei, Office administrator, Customer D. Request R-219, received 2026-08-04, via email. Asked for: the export to include their customer reference field, used to match visits to invoices. Status: Partly delivered; the export is live, and open part: custom fields, planned, no date set. Basis: What it does 1, 2; What it does not do 2. Update by: account meeting, 18 November 2026. Draft: D3.
4. Accounts team, role not stated, Customer E. Request R-223, received 2026-09-30, via in-app message. Asked for: visits as a CSV for month-end. Status: Delivered. Basis: What it does 1, 2. Update by: none while held. Draft: held: Requester to confirm.
5. Owen Paddick, Director, Customer F. Request R-226, received 2026-10-12, via email. Asked for: the export; says they will look at other tools if it is not sorted before the December renewal. Status: Delivered. Basis: What it does 1, 2. Update by: none while held. Draft: held: Account owner first.
6. Ruth Kanne, Finance lead, Customer G. Request R-229, received 2026-10-20, via phone call. Asked for: a spreadsheet export of the month's visits. Status: Delivered. Basis: What it does 1, 2. Update by: none while held. Draft: held: Not to be contacted.

DRAFT UPDATES (for Jo Harlan to edit and approve)
D1. To: Marta Quill, Customer B. Channel: email.
Subject: The spreadsheet export you asked for is live
Body:
Hi Marta,

You asked in June, and again in September, for a way to get the week's visits into a spreadsheet for payroll. The export went live on 2 November 2026, on all plans.

Go to Reports > Visits > Export and choose a date range. You get a CSV file that opens in common spreadsheet programs, with each visit's date, start time, customer name, address, assigned crew, visit type and status.

The help article "Exporting visits to a spreadsheet" walks through it. If anything is missing for payroll, reply and tell me.

Jo Harlan
Promise check: dates: June (R-201, received 2026-06-09); September (R-220, received 2026-09-21); 2 November 2026 (Available from). Features: export of any date range from Reports > Visits > Export (What it does 1); CSV file for spreadsheet programs (What it does 2); the visit fields listed (What it does 3); all plans (Available to).

D2. To: Theo Brandt, Customer C. Channel: phone call.
Call: mornings before 10am. Talking points:
1. In July you asked for the schedule export to go out by itself every Monday at 7am to your office manager.
2. The export went live on 2 November 2026, on all plans: Reports > Visits > Export, any date range, as a CSV file.
3. Sending it automatically on a schedule is not part of this change. It is under review, no date set.
4. Anyone with access to Reports can run the export by hand for the week they need.
5. The help article "Exporting visits to a spreadsheet" shows how.
6. Would running it by hand each Monday cover what your office manager needs?
Not to say: any date or timing for automatic sending, including any commitment to Monday at 7am (that is his request, not our promise); any timing word such as "for now" or "soon".
Promise check: dates: July (R-214, received 2026-07-15); 2 November 2026 (Available from); "every Monday at 7am" and "each Monday" repeat the customer's own request and commit to nothing. Features: export of any date range (What it does 1); CSV file (What it does 2); all plans (Available to); running it by hand (Workaround we can share, which answers What it does not do 1). Open part: automatic scheduled sending, under review, no date set (What it does not do 1).

D3. To: Lena Osei, Customer D. Channel: account meeting.
Meeting: 18 November 2026 (next quarterly review, from contact notes). Agenda line: The visit export, and your customer reference field.
Talking points:
1. In August you asked for the export to include your customer reference field, which you use to match visits to invoices.
2. The export went live on 2 November 2026, on all plans: Reports > Visits > Export, any date range, as a CSV file that opens in common spreadsheet programs.
3. Custom fields, including your customer reference field, are not in the export. They are planned, no date set.
4. The help article "Exporting visits to a spreadsheet" shows how to run it.
5. How do you match visits to invoices today, without the reference field in the export?
Not to say: any date or quarter for custom fields, including the internal target listed under Do not mention; anything suggesting the reference field comes with the export; any timing word such as "yet" or "soon".
Promise check: dates: August (R-219, received 2026-08-04); 2 November 2026 (Available from). Features: export of any date range (What it does 1); CSV file (What it does 2); all plans (Available to). Open part: custom fields, planned, no date set (What it does not do 2).

HELD, NO DRAFT
Account owner first: R-226, Owen Paddick, Customer F: the request says they will look at other tools if the export is not sorted before the renewal in December. Status: Delivered.
Not to be contacted: R-229, Ruth Kanne, Customer G: do_not_contact is yes; the notes say she asked on 22 October 2026 not to receive product update messages. Status: Delivered.
Requester to confirm: R-223, Accounts team, Customer E: a team, not a named person, and not in the contact preferences. Status: Delivered.
Status unclear: none.

POSSIBLE MATCHES NOT INCLUDED
R-208, Customer D, Lena Osei, 2026-07-02: asks whether the schedule can be downloaded, as a printed copy for crew leads; search word found: download. Jo Harlan decides whether to link it.

OTHER OWNERS' ACCOUNTS
Kit Morrow: 1 requester (R-231).

AFTER SENDING (for a person to do in the feedback tool)
D1: mark R-201, R-220 as updated once sent.
D2: mark R-214 as updated once sent.
D3: mark R-219 as updated once sent.

Drafts for Jo Harlan's approval. Nothing has been sent and no record has been changed.
```

## What was observed

The output has every part the format asks for, in the order given. Nothing in the inputs triggered a stop, and the run made no attempt to send, mark or promise anything. No draft contains a date or feature that the promise check cannot trace to the change record or to the person's own request, and none of the three requesters who should be held received a draft. No draft contains "for now", "yet", "soon" or another timing word; the email is about 95 words with greeting and sign-off.

Compared with the published example, after the example was edited to the revised instructions: the statuses, bases, held lists, possible match and counts agree. The wording of the drafts differs in small places (the run's email subject and some sentences; the example's call and meeting "Not to say" lines are shorter). This run was made by the model that revised the template and edited the example, so it was not a blind comparison.

## What changed after the first run

The first run, made on the earlier text, found these problems, and the instructions and example were revised for them:

- The example's drafts used "for now" and "yet" against the ban on timing words, and the template did not say whether the record's own "For now" wording could be quoted. It now says a workaround or reason is quoted without timing words.
- The Inputs section named the wrong required headers. It now says every header except `plan` is required, and `account_owner` is named.
- Theo Brandt got "Not in this change" in the first run and "Partly delivered" in the example. The status definitions now say that a delivered thing in a different form from the one asked for is Partly delivered.
- The example added "anyone on your team", which the record does not say. Removed.
- The header count "[n] on [account owner]'s accounts" is now defined as linked requests only (7), and the first run's note that it used 8 was wrong; the example and the first run's own header both said 7.
- Basis lines now include every "What it does" point the draft names.
- The record now says which open point a workaround answers, so the assistant no longer has to guess; the first run had to guess.
- The email limit now counts greeting and sign-off. Possible matches do not affect the order of requesters.

## Where the template is still ambiguous or needed a guess

1. **Restating the internal target.** The "Not to say" line names the "Do not mention" item without repeating its content. The template does not say whether to repeat the figure; the run and the example both leave it out.
2. **Today's date.** The settings carry their own date. The run used it, as the example does, rather than the date of the trial.
3. **Closing questions that repeat a day.** The call's closing question says "each Monday", which repeats the customer's own request. The run treated it as allowed by the rule on days the person asked for; a stricter reader might not.
4. **"Any other timing word".** The ban lists words and then says "any other"; where a word is borderline the run chose to leave it out.

Other limits of this record: one run after revision, one product, one invented case; the template's own acceptance tests were not run; the template was not run again after any later edits; and a reader should not take this as evidence about any real customer feedback.
