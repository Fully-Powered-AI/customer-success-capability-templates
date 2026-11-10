# Lapsed-customer win-back: an invented example

*Illustrative example with invented data.* The company, its customers, the people, the orders, the dates and the amounts below are all invented. The company is an invented 20-person business that makes cleaning and hygiene products and sells them on trade accounts to cafés, gyms, salons and small offices. Its account team is the owner and two account managers; an operations coordinator keeps the customer list and runs the exports. First come the inputs the owner supplied, in full, then the list the capability returned.

## The inputs

### 1. Settings

```
Run date: Monday 2 November 2026
Lapse multiple: 2 (default)
Lapse floor: 30 days (default)
Orders needed for a pattern: 3 (default)
Gaps used: the most recent 6 (default)
Value period: the 365 days ending on the last completed order (default)
Long gone: more than 365 days (default)
Rest period: 60 days (default)
Recent issue window: 90 days (default)
Offer in the note: last line
Note length: 120 words (default)
Approver: Owner
Offer approver: Owner
List owner: Operations coordinator
Complaints: Customer service lead
Column mapping: none (our exports use the default headers)
Amounts are in dollars, written without a symbol.
```

### 2. Approved offers (typed by the owner)

```
Offer 1: Free delivery on your next two orders.
  For customers with a value of 3,000 or more.
  Valid until 30 November 2026.
Offer 2: 10% off your next order, up to 150 off.
  For customers with a value of 1,000 to 2,999.
  Valid until 30 November 2026.
Customers with a value under 1,000: no offer.
```

### 3. Voice notes

```
Sign-off: first name only.
Plain, short sentences. No exclamation marks.
We say "order" and "delivery", never "purchase" or "shipment".
```

### 4. Order history (exported on 2 November 2026)

```
Order ID,Customer,Order date,Order value,Status,Items
4101,Customer H,2025-02-03,650,completed,Paper towel rolls x48; Hand soap refills 5L x4
4102,Customer H,2025-04-01,700,completed,Paper towel rolls x48; Hand soap refills 5L x4
4103,Customer H,2025-06-02,620,completed,Paper towel rolls x48; Hand soap refills 5L x4
4104,Customer H,2025-08-01,680,completed,Paper towel rolls x48; Hand soap refills 5L x4
4105,Customer C,2025-10-02,760,completed,Salon towels x100; Disinfectant 5L x4
4106,Customer B,2025-11-10,610,completed,Surface spray 5L x6; Microfibre cloths x200
4107,Customer B,2025-12-22,655,completed,Surface spray 5L x6; Microfibre cloths x200
4108,Customer C,2026-01-05,810,completed,Salon towels x100; Disinfectant 5L x4
4109,Customer F,2026-01-12,880,completed,Surface spray 5L x8; Floor cleaner 5L x4
4110,Customer B,2026-02-05,700,completed,Surface spray 5L x6; Microfibre cloths x200
4111,Customer A,2026-02-13,1150,completed,Hand soap refills 5L x6; Paper towel rolls x48
4112,Customer F,2026-02-23,910,completed,Surface spray 5L x8; Floor cleaner 5L x4
4113,Customer E,2026-03-03,520,completed,Dish detergent 5L x4; Floor cleaner 5L x2
4114,Customer A,2026-03-16,1180,completed,Hand soap refills 5L x6; Paper towel rolls x48
4115,Customer B,2026-03-23,640,completed,Surface spray 5L x6; Microfibre cloths x200
4116,Customer C,2026-04-02,790,completed,Salon towels x100; Disinfectant 5L x4
4117,Customer E,2026-04-02,540,completed,Dish detergent 5L x4; Floor cleaner 5L x2
4118,Customer F,2026-04-06,860,completed,Surface spray 5L x8; Floor cleaner 5L x4
4119,Customer D,2026-04-08,420,completed,Hand soap refills 5L x4; Paper towel rolls x24
4120,Customer A,2026-04-15,1240,completed,Hand soap refills 5L x6; Paper towel rolls x48
4121,Customer B,2026-05-04,590,completed,Surface spray 5L x6; Microfibre cloths x200
4122,Customer E,2026-05-04,505,completed,Dish detergent 5L x4; Floor cleaner 5L x2
4123,Customer D,2026-05-07,455,completed,Hand soap refills 5L x4; Paper towel rolls x24
4124,Customer A,2026-05-18,1095,completed,Hand soap refills 5L x6; Paper towel rolls x48
4125,Customer F,2026-05-18,900,completed,Surface spray 5L x8; Floor cleaner 5L x4
4126,Customer G,2026-05-20,300,completed,Disinfectant 5L x2; Salon towels x50
4127,Customer E,2026-06-03,560,completed,Dish detergent 5L x4; Floor cleaner 5L x2
4128,Customer D,2026-06-09,380,refunded,Hand soap refills 5L x4; Paper towel rolls x24
4129,Customer D,2026-06-12,470,completed,Hand soap refills 5L x4; Paper towel rolls x24
4130,Customer B,2026-06-15,720,completed,Surface spray 5L x6; Microfibre cloths x200
4131,Customer A,2026-06-17,1310,completed,Hand soap refills 5L x6; Paper towel rolls x48
4132,Customer G,2026-06-25,340,completed,Disinfectant 5L x2; Salon towels x50
4133,Customer C,2026-07-01,830,completed,Salon towels x100; Disinfectant 5L x4
4134,Customer I,2026-07-06,115,completed,Dish detergent 5L x2; Sanitiser spray x12
4135,Customer D,2026-07-10,430,completed,Hand soap refills 5L x4; Paper towel rolls x24
4136,Customer A,2026-07-20,1265,completed,Hand soap refills 5L x6; Paper towel rolls x48
4137,Customer I,2026-07-20,130,completed,Dish detergent 5L x2; Sanitiser spray x12
4138,Customer I,2026-08-03,120,completed,Dish detergent 5L x2; Sanitiser spray x12
4139,Customer J,2026-08-04,390,completed,Paper towel rolls x24; Surface spray 5L x2
4140,Customer D,2026-08-10,445,completed,Hand soap refills 5L x4; Paper towel rolls x24
4141,Customer I,2026-08-17,125,completed,Dish detergent 5L x2; Sanitiser spray x12
4142,Customer I,2026-08-31,110,completed,Dish detergent 5L x2; Sanitiser spray x12
4143,Customer J,2026-09-03,410,completed,Paper towel rolls x24; Surface spray 5L x2
4144,Customer I,2026-09-14,135,completed,Dish detergent 5L x2; Sanitiser spray x12
4145,Customer I,2026-09-28,120,completed,Dish detergent 5L x2; Sanitiser spray x12
4146,Customer J,2026-10-05,400,completed,Paper towel rolls x24; Surface spray 5L x2
```

