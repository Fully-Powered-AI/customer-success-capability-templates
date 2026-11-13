# Customer journey ending review: an invented example

*Illustrative example with invented data.* Company A, Customer B, the people, the records and the dates below are all invented. Company A is an invented 30-person digital agency that builds online stores for small retailers and hands each one over at the end of the project. Customer B, an invented home-goods retailer, gave the close survey 5 out of 10. Noor Ellery, Company A's customer experience lead, supplied the inputs below in full on Wednesday 11 November 2026; the review the workflow template returned comes after them.

## The inputs

### 1. The review brief

```
Customer: Customer B
Journey type: project close (a new online store, built and handed over)
Journey start: 2026-09-01
Final handoff: E19
Review date: 2026-11-11
Review owner: Noor Ellery, customer experience lead
Decision by: customer success lead
Reason for review: Customer B scored the close survey 5 out of 10.
Contact limits: none
Settings: (left blank: use the defaults)
```

### 2. The completion criteria

```
criterion_id,criterion,status_at_end,evidence_event,owner
C1,Store live on the customer's own domain,met,E14,Project manager
C2,Product catalogue imported and checked by the customer,met,E12,Project manager
C3,Payment and delivery settings tested with a live order,partly met,E16,Developer
C4,Two of the customer's staff trained to add products and process orders,met,E19,Project manager
C5,Admin guide delivered,met,E22,Project manager
C6,Support contact and hours confirmed to the customer in writing,not recorded,,Customer success manager
```

### 3. The journey log (exported from the project tool and the shared inbox)

```
event_id,date,thread,stage,channel,direction,owner,summary,criterion,due_date,fulfils
E01,2026-09-01,T1,Kickoff,video call,to customer,Project manager,"Kickoff call: scope agreed; launch planned for 9 October",,,
E02,2026-09-03,T2,Build,email,from customer,Project manager,"Sends the product spreadsheet; asks when he will see the first designs",C2,,
E03,2026-09-04,T2,Build,email,to customer,Project manager,"Says the first designs will be shared by 11 September",,2026-09-11,
E04,2026-09-14,T2,Build,email,to customer,Designer,"Shares the first designs for comment",,,E03
E05,2026-09-15,T2,Build,email,from customer,Designer,"Approves the designs with two changes",,,
E06,2026-09-16,T2,Build,email,to customer,Designer,"Confirms the two changes are made",,,
E07,2026-09-24,T3,Build,email,from customer,Project manager,"Asks whether the launch is still 9 October",,,
E08,2026-09-29,T3,Build,email,from customer,Project manager,"Asks again about the launch date; says a promotion is booked for the weekend of 10 October",,,
E09,2026-10-01,T3,Build,phone call,to customer,Project manager,"Call: the launch moves to 16 October because the catalogue import needs fixing",C2,,
E10,2026-10-01,T3,Build,internal note,internal,Project manager,"Catalogue import: 140 products missing prices; developer to fix",C2,,
E11,2026-10-02,T4,Launch,email,to customer,Project manager,"Sends the fixed catalogue and asks the customer to check it",C2,,
E12,2026-10-08,T4,Launch,email,from customer,Project manager,"Catalogue checked and approved",C2,,
E13,2026-10-09,T4,Launch,email,to customer,Project manager,"Confirms launch on 16 October; says a test order will be placed by 15 October",C3,2026-10-15,
E14,2026-10-16,T4,Launch,email,to customer,Project manager,"The store is live on the customer's domain",C1,,
E15,2026-10-17,T5,Launch,email,from customer,Project manager,"Two shoppers report that the delivery charge shows as zero at checkout",C3,,
E16,2026-10-20,T5,Launch,email,to customer,Developer,"Standard delivery charge fixed and a test order placed; express delivery still shows zero",C3,,E13
E17,2026-10-21,T5,Launch,email,from customer,Developer,"Asks when express delivery will be fixed",C3,,
E18,2026-10-22,T6,Handover,email,to customer,Customer success manager,"Invites the customer to the handover call on 23 October",,,
E19,2026-10-23,T6,Handover,video call,to customer,Project manager,"Handover call: two staff trained; project marked closed; admin guide to follow",C4,2026-10-26,
E20,2026-10-23,T6,Handover,email,to customer,Customer success manager,"Thank-you note: the project is complete; link to the close survey",,,
E21,2026-10-27,T5,Handover,email,from customer,Customer success manager,"Express delivery still shows zero; asks who to contact now the project is closed",C3,,
E22,2026-10-29,T7,Handover,email,to customer,Project manager,"Sends the admin guide",C5,,E19
```

