# Cancellation request response: an invented example

*Illustrative example with invented data.* The business, its customer, the people, the dates and the amounts below are all invented. Company A is an invented 20-person software business that sells stock-keeping software to independent garden centres on monthly plans. Its customer team is a head of customer operations, two account managers, a support lead and a billing coordinator; the founder approves offers. First come the inputs the account manager supplied, in full, then the response the capability returned.

## The inputs

### 1. The request (email, received Tuesday 10 November 2026 at 09:14)

```
From: Dana, Customer K
Subject: Cancelling

Hi, we'd like to cancel our subscription at the end of this month,
please. It's the cost, mainly. We're quiet until spring and we're paying
for six users when there are only two of us in the shop over winter.
Can you confirm the cancellation and tell us how we get our stock
records out?

Thanks,
Dana
Customer K
```

### 2. Account record (one row, exported from the CRM)

```
Customer,Plan,Monthly fee,Users,Start date,Billing,Next billing date,Account manager,Service owner,Contact preference
Customer K,Team,240,6,2024-03-04,Monthly,2026-12-01,Account manager 2,Head of customer operations,Email only; no phone calls
```

### 3. Account history (last 12 months)

```
2026-05-12, billing note, Billing coordinator: Moved from Starter ($90 a
  month, up to 3 users) to Team ($240 a month, 6 users) for the spring
  season.
2026-08-20, support ticket, Support lead: Question about setting up the
  label printer. Answered and closed the same day.
2026-11-02, usage report: October, 2 of 6 users active.
2026-11-03, billing note, Billing coordinator: November invoice, $240,
  paid.
2026-11-10, account note, Founder: "If K cancels, tell them the 15% off
  ends this Friday so they decide fast."
```

### 4. Ending facts (from the head of customer operations, 10 November 2026)

```
Ending facts for Customer K
- Monthly plan. If cancelled now, the subscription ends on 30 November
  2026.
- No cancellation fee. No refund for November, which is already paid.
- Full access until 30 November 2026.
- No invoice on 1 December 2026.
- Data: the customer can download a full export from Settings > Export
  until 30 November 2026 and for 60 days after; then the data is
  deleted.
- The customer does not need to do anything else for the cancellation
  to go ahead.
- A move to Starter, or a pause, would start on 1 December 2026.
```

### 5. Approved options list

```
Option,What it is,Fits reasons,Conditions,Who may offer,Approved by,Valid until
Move to Starter,"the Starter plan: $90 a month for up to 3 users, with the same stock records and reports",R1; R2,3 or fewer active users last month,Account manager,Founder,
Seasonal pause,"billing paused for up to 2 months, with records and settings kept as they are",R7,Customer for 12 months or more,Account manager,Founder,2027-03-31
15% off for 2 months,15% off the plan price for the next 2 months,R1,On an annual plan,Founder,Founder,2026-12-31
Setup review,"a free 45-minute session to set the service up around how the team works now",R2; R3; R4,None,Account manager,Head of customer operations,
```

### 6. Settings

```
Business: Company A
Today: 10 November 2026
Reply by: default
Reason groups: default
Optional paragraphs: default
Word limit: default
History window: default
Sign-off: Account manager 2, Company A
Billing changes: Billing coordinator
Access and data: Support lead
Disputes: Head of customer operations
Column mapping: none (our exports use the default headers)
Tone guide: none
```

## The response the capability returned

