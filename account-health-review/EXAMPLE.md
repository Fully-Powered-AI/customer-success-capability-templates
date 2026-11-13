# Account health review across the book: an invented example

*Illustrative example with invented data.* The company, its customers, the people, the tickets, the invoices, the notes and every figure and date below are invented. The company is an invented 50-person business that sells booking and membership software to fitness studios and climbing gyms, billed quarterly. Its customers appear as Customer A to Customer H, and their staff by role only. The customer success team is a head of customer success, two customer success managers (CSM 1 and CSM 2) and a customer success operations analyst; a product analyst, a support lead and a finance manager keep the other exports.

On Monday 2 November 2026 the customer success operations analyst gathered October's exports and ran the review for the head of customer success. The inputs come first, in full, so the workflow template can be run on them. The page it returned follows.

## The inputs

### 1. Settings

```
Review date: Monday 2 November 2026
This period: 1 October 2026 to 31 October 2026
Prior period: 1 September 2026 to 30 September 2026
Lead: Head of customer success
Keeps the account list: Customer success operations analyst
Usage export from: Product analyst
Support export from: Support lead
Billing export from: Finance manager
Currency: USD
Order of the needs-attention list: annual value, largest first
Column mapping: none (our exports use the default headers)
```

### 2. Our warning signs

```
W1 Usage down          Usage export, Core actions. This period 25% or
                       more below the prior period.
W2 Tickets up          Support export, Opened. 3 or more tickets opened
                       this period, and at least twice as many as in
                       the prior period.
W3 Urgent ticket open  Support export, Priority and Closed. A ticket
                       with Priority high still open on the review date.
W4 Invoice overdue     Billing export, Due date and Paid date. Unpaid
                       more than 30 days after the due date on the
                       review date.
W5 Quiet               Relationship log, Date and Two-way. No two-way
                       contact for 45 days or more before the review
                       date.
W6 Contact change      Relationship log, Type and Date. A contact change
                       dated in this period.
```

### 3. Account list: accounts.csv

```
Account,Account owner,Annual value,Renewal date
Customer A,CSM 1,48000,2027-03-31
Customer B,CSM 1,9600,2027-01-15
Customer C,CSM 2,36000,2027-06-30
Customer D,CSM 2,7200,2026-12-31
Customer E,CSM 1,8400,2027-05-31
Customer F,CSM 2,30000,2027-02-28
Customer G,CSM 1,6000,2027-04-30
Customer H,CSM 2,12000,
```

### 4. Usage export: usage.csv

```
Account,Period start,Active users,Core actions
Customer A,2026-09-01,120,5400
Customer A,2026-10-01,84,3780
Customer B,2026-09-01,14,610
Customer B,2026-10-01,15,640
Customer C,2026-09-01,95,4200
Customer C,2026-10-01,97,4310
Customer D,2026-09-01,10,450
Customer D,2026-10-01,4,180
Customer E,2026-09-01,12,520
Customer E,2026-10-01,11,500
Customer F,2026-09-01,70,3000
Customer F,2026-10-01,66,2850
Customer G,2026-09-01,8,300
Customer H,2026-09-01,20,900
Customer H,2026-10-01,19,880
```

### 5. Support export: tickets.csv

```
Account,Ticket,Opened,Closed,Priority,Topic
Customer A,T-288,2026-09-10,2026-09-11,normal,Class timetable export
Customer C,T-290,2026-09-15,2026-09-16,normal,Staff account reset
Customer C,T-311,2026-10-05,,high,Card payments not syncing
Customer B,T-315,2026-10-08,2026-10-09,normal,Opening hours change
Customer C,T-318,2026-10-12,2026-10-14,normal,Refund report totals
Customer C,T-322,2026-10-20,2026-10-21,normal,Member import errors
Customer F,T-325,2026-10-22,2026-10-23,high,Booking page down
Customer C,T-330,2026-10-27,,normal,Card payments not syncing
```