### 4. The customer feedback

```
feedback_id,date,source,person,score,scale,refers_to,text
F1,2026-10-26,survey,"Tomas Reade, owner, Customer B",5,0 to 10,,"The store looks great and the training was clear. But we lost our promotion weekend when the launch moved, and nobody has told us when express delivery will work."
F2,2026-10-01,call note,"Tomas Reade, owner, Customer B",,,E09,"Not happy that the launch moved after the promotion was booked. Asked why he was not told sooner."
```

## The output

**JOURNEY ENDING REVIEW: Customer B, project close**

**For:** Noor Ellery, customer experience lead. **Decision by:** customer success lead. Prepared 11 November 2026 from: brief; completion criteria (6); journey log (22 rows: 20 in the window, 2 after the end, 0 before the start, left out); feedback (2 items).
**Reason for review:** Customer B scored the close survey 5 out of 10. **Settings:** reply target 2 days; silence limit 10 days; low score 6 or below on 0 to 10, 2 or below on 1 to 5; changes measured on the next 5 journeys. Defaults used: all four settings. **Contact limits:** none.

**HOW IT ENDED**

- **Final handoff:** E19, 23 October 2026, video call, Project manager: Handover call: two staff trained; project marked closed; admin guide to follow.
- **Ending:** Ended with work open and a question unanswered.
- **Criteria:** 3 met by the handoff; 3 open at the handoff; 2 still open on 11 November 2026.
  - C1 Store live on the customer's own domain: met by the handoff, E14 on 16 October 2026. Owner: Project manager.
  - C2 Product catalogue imported and checked by the customer: met by the handoff, E12 on 8 October 2026. Owner: Project manager.
  - C3 Payment and delivery settings tested with a live order: partly met, E16 on 20 October 2026: standard delivery charge fixed and a test order placed; express delivery still shows zero. Owner: Developer.
  - C4 Two of the customer's staff trained to add products and process orders: met by the handoff, E19 on 23 October 2026. Owner: Project manager.
  - C5 Admin guide delivered: met after the handoff, E22 on 29 October 2026. Owner: Project manager.
  - C6 Support contact and hours confirmed to the customer in writing: not recorded. Owner: Customer success manager.
- **Questions unanswered at the handoff:** E17, 21 October 2026.
- **Closing words against open work:** E19, 23 October 2026: Handover call: two staff trained; project marked closed; admin guide to follow, while C3, C5 and C6 were open. E20, 23 October 2026: Thank-you note: the project is complete; link to the close survey, while C3, C5 and C6 were open.
- **Low scores:** F1, 5 on 0 to 10, cut-off 6 or below.
- **After the end:** E21, 27 October 2026, from customer: Express delivery still shows zero; asks who to contact now the project is closed; unanswered. E22, 29 October 2026, to customer: Sends the admin guide.

**DIFFICULT MOMENTS (4), in date order**

- **M1.** 4 September to 14 September 2026, Build. Missed date: E03 said the first designs would be shared by 11 September; E04 shared them on 14 September, 3 days late. Open criterion: none. Named in feedback: none. Proposed link: none.
- **M2.** 16 September to 1 October 2026, Build. Silence: no item to the customer from E06 (16 September) to E09 (1 October), 15 days. Slow reply: E07 (24 September) answered by E09 (1 October), 7 days, 5 over the target. Asked again: E08 (29 September), with no item to the customer since E07; answered by E09 in 2 days. Open criterion: none. Named in feedback: F2. Proposed link: F1, "the launch" (E09, "the launch moves"), "promotion" and "weekend" (E08, "a promotion is booked for the weekend").
- **M3.** 9 October to 27 October 2026, Launch and Handover. Missed date: E13 said a test order would be placed by 15 October; E16 placed it on 20 October, 5 days late. Slow reply: E15 (17 October) answered by E16 (20 October), 3 days, 1 over the target. Unanswered: E17 (21 October), 21 days open on 11 November. Asked again: E21 (27 October), with no item to the customer since E17; unanswered, 15 days open on 11 November. Open criterion: C3. Named in feedback: none. Proposed link: F1, "express delivery" (E16, E17, E21). After the end: E21.
- **M4.** 23 October to 29 October 2026, Handover. Missed date: E19 said the admin guide would follow, due 26 October; E22 sent it on 29 October, 3 days late. Open criterion: none. Named in feedback: none. Proposed link: none. After the end: E22.

**MOMENTS TO LOOK AT FIRST**

