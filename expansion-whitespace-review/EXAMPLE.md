# Expansion whitespace review: an invented example

*Illustrative example with invented data.* The company, its customers, the people, the dates and the amounts below are all invented. The company is an invented 45-person business that sells maintenance software to property managers and facilities teams, priced per user, per site or per account. Its account team is a head of customer success and two account managers; a sales operations lead keeps the sales system. Account manager 1 ran the review for their own book. First come the inputs they supplied, in full, then the page the capability returned.

## The inputs

### 1. Settings

```
Run date: Monday 9 November 2026
Scope: book, the accounts owned by Account manager 1
Dimensions: all four (offers, teams, sites, volume)
Volume threshold: 80 per cent of the licensed limit
Size bands, on the low end: large 10,000 or more, medium 3,000 to
  9,999, small under 3,000
Plays per account: 5
Onboarding hold: 90 days from the earliest start date
Next steps due: 14 days after the run date
Earliest stage in our sales system: Qualify
Reviewer: Head of customer success
Sales system owner: Sales operations lead
Column mapping: none (our exports use the default headers)
```

### 2. Offer catalogue

```
Offer,Kind,Unit,Value low,Value high,Fits
Work orders,product,per user,600,600,Maintenance
Inspections,add-on,per site,1200,1800,every site
Energy reporting,add-on,per account,6000,9000,Finance; Sustainability
Premium support,tier,per account,4000,4000,accounts with 25 or more Work orders users
```

### 3. Holdings export (from the sales system, 9 November 2026)

```
Account,Account owner,Offer,Team or site,Quantity,Licensed limit,Annual value,Start date
Customer A,Account manager 1,Work orders,Maintenance,36,40,24000,2024-03-01
Customer A,Account manager 1,Inspections,Site 1,1,1,1500,2025-01-15
Customer A,Account manager 1,Inspections,Site 2,1,1,,2025-01-15
Customer B,Account manager 1,Work orders,Maintenance,51,60,36000,2023-09-01
Customer B,Account manager 1,Energy reporting,Finance,1,1,7500,2025-09-01
Customer C,Account manager 1,Work orders,Maintenance,12,20,12000,2026-09-21
Customer D,Account manager 2,Work orders,Maintenance,18,25,15000,2025-02-01
```

### 4. Account structure

```
Account,Unit,Kind
Customer A,Maintenance,team
Customer A,Finance,team
Customer A,Site 1,site
Customer A,Site 2,site
Customer A,Site 3,site
Customer A,Site 4,site
Customer B,Maintenance,team
Customer B,Finance,team
Customer B,Sustainability,team
Customer B,Site 1,site
Customer B,Site 2,site
Customer B,Site 3,site
Customer C,Maintenance,team
Customer C,Site 1,site
Customer C,Site 2,site
```

### 5. Contacts

```
Account,Contact role,Team or site,Relationship,Last contact
Customer A,Facilities director,Maintenance,strong,2026-10-28
Customer A,Finance controller,Finance,none,
Customer B,Operations director,Maintenance,strong,2026-11-02
Customer B,Finance manager,Finance,some,2026-08-12
Customer B,Sustainability lead,Sustainability,none,
Customer C,Maintenance lead,Maintenance,some,2026-11-04
Customer D,Maintenance manager,Maintenance,strong,2026-10-01
```

### 6. Account health (from last month's renewal risk review)

```
Account,Health,Reason
Customer A,steady,
Customer B,watch,one open support escalation for a failed data import
Customer C,steady,
```

### 7. Account notes

```
2026-10-15, Account manager 1, Customer B: The operations director said
  support replies take two days and asked whether a faster support
  option exists. One escalation about a failed data import is still
  open.
2026-10-21, Account manager 1, Customer A: The facilities director asked
  what it would cost to add inspections at Sites 3 and 4, which still
  use paper checklists. She says missed checks at Sites 1 and 2 have
  fallen to almost none since inspections went live there.
2026-10-28, Account manager 1, Customer A: The facilities director
  mentioned six maintenance technicians joining in January.
2026-11-02, Account manager 1, Customer B: The operations director
  mentioned an insurance audit next spring that will ask for inspection
  records at all three sites.
2026-11-04, Account manager 1, Customer C: The maintenance lead asked
  whether inspections could be added at both sites once the team is
  settled.
2026-11-05, Account manager 1, Customer B: Their office manager asked
  us to change the billing contact in our system to her.
```

## The output

The page is shown here with light formatting for reading on the web: headings in bold and lines set as lists. Its content and order are those of the output format, which is plain text.

**EXPANSION WHITESPACE REVIEW: book: the accounts owned by Account manager 1, 9 November 2026**

