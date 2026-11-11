# Feedback follow-through updates: an invented example

*Illustrative example with invented data.* Company A, the customers, the people, the requests and the dates below are all invented. Company A is an invented 40-person company that sells visit-scheduling software to cleaning and maintenance businesses. Its product team shipped a spreadsheet export that several customers had asked for. Jo Harlan, an account manager, supplied the inputs below in full on Wednesday 4 November 2026; the follow-through the capability returned comes after them.

## The inputs

### 1. The change record (from the product manager for scheduling)

```
Change: Schedule export to spreadsheet
Item ID: FR-112
Decision: shipped
Available from: 2 November 2026
Date confirmed by: Product manager, scheduling, 3 November 2026
Available to: all plans
What it does:
  1. Exports the visits for any chosen date range, from Reports > Visits > Export.
  2. Produces a CSV file that opens in common spreadsheet programs.
  3. Gives each visit's date, start time, customer name, address, assigned
     crew, visit type and status.
What it does not do:
  1. Send the export automatically on a schedule. Status: under review.
  2. Include custom fields, such as a customer's own reference field.
     Status: planned, no date.
Reason we can share: (blank)
Workaround we can share: For now, anyone with access to Reports can run
  the export by hand for the week they need. Answers: What it does not do 1.
Guide: Help article "Exporting visits to a spreadsheet"
Search words: export, spreadsheet, CSV, download
Do not mention: The internal target of Q1 2027 for custom fields. It is
  not confirmed.
Status confirmed by: Product manager, scheduling, 3 November 2026
```

### 2. The feedback export

```
request_id,received_date,account,requester_name,requester_role,channel_received,request_text,linked_item,plan,account_owner
R-201,2026-06-09,Customer B,Marta Quill,Operations manager,email,"We need the week's visits in a spreadsheet for payroll. Copying them over by hand takes most of Friday afternoon.",FR-112,Standard,Jo Harlan
R-208,2026-07-02,Customer D,Lena Osei,Office administrator,in-app message,"Is there a way to download the schedule? Our crew leads want a printed copy.",,Plus,Jo Harlan
R-214,2026-07-15,Customer C,Theo Brandt,Owner,in-app message,"Could the schedule export go out by itself every Monday at 7am to my office manager?",FR-112,Standard,Jo Harlan
R-219,2026-08-04,Customer D,Lena Osei,Office administrator,email,"When you add the export, please include our customer reference field. We match visits to invoices on it.",FR-112,Plus,Jo Harlan
R-220,2026-09-21,Customer B,Marta Quill,Operations manager,email,"Any news on the spreadsheet export?",FR-112,Standard,Jo Harlan
R-223,2026-09-30,Customer E,Accounts team,,in-app message,"Need visits as CSV for month-end.",FR-112,Standard,Jo Harlan
R-226,2026-10-12,Customer F,Owen Paddick,Director,email,"Still no export. If this isn't sorted before our renewal in December we will look at other tools.",FR-112,Plus,Jo Harlan
R-229,2026-10-20,Customer G,Ruth Kanne,Finance lead,phone call,"Asked for a spreadsheet export of the month's visits.",FR-112,Standard,Jo Harlan
R-231,2026-10-27,Customer H,Sam Ivers,Operations lead,email,"Export to spreadsheet please.",FR-112,Standard,Kit Morrow
```

### 3. The contact preferences export

```
account,requester_name,preferred_channel,do_not_contact,notes
Customer B,Marta Quill,email,no,
Customer C,Theo Brandt,phone call,no,Mornings before 10am
Customer D,Lena Osei,account meeting,no,Next quarterly review 18 November 2026
Customer F,Owen Paddick,email,no,Renewal 1 December 2026
Customer G,Ruth Kanne,email,yes,Asked on 22 October 2026 not to receive product update messages
Customer H,Sam Ivers,email,no,
```

### 4. Run settings and style notes

```
Account owner: Jo Harlan, account manager
Today: 4 November 2026
Responsible team: Product manager, scheduling
Style notes: none
```

## The output

**FEEDBACK FOLLOW-THROUGH UPDATES: Schedule export to spreadsheet (FR-112)**