1. M3, placed by rule (a): it touches C3, still open.
2. M2, placed by rule (b): F2 refers to E09.
3. M4, placed by rule (d): 3 days late, level with M1, and nearer to the final handoff.

**IN THE CUSTOMER'S WORDS**

- F2, 1 October 2026, call note, Tomas Reade, owner, Customer B, the note-taker's words: Not happy that the launch moved after the promotion was booked. Asked why he was not told sooner. Link: E09.
- F1, 26 October 2026, survey, Tomas Reade, owner, Customer B, score 5 on 0 to 10: "The store looks great and the training was clear. But we lost our promotion weekend when the launch moved, and nobody has told us when express delivery will work." Link: proposed link to M2, "the launch", "promotion", "weekend"; proposed link to M3, "express delivery".

**READINGS, TO CONFIRM**

1. M3: The records are consistent with the customer leaving the project without knowing who owns the express delivery problem: E17 asked when it would be fixed and had no reply, E19 and E20 described the project as closed and complete two days later, and E21 asks who to contact now. Rests on: E17, E19, E20, E21, F1. To confirm: ask the customer whether express delivery still shows zero at checkout and whether they know who supports the store now.
2. M2: The records are consistent with the customer hearing of the launch delay only after asking twice, once a promotion had been booked: E07 and E08 asked about the date, E08 names the promotion, and the new date came in the call E09 on 1 October; the earliest records of the import problem in the log are E09 ("because the catalogue import needs fixing") and the internal note E10, both dated 1 October. Rests on: E07, E08, E09, E10, F1, F2. To confirm: check in the project tool when the catalogue import problem was first found.
3. M4: The records are consistent with the admin guide reaching the customer six days after the handover call: E19 said it would follow by 26 October, and E22 sent it on 29 October. Rests on: E19, E22. To confirm: ask the two staff whether they needed the guide in the week after the handover call.

**FOLLOW-UP OPTIONS (for the customer success lead to choose; none is recommended)**

*For this customer:*

- **O1.** Finish C3: express delivery still shows zero at checkout (E16), and E16 records a test order for standard delivery only. Rests on: C3, E16, E17, E21. Owner if chosen: Developer.
- **O2.** Finish C6: no written confirmation of the support contact and hours is recorded. Rests on: C6, E21. Owner if chosen: Customer success manager.
- **O3.** Reply on T5 to E17 and E21: where express delivery stands and who supports the store now the project is closed. Rests on: E17, E21. Owner if chosen: Customer success manager.

*Changes to test in the journey (proposed, untested):*

- **O4.** At Handover: before the handover call, every customer question still open on a thread is given to a named owner, and the customer is told who that is. Rests on: M3. How you would know: items from the customer still unanswered on the final handoff date, from the journey log, over the next 5 journeys of this type. Owner if chosen: owner to choose.
- **O5.** At Build: when the launch date is at risk, the customer is told on the day the risk is first recorded, before they ask. Rests on: M2. How you would know: items from the customer asking about the launch date before a change to it was announced, from the journey log, over the next 5 journeys of this type. Owner if chosen: owner to choose.
- **O6.** At Handover: the admin guide is sent before or during the handover call, not after it. Rests on: M4. How you would know: days between the final handoff and the admin guide's evidence item, from the completion criteria and the journey log, over the next 5 journeys of this type. Owner if chosen: owner to choose.
- **O7.** At Handover: the project is called closed, and the thank-you note sent, only once every completion criterion is met; until then the customer hears what is still open and who owns it. Rests on: the ending (E19, E20; C3, C5, C6). How you would know: criteria open at the final handoff, from the completion criteria, over the next 5 journeys of this type. Owner if chosen: owner to choose.

*For the records:*

- **O8.** C6 is "not recorded": record each criterion's status at the handoff with the logged item that shows it. Rests on: C6.
- **O9.** F1 has no refers_to: link each close survey comment to the stage or item it is about when it arrives. Rests on: F1.

**NOT CHECKED**

Nothing.

**DECISIONS FOR THE CUSTOMER SUCCESS LEAD**

1. Which change, if any, to test, and with which journeys: O4, O5, O6, O7.
2. Work still open: C3, who finishes it and whether the customer is told; C6, who finishes it and whether the customer is told.
3. Unanswered items: T5 (E17, E21), whether a person replies now, and who.
4. Losses the customer names: F1, "we lost our promotion weekend": whether and how to acknowledge it; no amount is proposed.
5. Records changes: O8, O9, whether to adopt.
6. Referrals: none.

Review for Noor Ellery and the customer success lead. Nothing has been sent, no customer has been contacted and no record has been changed.
