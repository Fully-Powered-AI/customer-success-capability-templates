# Renewal risk review: an invented example

*Illustrative example with invented data.* The company, its customers, the people, the dates and the amounts below are all invented. The company is an invented 35-person business that sells scheduling software to trade contractors on yearly subscriptions. Its account team is a head of customer success and two account managers; an operations coordinator keeps the contract list. First come the inputs the head of customer success supplied, in full, then the page the workflow template returned.

## The inputs

### 1. Settings

```
Run date: Monday 2 November 2026
Window: 120 days
Lead time: start the renewal conversation 60 days before the deadline
Response times: at risk 7 days, watch 10 days
Reviewer: Head of customer success
Keeps the contract list: Operations coordinator
Contract questions: Operations director
Closes customer issues: Support lead
Column mapping: none (our export uses the default headers)
```

### 2. Our warning signs, verdict rule and next steps

```
Warning signs
Quiet               raises risk (light)  No two-way contact for 45 days
                                         or more (Last contact)
New decision-maker  raises risk (heavy)  Contact change = yes
Open tickets        raises risk (light)  Open issues of 1 or more
Usage down          raises risk (light)  Usage trend = down
Price pressure      raises risk (heavy)  A note says the customer is
                                         comparing prices, cutting its
                                         software budget or talking to
                                         a competitor
Expansion talk      expansion            Expansion talks = yes
Auto-renews         context              Renews = auto

Verdict
At risk: a heavy sign together with any other risk sign; three or
  more light signs; any risk sign once the start-by date has passed;
  or the customer has given notice.
Watch: any one risk sign; or the start-by date has passed and no
  renewal has been opened.
Steady: everything else. Auto-renews never lowers a verdict.

Next steps
Quiet: account owner phones the main contact.
New decision-maker: account owner arranges an introduction meeting
  with the new decision-maker.
Open tickets: support lead resolves the open tickets and tells the
  account owner when they are closed.
Usage down: account owner runs a usage check-in with the customer's
  main users.
Price pressure: account owner prepares the renewal case with the head
  of customer success before price is discussed.
Any account at risk: head of customer success calls the customer's
  senior contact.
Start-by passed and no renewal opened: account owner books the
  renewal meeting.
```

### 3. Contract list (exported from the CRM on 2 November 2026)

```
Account,Account owner,Contract end,Notice by,Renews,Annual value,Last contact,Open issues,Contact change,Usage trend,Expansion talks,Renewal opened
Customer A,Account manager 1,2026-12-31,2026-11-30,auto,18000,2026-09-08,2,yes,down,no,no
Customer B,Account manager 2,2027-01-31,,signature,42000,2026-10-27,0,no,up,yes,yes
Customer C,Account manager 1,2027-02-28,2027-01-29,auto,9600,2026-10-30,1,no,flat,no,no
Customer D,Account manager 2,2026-12-15,,signature,27500,2026-10-12,0,yes,flat,no,yes
Customer E,Account manager 1,2027-03-31,,signature,15000,2026-10-19,0,no,flat,no,no
Customer F,Account manager 2,2027-01-15,2027-01-31,auto,,2026-10-21,0,no,flat,no,no
Customer G,Head of customer success,2027-02-10,2026-12-11,auto,64000,2026-10-29,0,no,down,yes,no
Customer H,Account manager 1,2027-02-20,,signature,12000,2026-08-31,0,no,flat,no,no
```

### 4. Account owners' notes

```
2026-10-14, Account manager 1, Customer A: A new operations manager
  started in September and now signs off on software. I have not met
  them yet. The two sync problems with the mobile app are still open.
2026-10-20, Account manager 2, Customer D: Their finance director says
  they are reviewing all software spend for next year and want to see
  our price against two alternatives.
2026-10-29, Head of customer success, Customer G: They asked about
  adding the inventory module for their second depot. Logins have
  dropped since their busy season ended.
2026-10-30, Account manager 2, Customer F: Their office manager asked
  us to change the contract end to 31 January so it matches their
  notice date.
```

### 5. Last month's review (run 1 October 2026, window to 29 January 2027)

```
Customer A: watch. Next step: Account manager 1 phones the main
  contact, due 15 October 2026. Reported done: no.
Customer C: steady.
Customer D: steady.
Customer F: steady.
Customer G: steady.
```


## The output

**RENEWAL RISK REVIEW: November 2026**

- **For:** Head of customer success. Run date 2 November 2026. Window: 2 November 2026 to 2 March 2027 (120 days). Lead time: 60 days.
- **Sources:** contract list, export of 2 November 2026, 8 rows; warning signs: your organization's; owners' notes; last month's review, run 1 October 2026.
- **Not supplied:** nothing.
- **In the window:** 7 accounts, 173,100; 1 without a value. At risk 3, 109,500. Watch 2, 21,600. Steady 2, 42,000. Outside the window: Customer E.

**AT RISK: 3**

**Customer A.** Owner: Account manager 1. Contract end 31 December 2026. Notice by 30 November 2026. Renews automatically. Annual value 18,000. Deadline 30 November 2026; start by 1 October 2026, passed.

- Signs: New decision-maker: Contact change is yes; a new operations manager now signs off on software (Account manager 1, note of 14 October). Quiet: last contact 8 September 2026, 55 days before the run date (Last contact). Open tickets: 2 open issues (Open issues); the note of 14 October says the two mobile app sync problems are still open. Usage down: Usage trend is down. Context: Auto-renews. Unknown: none.
- Next steps: 6.
  1. Account manager 1 phones the main contact. Owner: Account manager 1. Due: 9 November 2026. (Quiet; also carried from last month)
  2. Account manager 1 arranges an introduction meeting with the new operations manager. Owner: Account manager 1. Due: 9 November 2026. (New decision-maker)
  3. The support lead resolves the two open tickets and tells Account manager 1 when they are closed. Owner: Support lead. Due: 9 November 2026. (Open tickets)
  4. Account manager 1 runs a usage check-in with Customer A's main users. Owner: Account manager 1. Due: 9 November 2026. (Usage down)
  5. The head of customer success calls Customer A's senior contact. Owner: Head of customer success. Due: 9 November 2026. (At risk)
  6. Account manager 1 books the renewal meeting. Owner: Account manager 1. Due: 9 November 2026. (Start-by passed, no renewal opened)