### 5. Customer list

```
Customer,Contact,Account owner,Contact allowed
Customer A,Nadia,Account manager 1,yes
Customer B,Teodor,Account manager 1,yes
Customer C,Ines,Account manager 2,yes
Customer D,Marisol,Account manager 2,yes
Customer E,Bram,Account manager 1,no
Customer F,Odile,Account manager 2,yes
Customer G,Kasper,Account manager 1,yes
Customer H,Lucinda,Account manager 2,yes
Customer I,Wendell,,yes
Customer J,Pilar,Account manager 1,yes
```

### 6. Open issues

```
Customer,Opened,Kind,Summary,Status,Closed
Customer A,2026-07-24,complaint,"Two cases of hand soap refills arrived leaking. Customer asked for a credit.",open,
Customer D,2026-08-12,complaint,"Delivery arrived two days late.",closed,2026-08-19
```

### 7. Win-back log

```
Customer,Sent,Outcome
Customer E,2026-07-15,Replied: asked us to stop sending offers
Customer F,2026-09-21,No reply
```

## The output

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

## How the figures were worked out

- **Usual gaps** are the middle of each customer's recent gaps between completed orders. Customer A: 31, 30, 33, 30 and 33 days, middle value 31. Customer B: 42, 45, 46, 42 and 42, middle value 42. Customer D: 29, 36, 28 and 31 days (the refunded order of 9 June left out), average of the two middle values 29 and 31, so 30. Customer I: six gaps of 14 days. Customer C: 95, 87 and 90, so 90.
- **Lapsed:** Customer I's 35 days is more than twice 14 (28) and at least 30. Customer C's 124 days is more than 90 but not more than 180, so C counts as lapsed from day 181, 29 December 2026. Customer J's last order, 5 October 2026, was 28 days ago, inside its usual gap of 31 days.
- **Values** are each customer's completed orders in the 365 days ending on their last order: A 7,240; B 3,915; F 3,550; D 2,220; E 2,125; I 855. Together 19,905.
- **Offers:** Customer B's 3,915 meets Offer 1; Customer D's 2,220 meets Offer 2; Customer I's 855 is under 1,000.
- **Rest period:** Customer F's note of 21 September 2026 was 42 days before the run date; 60 days after it is 20 November 2026.
- **Recent issue:** Customer D's complaint closed on 19 August 2026, 75 days before the run date, inside the 90-day window.