**For:** Jo Harlan, account manager. Prepared 4 November 2026 from: change record confirmed by the product manager, scheduling, on 3 November 2026; feedback export (9 rows; 8 linked to FR-112; 7 of those on Jo Harlan's accounts); contact preferences (6 rows).

**STATUS TO VERIFY WITH THE PRODUCT MANAGER, SCHEDULING**

- **Decision:** shipped. **Available from:** 2 November 2026. **Available to:** all plans.
- **What it does:** 1. Exports the visits for any chosen date range, from Reports > Visits > Export. 2. Produces a CSV file that opens in common spreadsheet programs. 3. Gives each visit's date, start time, customer name, address, assigned crew, visit type and status.
- **What it does not do:** 1. Send the export automatically on a schedule: under review. 2. Include custom fields, such as a customer's own reference field: planned, no date.
- **Reason we can share:** none supplied. **Workaround we can share:** anyone with access to Reports can run the export by hand for the week they need (answers What it does not do 1). **Guide:** help article "Exporting visits to a spreadsheet".
- **Questions before anything is sent:** none.

**REQUESTERS: 6 requesters at 6 accounts, from 7 linked requests (1 merged as a repeat request)**

1. **Marta Quill**, Operations manager, Customer B. Requests R-201 and R-220, received 9 June 2026 and 21 September 2026, via email. Asked for: the week's visits in a spreadsheet for payroll; then asked for news. Status: Delivered. Basis: What it does 1, 2, 3. Update by: email. Draft: D1.
2. **Theo Brandt**, Owner, Customer C. Request R-214, received 15 July 2026, via in-app message. Asked for: the schedule export sent automatically every Monday at 7am to his office manager. Status: Partly delivered: the export is live; sending it automatically on a schedule is under review, no date set. Basis: What it does 1, 2; What it does not do 1. Update by: phone call, mornings before 10am. Draft: D2.
3. **Lena Osei**, Office administrator, Customer D. Request R-219, received 4 August 2026, via email. Asked for: the export, including the account's customer reference field, which it uses to match visits to invoices. Status: Partly delivered: the export is live; custom fields, including the customer reference field, are planned, no date set. Basis: What it does 1, 2; What it does not do 2. Update by: account meeting, 18 November 2026. Draft: D3.
4. **Accounts team**, role not stated, Customer E. Request R-223, received 30 September 2026, via in-app message. Asked for: visits as a CSV file for month-end. Status: Delivered. Basis: What it does 1, 2. Update by: none while held. Draft: held: Requester to confirm.
5. **Owen Paddick**, Director, Customer F. Request R-226, received 12 October 2026, via email. Asked for: the export, before the account's renewal in December. Status: Delivered. Basis: What it does 1, 2. Update by: none while held. Draft: held: Account owner first.
6. **Ruth Kanne**, Finance lead, Customer G. Request R-229, received 20 October 2026, via phone call. Asked for: a spreadsheet export of the month's visits. Status: Delivered. Basis: What it does 1, 2. Update by: none while held. Draft: held: Not to be contacted.

**DRAFT UPDATES (for Jo Harlan to edit and approve)**

**D1.** To: Marta Quill, Customer B. Channel: email.

*Subject:* The spreadsheet export you asked for is live

*Body:*

> Hi Marta,
>
> In June you asked for a way to get the week's visits into a spreadsheet for payroll, and you checked in again in September. That export went live on 2 November 2026, on all plans.
>
> Go to Reports > Visits > Export and choose a date range. You get a CSV file that opens in common spreadsheet programs, with each visit's date, start time, customer name, address, assigned crew, visit type and status.
>
> The help article "Exporting visits to a spreadsheet" walks through it. If it does not fit how you run payroll, reply and tell me what is missing.
>
> Jo Harlan

*Promise check:* dates: June (R-201, received 9 June 2026), September (R-220, received 21 September 2026), 2 November 2026 (Available from). Features: date-range export from Reports > Visits > Export (What it does 1); CSV file for spreadsheet programs (What it does 2); the visit details listed (What it does 3); all plans (Available to).

**D2.** To: Theo Brandt, Customer C. Channel: phone call.

*Call:* mornings before 10am.

*Talking points:*

1. In July you asked whether the schedule export could go out by itself every Monday at 7am to your office manager.
2. The export went live on 2 November 2026, on all plans: Reports > Visits > Export, any date range, as a CSV file.
3. Sending it automatically on a schedule is not part of this change. It is under review, no date set.
4. Anyone with access to Reports can run the export by hand for the week they need.
5. The help article "Exporting visits to a spreadsheet" shows how.
6. Would running it by hand each Monday cover what your office manager needs?

*Not to say:* any date or timing for automatic sending, and any timing word such as "for now" or "soon".

*Promise check:* dates: July (R-214, received 15 July 2026), 2 November 2026 (Available from); "every Monday at 7am" repeats the customer's own request and commits to nothing. Features: date-range export from Reports > Visits > Export (What it does 1); CSV file (What it does 2); all plans (Available to); running it by hand (Workaround we can share).

**D3.** To: Lena Osei, Customer D. Channel: account meeting.

*Meeting:* 18 November 2026.

*Agenda line:* The visit export, and your customer reference field.

*Talking points:*

1. In August you asked for the visit export to include your customer reference field, which you use to match visits to invoices.
2. The export went live on 2 November 2026, on all plans: Reports > Visits > Export, any date range, as a CSV file that opens in common spreadsheet programs.
3. Custom fields, including your customer reference field, are not in the export. They are planned, no date set.
4. The help article "Exporting visits to a spreadsheet" shows how to run it.
5. How do you match visits to invoices without the reference field in the export?

*Not to say:* any date or quarter for custom fields, including the internal target under "Do not mention".

*Promise check:* dates: August (R-219, received 4 August 2026), 2 November 2026 (Available from). Features: date-range export from Reports > Visits > Export (What it does 1); CSV file for spreadsheet programs (What it does 2); all plans (Available to). Open part: custom fields, planned, no date set (What it does not do 2).

**HELD, NO DRAFT**

- **Account owner first:** R-226, Owen Paddick, Customer F. The request says the company will look at other tools if the export is not sorted before its renewal in December; the contact notes give the renewal as 1 December 2026. Status: Delivered.
- **Not to be contacted:** R-229, Ruth Kanne, Customer G. do_not_contact is yes; the notes say she asked on 22 October 2026 not to receive product update messages. Status: Delivered.
- **Requester to confirm:** R-223, Accounts team, Customer E. A team name rather than a person, and not in the contact preferences. Status: Delivered.
- **Status unclear:** none.

**POSSIBLE MATCHES NOT INCLUDED**

- R-208, Customer D, Lena Osei, received 2 July 2026: asks whether the schedule can be downloaded, for a printed copy for crew leads. Search word found: "download". Jo Harlan decides whether to link it to FR-112.

**OTHER OWNERS' ACCOUNTS**

- Kit Morrow: 1 requester (R-231).

**AFTER SENDING (for a person to do in the feedback tool)**

- D1: mark R-201 and R-220 as updated once sent.
- D2: mark R-214 as updated once sent.
- D3: mark R-219 as updated once sent.

Drafts for Jo Harlan's approval. Nothing has been sent and no record has been changed.