- **For:** Head of customer success. Run date 9 November 2026. Scope: book: the accounts owned by Account manager 1.
- **Sources:** offer catalogue, 4 offers; holdings, export of 9 November 2026, 7 rows; structure, 15 rows; contacts, 7 rows; health, 3 rows; notes, 6.
- **Settings:** volume threshold 80 per cent; size bands on the low end: large 10,000 or more, medium 3,000 to 9,999, small under 3,000; plays per account 5; onboarding hold 90 days; next steps due 14 days after the run date.
- **Not supplied:** nothing.
- **Accounts reviewed:** 3 (Customer A, Customer B, Customer C). Ranked plays 7. Held 1. No evidence yet 2. Outside the scope: Customer D.

**BOOK RANKING**

1. Customer B: Premium support, whole account, score 8.
2. Customer A: Inspections, Sites 3 and 4, score 7.
3. Customer C: no play to raise now; its one play is held until 20 December 2026.

**ACCOUNT: Customer B.** Owner: Account manager 1. Customer since 1 September 2023. Health: watch, one open support escalation for a failed data import.

Holds today: Work orders, Maintenance, 51 of 60, 36,000; Energy reporting, Finance, 1 of 1, 7,500.

*Whitespace map*

- Offers: Premium support for the whole account: strong. Inspections for Sites 1, 2 and 3: moderate.
- Teams: none.
- Sites: none.
- Volume: Work orders: 51 of 60, 85 per cent: strong.

*Plays ranked: 3*

1. **Premium support, whole account.** Type: higher tier. Estimated annual value: 4,000.
   - Evidence: strong: the operations director "said support replies take two days and asked whether a faster support option exists" (Account manager 1, note of 15 October 2026); 51 Work orders users meets the condition of 25 or more (holdings, catalogue). Size: medium. Access: strong: operations director, strong. Score: 3 + 2 + 3 = 8.
   - Approach: the operations director, about support replies taking two days, building on no result on record.
   - Next step: Account manager 1 answers the operations director's question about a faster support option, with any proposal going to the head of customer success first. Owner: Account manager 1. Due: 23 November 2026.
2. **Work orders, Maintenance.** Type: more volume. Estimated annual value: not estimated (no number of extra users recorded).
   - Evidence: strong: 51 of 60 licences in use, 85 per cent, at or above the 80 per cent threshold (holdings). Size: small. Access: strong: operations director, strong (Maintenance). Score: 3 + 1 + 3 = 7.
   - Approach: the operations director, about the team using 51 of its 60 licences, building on no result on record.
   - Next step: Account manager 1 asks the operations director how many more users the maintenance team expects to need. Owner: Account manager 1. Due: 23 November 2026.
3. **Inspections, Sites 1, 2 and 3.** Type: another offer. Estimated annual value: 3,600 to 5,400.
   - Evidence: moderate: the operations director "mentioned an insurance audit next spring that will ask for inspection records at all three sites" (Account manager 1, note of 2 November 2026). Size: medium. Access: strong: operations director, strong, named in the evidence. Score: 2 + 2 + 3 = 7.
   - Approach: the operations director, about the inspection records the spring insurance audit will ask for at all three sites, building on no result on record.
   - Next step: Account manager 1 asks the operations director what the audit will require at each site. Owner: Account manager 1. Due: 23 November 2026.

Health watch: the account's health is watch (one open support escalation for a failed data import); the account owner decides the timing of each play.

More plays beyond the limit: none.

*Held:* none.

*No evidence yet:* none.

**ACCOUNT: Customer A.** Owner: Account manager 1. Customer since 1 March 2024. Health: steady.

Holds today: Work orders, Maintenance, 36 of 40, 24,000; Inspections, Site 1, 1 of 1, 1,500; Inspections, Site 2, 1 of 1, value not stated.

*Whitespace map*

- Offers: Premium support for the whole account: light. Energy reporting for Finance: light.
- Teams: none.
- Sites: Inspections for Sites 3 and 4: strong.
- Volume: Work orders: 36 of 40, 90 per cent: strong.

*Plays ranked: 4*

1. **Inspections, Sites 3 and 4.** Type: another site. Estimated annual value: 2,400 to 3,600.
   - Evidence: strong: the facilities director "asked what it would cost to add inspections at Sites 3 and 4, which still use paper checklists" (Account manager 1, note of 21 October 2026); Sites 3 and 4 are sites, like Sites 1 and 2, which hold Inspections (structure, holdings). Size: small. Access: strong: facilities director, strong, named in the evidence. Score: 3 + 1 + 3 = 7.
   - Approach: the facilities director, about the paper checklists still used at Sites 3 and 4, building on her report that "missed checks at Sites 1 and 2 have fallen to almost none since inspections went live there" (Account manager 1, note of 21 October 2026).
   - Next step: Account manager 1 answers the facilities director's question about adding inspections at Sites 3 and 4, with the cost taken from the company's own price list and any proposal going to the head of customer success first. Owner: Account manager 1. Due: 23 November 2026.