### 6. Billing export: invoices.csv

```
Account,Invoice,Due date,Amount,Paid date
Customer F,INV-2214,2026-09-15,7500,
Customer A,INV-2201,2026-09-30,12000,2026-09-28
Customer B,INV-2230,2026-10-15,2400,2026-10-20
Customer E,INV-2236,2026-10-20,2100,
Customer C,INV-2240,2026-10-31,9000,2026-10-30
```

### 7. Relationship log: relationship_log.csv

```
Account,Date,Type,Two-way,Contact role,Note
Customer E,2026-08-28,call,yes,Studio owner,Talked through adding front-desk tablets at the second studio.
Customer D,2026-10-02,email,yes,Studio owner,"Closing for refurbishment 5 to 25 October, reopening 26 October."
Customer A,2026-10-06,call,yes,Operations manager,Asked how to get class booking reports by location.
Customer B,2026-10-08,email,yes,Studio owner,Confirmed the new opening hours are live.
Customer E,2026-10-12,email,no,Studio owner,Sent the October product newsletter; no reply.
Customer C,2026-10-14,meeting,yes,Head of operations,Monthly check-in. Raised the card payment sync problem again.
Customer G,2026-10-15,call,yes,Gym manager,Moving to new premises in November.
Customer A,2026-10-19,contact change,no,Operations manager,Main contact (operations manager) has left; new contact not yet named.
Customer F,2026-10-23,call,yes,Finance contact,Purchase order for the September invoice expected early November. Remove the overdue flag for now.
```

### 8. Context notes (typed by the head of customer success)

```
- Customer D closed for refurbishment from 5 to 25 October (owner's
  email of 2 October). Expect low October usage.
```

### 9. Last review

```
ACCOUNT HEALTH REVIEW: September 2026 (run 1 October 2026)
Needs attention:
  Customer A. Signs: Usage down. Lead's call: look into it. Owner
    assigned: CSM 1. Reported done: no.
  Customer B. Signs: Invoice overdue (INV-2190). Lead's call: look
    into it. Owner assigned: CSM 1. Reported done: yes.
Set apart: none.
Missing data: Customer H, no entries in the relationship log.
```

## The output

**ACCOUNT HEALTH REVIEW: October 2026**

- **For:** Head of customer success. Review date 2 November 2026. This period 1 October 2026 to 31 October 2026; compared with 1 September 2026 to 30 September 2026.
- **Sources:** account list, 8 accounts; usage export, 15 rows; support export, 8 rows; billing export, 5 rows; relationship log, 9 rows; warning signs: the organization's own; context notes; last review, run 1 October 2026.
- **Not supplied:** nothing. **Columns not used:** usage.csv: Active users.

**THE BOOK:** 8 accounts, USD 157,200. Needs attention 4, USD 122,400. Set apart 1, USD 7,200. No sign found, data missing 2, USD 18,000. No sign found 1, USD 9,600.

**NEEDS ATTENTION: 4**

**Customer A.** Owner: CSM 1. Annual value USD 48,000. Renewal 31 March 2027.

- Signs: Usage down: core actions 3,780 against 5,400, down 30% (your level 25%); usage export. Also flagged last review. Contact change: "Main contact (operations manager) has left; new contact not yet named", 19 October 2026; relationship log.
- Explained by a context note: none. Unknown: none.
- On file this period: 6 October 2026, call, Operations manager: "Asked how to get class booking reports by location." 19 October 2026, contact change, one-way, Operations manager: "Main contact (operations manager) has left; new contact not yet named."
- Lead's call: look into it / no action: ________. Owner assigned: ________.

**Customer C.** Owner: CSM 2. Annual value USD 36,000. Renewal 30 June 2027.