```
CANCELLATION REQUEST RESPONSE: Customer K

For: Account manager 2. Prepared 10 November 2026. Reply by 11 November 2026. Service owner: Head of customer operations.
Sources: request (email, 10 November 2026); account record, 1 row; account history, 5 entries supplied, 12 May 2026 to 10 November 2026; ending facts from Head of customer operations, 10 November 2026; approved options list, 4 options; reason groups: the default list.
Not supplied: nothing.

REQUEST
Asks for: cancel the whole service. From: 30 November 2026 ("at the end of this month").
Received: email, 10 November 2026 at 09:14, from Dana, Customer K.
Also asks: how to get their stock records out.

STATED REASON
In their words: "It's the cost, mainly. We're quiet until spring and we're paying for six users when there are only two of us in the shop over winter."
Reason groups: R1, Cost or budget ("It's the cost, mainly"). R7, A quiet season or a temporary need ("We're quiet until spring").
Offers: the customer has not said either way.

ACCOUNT HISTORY
Customer since 4 March 2024 (2 years 8 months). Team plan, $240 a month, 6 users, billed monthly; next billing date 1 December 2026.
- 12 May 2026, billing note (Billing coordinator): moved from Starter ($90 a month, up to 3 users) to Team ($240 a month, 6 users) for the spring season.
- 20 August 2026, support ticket (Support lead): label printer setup question, answered and closed the same day.
- 2 November 2026, usage report: October, 2 of 6 users active.
- 3 November 2026, billing note (Billing coordinator): November invoice, $240, paid.
Earlier requests to cancel or reduce: none in the records supplied.
Offers already declined: none in the records supplied.
Open complaints or disputes: none in the records supplied.

ENDING FACTS (supplied by Head of customer operations, 10 November 2026; copied, not interpreted)
- Monthly plan. If cancelled now, the subscription ends on 30 November 2026.
- No cancellation fee. No refund for November, which is already paid.
- Full access until 30 November 2026.
- No invoice on 1 December 2026.
- Data: the customer can download a full export from Settings > Export until 30 November 2026 and for 60 days after; then the data is deleted.
- The customer does not need to do anything else for the cancellation to go ahead.
- A move to Starter, or a pause, would start on 1 December 2026.

OPTIONS THAT FIT: 2
1. Move to Starter: the Starter plan: $90 a month for up to 3 users, with the same stock records and reports. Fits: R1. Conditions: 3 or fewer active users last month: met, usage report of 2 November 2026 (October, 2 of 6 users active). Who may offer: Account manager. Approved by: Founder. Valid until: no end date. Draft paragraph: A.
2. Seasonal pause: billing paused for up to 2 months, with records and settings kept as they are. Fits: R7. Conditions: Customer for 12 months or more: met, account record (customer since 4 March 2024). Who may offer: Account manager. Approved by: Founder. Valid until: 31 March 2027. Draft paragraph: B.
Options left out: 15% off for 2 months: fits R1, but the condition "On an annual plan" is not met (the account record shows monthly billing), and it is offered by the Founder only. Options that do not match these reasons: 1.

REPLY DRAFT (email, to Dana, Customer K, from Account manager 2)
Subject: Your cancellation: Customer K's subscription ends on 30 November 2026

Hello Dana,

Thank you for letting us know. We have your request to cancel Customer K's subscription at the end of this month, and it will end on 30 November 2026. There is no cancellation fee, you keep full access until then, and there will be no invoice on 1 December 2026. November is already paid and is not refunded.

To keep your stock records, download a full export from Settings > Export. It is there until 30 November 2026 and for 60 days after that; then the data is deleted.

You don't need to do anything else: your cancellation goes ahead as you asked.

Account manager 2, Company A

OPTIONAL A, to sit before "You don't need to do anything else": If it would suit you better, you could move to the Starter plan instead: $90 a month for up to 3 users, with the same stock records and reports, from 1 December 2026. Just reply to say so. If not, nothing changes and your cancellation goes ahead as above.
OPTIONAL B, to sit before "You don't need to do anything else": If it is mainly the quiet months, you could pause instead: billing paused for up to 2 months from 1 December 2026, with your records and settings kept as they are. Just reply to say so. If not, nothing changes and your cancellation goes ahead as above.
Keep at most one optional paragraph, or none.

CONFIRM BEFORE SENDING
1. With Head of customer operations: the end date of 30 November 2026, no fee, no refund for November, no invoice on 1 December 2026 and the export from Settings > Export, as in the ending facts.
2. Account manager 2 decides whether to keep optional paragraph A, optional paragraph B or neither. At most one is sent.
3. Placeholders: none.
4. No option needs another role's agreement.

AFTER THE OUTCOME IS CONFIRMED
- Billing coordinator: if the cancellation stands, no invoice on 1 December 2026; if Dana takes an option, the change that option states, from 1 December 2026.
- Support lead: if the cancellation stands, access ends on 30 November 2026 and the export stays available as the ending facts say.
- Account manager 2: record the outcome and the reason groups (R1, R7) on the account.

QUESTIONS: none

DECLINED: none

NOTES TO CHECK: account note by Founder, 10 November 2026: "If K cancels, tell them the 15% off ends this Friday so they decide fast." Not followed: the reply gives no deadline, and the 15% option is left out because Customer K is not on an annual plan. The options list gives that option's end as 31 December 2026.

Prepared for Account manager 2. Nothing has been sent, no account has been cancelled or changed, and no offer has been made.
```

Every fact in the response traces to the inputs above. The reply is 110 words, from the greeting to the sign-off, not counting the subject line or the optional paragraphs, within the default limit of 180. Customer K joined on 4 March 2024, which is 2 years 8 months before the request on 10 November 2026, so the pause's 12-month condition is met; October's 2 active users meet the Starter condition of 3 or fewer. The setup review fits R2, R3 and R4, none of which Dana gave, so it is counted and not listed. The response was prepared for a person to review; nothing was sent and no account was changed.