2. **Work orders, Maintenance.** Type: more volume. Estimated annual value: 1,200 (2 users: 36 in use plus 6 technicians joining, against a limit of 40).
   - Evidence: strong: 36 of 40 licences in use, 90 per cent, at or above the 80 per cent threshold (holdings); the facilities director "mentioned six maintenance technicians joining in January" (Account manager 1, note of 28 October 2026). Size: small. Access: strong: facilities director, strong (Maintenance). Score: 3 + 1 + 3 = 7.
   - Approach: the facilities director, about licences for the six maintenance technicians joining in January, building on no result on record.
   - Next step: Account manager 1 asks the facilities director to confirm when the six technicians start and how many licences the team will need. Owner: Account manager 1. Due: 23 November 2026.
3. **Premium support, whole account.** Type: higher tier. Estimated annual value: 4,000.
   - Evidence: light: 36 Work orders users meets the condition of 25 or more (holdings, catalogue); no need recorded. Size: medium. Access: strong: facilities director, strong. Score: 1 + 2 + 3 = 6.
   - Approach: the facilities director, about whether there is a need for Premium support, building on no result on record.
   - Next step: Account manager 1 confirms with the facilities director whether there is a need before anything is proposed. Owner: Account manager 1. Due: 23 November 2026.
4. **Energy reporting, Finance.** Type: another offer. Estimated annual value: 6,000 to 9,000.
   - Evidence: light: the structure lists a Finance team, and the catalogue says the offer fits Finance; no need recorded. Size: medium. Access: partial: finance controller, no relationship; the facilities director, strong, could introduce. Score: 1 + 2 + 2 = 5.
   - Approach: an introduction to the finance controller through the facilities director, about whether there is a need for Energy reporting, building on no result on record.
   - Next step: Account manager 1 asks the facilities director whether she would introduce the finance controller, to confirm whether there is a need before anything is proposed. Owner: Account manager 1. Due: 23 November 2026.

More plays beyond the limit: none.

*Held:* none.

*No evidence yet:* none.

**ACCOUNT: Customer C.** Owner: Account manager 1. Customer since 21 September 2026. Health: steady.

Holds today: Work orders, Maintenance, 12 of 20, 12,000.

*Whitespace map*

- Offers: Inspections for Sites 1 and 2: strong.
- Teams: none.
- Sites: none.
- Volume: Work orders: 12 of 20, 60 per cent: under the threshold.

*Plays ranked:* none.

More plays beyond the limit: none.

*Held: 1*

- Inspections, Sites 1 and 2: customer for 49 days, inside the 90-day onboarding hold. Evidence: strong: the maintenance lead "asked whether inspections could be added at both sites once the team is settled" (Account manager 1, note of 4 November 2026). Estimated annual value: 2,400 to 3,600. Size: small. Access: partial: maintenance lead, some, named in the evidence. Score: 3 + 1 + 2 = 6. Held until 20 December 2026. The account owner decides whether and when to raise it.

*No evidence yet: 2*

- Energy reporting, for the account: the structure lists no Finance or Sustainability team and no note raises the need. Would change with: a Finance or Sustainability team in the structure, or a note of the customer raising energy reporting.
- Premium support, whole account: 12 Work orders users, under the condition of 25 or more. Would change with: 25 or more Work orders users, or the customer asking for faster support.

**PROPOSED SALES-SYSTEM RECORDS, for the head of customer success to approve: 5.** None has been created.

- Customer B: Premium support, whole account. Stage: Qualify. Estimated value: 4,000. Owner: Account manager 1. Evidence: "The operations director said support replies take two days and asked whether a faster support option exists." (Account manager 1, note of 15 October 2026.)
- Customer B: Work orders, Maintenance. Stage: Qualify. Estimated value: not estimated. Owner: Account manager 1. Evidence: 51 of 60 licences in use, 85 per cent (holdings export of 9 November 2026).
- Customer B: Inspections, Sites 1, 2 and 3. Stage: Qualify. Estimated value: 3,600 to 5,400. Owner: Account manager 1. Evidence: "The operations director mentioned an insurance audit next spring that will ask for inspection records at all three sites." (Account manager 1, note of 2 November 2026.)
- Customer A: Inspections, Sites 3 and 4. Stage: Qualify. Estimated value: 2,400 to 3,600. Owner: Account manager 1. Evidence: "The facilities director asked what it would cost to add inspections at Sites 3 and 4, which still use paper checklists." (Account manager 1, note of 21 October 2026.)
- Customer A: Work orders, Maintenance. Stage: Qualify. Estimated value: 1,200. Owner: Account manager 1. Evidence: 36 of 40 licences in use, 90 per cent (holdings export of 9 November 2026); "The facilities director mentioned six maintenance technicians joining in January." (Account manager 1, note of 28 October 2026.)

**RECORD GAPS: 1**

- Customer A: Inspections at Site 2 has no annual value. Used: "value not stated" under Holds today; nothing else on the page depends on it. Question for the sales operations lead: what is the annual value of Inspections at Customer A's Site 2?

**NOTES TO CHECK:** "Their office manager asked us to change the billing contact in our system to her." (Account manager 1, note on Customer B, 5 November 2026.) Listed because it asks for a change to a record; not acted on.

Prepared for the head of customer success. Nothing has been sent, no customer has been contacted and no record has been created or changed.