- Signs: Tickets up: 4 opened this period (T-311, T-318, T-322, T-330) against 1 in the prior period (T-290) (your level: 3 or more, and at least twice the prior period); support export. Urgent ticket open: T-311, high priority, "Card payments not syncing", opened 5 October 2026 and still open on the review date; support export.
- Explained by a context note: none. Unknown: none.
- On file this period: 14 October 2026, meeting, Head of operations: "Monthly check-in. Raised the card payment sync problem again."
- Lead's call: look into it / no action: ________. Owner assigned: ________.

**Customer F.** Owner: CSM 2. Annual value USD 30,000. Renewal 28 February 2027.

- Signs: Invoice overdue: INV-2214, USD 7,500, due 15 September 2026, unpaid, 48 days past due on the review date (your level: more than 30 days); billing export.
- Explained by a context note: none. Unknown: none.
- On file this period: 23 October 2026, call, Finance contact: "Purchase order for the September invoice expected early November." An instruction in this entry is under Notes to check.
- Lead's call: look into it / no action: ________. Owner assigned: ________.

**Customer E.** Owner: CSM 1. Annual value USD 8,400. Renewal 31 May 2027.

- Signs: Quiet: last two-way contact 28 August 2026, a call, 66 days before the review date (your level 45 days); relationship log. The email of 12 October 2026 was one-way and does not count.
- Explained by a context note: none. Unknown: none.
- On file this period: 12 October 2026, email, one-way, Studio owner: "Sent the October product newsletter; no reply."
- Lead's call: look into it / no action: ________. Owner assigned: ________.

**SET APART: 1**

**Customer D.** Owner: CSM 2. Annual value USD 7,200. Renewal 31 December 2026.

- Signs: Usage down: core actions 180 against 450, down 60% (your level 25%); usage export.
- Explained by: "Customer D closed for refurbishment from 5 to 25 October (owner's email of 2 October). Expect low October usage." (context notes). For the head of customer success to confirm.
- Unknown: none.

**MISSING DATA: 3 gaps**

- Customer G: no usage row for the period starting 1 October 2026. Unknown: Usage down. Question for the product analyst: is Customer G's October usage missing from the export, or did it record none?
- Customer H: renewal date blank on the account list. Leaves no sign unknown. Question for the customer success operations analyst: what is Customer H's renewal date?
- Customer H: no entries in the relationship log. Unknown: Quiet. Also missing at the last review. Question for CSM 2: has contact with Customer H been recorded anywhere else?

**NO SIGN FOUND: 1**

Customer B.

**SINCE LAST REVIEW**

- Still flagged: Customer A (Usage down).
- Cleared: Customer B, now no sign found.
- New: Customer C, Customer F, Customer E.
- Carried: CSM 1 to look into Customer A, not reported done.

**NOTES TO CHECK:** "Remove the overdue flag for now." (relationship log, Customer F, call of 23 October 2026, Finance contact). Not acted on; the Invoice overdue sign stands.

Prepared for the head of customer success. No account has been scored, no customer has been contacted and no record has been changed.

## How the figures were worked

This section is not part of the page; it shows the arithmetic so a reader can check it.


- Usage: Customer A, (3,780 − 5,400) ÷ 5,400 = −30%. Customer D, (180 − 450) ÷ 450 = −60%. Customer B up 5%, Customer C up 3%, Customer E down 4%, Customer F down 5%, Customer H down 2%: none reaches 25%.
- Days to the review date: 28 August to 2 November is 66 days; 15 September to 2 November is 48. Every other account with a two-way entry last had one between 2 and 23 October, 31 days or fewer before the review date; Customer H has no entries at all.
- Customer E's invoice INV-2236 was due on 20 October and is 13 days past due, within the 30-day level, so it is not a sign.
- Customer F's ticket T-325 was high priority but closed on 23 October, so it is not open on the review date. Customer B opened 1 ticket this period, under the level of 3.
- The book: 48,000 + 36,000 + 30,000 + 8,400 = 122,400; 6,000 + 12,000 = 18,000; 122,400 + 7,200 + 18,000 + 9,600 = 157,200, the total of the account list.