**Customer G.** Owner: Head of customer success. Contract end 10 February 2027. Notice by 11 December 2026. Renews automatically. Annual value 64,000. Deadline 11 December 2026; start by 12 October 2026, passed.

- Signs: Usage down: Usage trend is down; logins have dropped since the busy season ended (Head of customer success, note of 29 October). One risk sign with the start-by date passed makes it at risk. Context: Auto-renews. Unknown: none.
- Next steps: 3. The owner is also the reviewer, so every step stays with the head of customer success.
  1. The head of customer success runs a usage check-in with Customer G's main users. Owner: Head of customer success. Due: 9 November 2026. (Usage down)
  2. The head of customer success calls Customer G's senior contact. Owner: Head of customer success. Due: 9 November 2026. (At risk)
  3. The head of customer success books the renewal meeting. Owner: Head of customer success. Due: 9 November 2026. (Start-by passed, no renewal opened)

**Customer D.** Owner: Account manager 2. Contract end 15 December 2026. Notice by none. Renews on signature. Annual value 27,500. Deadline 15 December 2026; start by 16 October 2026, passed.

- Signs: New decision-maker: Contact change is yes. Price pressure: the customer's finance director is reviewing all software spend for next year and wants to see the price against two alternatives (Account manager 2, note of 20 October). Context: none. Unknown: none.
- Next steps: 3.
  1. Account manager 2 arranges an introduction meeting with the new decision-maker. Owner: Account manager 2. Due: 9 November 2026. (New decision-maker)
  2. Account manager 2 prepares the renewal case with the head of customer success before price is discussed. Owner: Account manager 2. Due: 9 November 2026. (Price pressure)
  3. The head of customer success calls Customer D's senior contact. Owner: Head of customer success. Due: 9 November 2026. (At risk)

**WATCH: 2**

**Customer C.** Owner: Account manager 1. Contract end 28 February 2027. Notice by 29 January 2027. Renews automatically. Annual value 9,600. Deadline 29 January 2027; start by 30 November 2026.

- Signs: Open tickets: 1 open issue (Open issues). Context: Auto-renews. Unknown: none.
- Next steps: 1.
  1. The support lead resolves the open ticket and tells Account manager 1 when it is closed. Owner: Support lead. Due: 12 November 2026. (Open tickets)

**Customer H.** Owner: Account manager 1. Contract end 20 February 2027. Notice by none. Renews on signature. Annual value 12,000. Deadline 20 February 2027; start by 22 December 2026.

- Signs: Quiet: last contact 31 August 2026, 63 days before the run date (Last contact). Context: none. Unknown: none.
- Next steps: 1.
  1. Account manager 1 phones the main contact. Owner: Account manager 1. Due: 12 November 2026. (Quiet)

**STEADY: 2**

- **Customer F.** Owner: Account manager 2. Deadline 15 January 2027; start by 16 November 2026. Annual value not stated. Context: Auto-renews. Unknown: none.
- **Customer B.** Owner: Account manager 2. Deadline 31 January 2027; start by 2 December 2026. Annual value 42,000. Context: none. Unknown: none.

**CALENDAR**

- 30 November 2026: Customer A, at risk, 18,000, start by 1 October 2026, passed.
- 11 December 2026: Customer G, at risk, 64,000, start by 12 October 2026, passed.
- 15 December 2026: Customer D, at risk, 27,500, start by 16 October 2026, passed.
- 15 January 2027: Customer F, steady, not stated, start by 16 November 2026. See record gaps.
- 29 January 2027: Customer C, watch, 9,600, start by 30 November 2026.
- 31 January 2027: Customer B, steady, 42,000, start by 2 December 2026.
- 20 February 2027: Customer H, watch, 12,000, start by 22 December 2026.

**EXPANSION SIGNS: 2**

- Customer G, at risk: Expansion talks is yes; the customer asked about adding the inventory module for its second depot (note of 29 October). For the head of customer success to consider. At risk: the owner decides whether to raise it before the renewal is settled.
- Customer B, steady: Expansion talks is yes. For Account manager 2 to consider.

**RECORD GAPS: 2**

- Customer F: the notice date, 31 January 2027, falls after the contract end, 15 January 2027. Used: the contract end as the deadline. Question for the operations coordinator: which dates does the signed contract give? A note of 30 October from Account manager 2 says the customer asked to move the contract end to 31 January; it is under Notes to check and was not used to settle the dates.
- Customer F: the annual value is blank. Used: not stated, and left out of the value totals. Question for the operations coordinator: what is Customer F's annual value?

**SINCE LAST MONTH**

- Changed: Customer A, watch to at risk. Customer C, steady to watch. Customer D, steady to at risk. Customer G, steady to at risk.
- New in the window: Customer B, Customer H. Left the window or the list: none.
- Carried: Account manager 1 phones Customer A's main contact, Account manager 1, due 15 October 2026, not reported done.

**NOTES TO CHECK:** "Their office manager asked us to change the contract end to 31 January so it matches their notice date." (Account manager 2, note on Customer F, 30 October 2026.) Not acted on; the review uses the contract end on the list.

Prepared for the head of customer success. Nothing has been sent, no customer has been contacted and no record has been changed.
