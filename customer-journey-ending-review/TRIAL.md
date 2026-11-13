# Trial of the customer journey ending review on its invented example

- **Product:** Claude, run in Claude Code

Model: Claude Sonnet 5.5 (model ID claude-sonnet-5-5). Date: 2026-11-11.

The inputs were the invented example published with this template (Company A, Customer B). No client data was used. I used only the four inputs in `public/example.md` (the brief, the six completion criteria, the 22-row journey log and the two feedback items). I followed the instruction block and the output format in `member/template.md`, produced the review, and only then read the example's own output and the reviewer checklist. I did not write the template.

## What came out

All twelve procedure steps ran and every part of the output format was produced. Nothing stopped the run. The substantial parts:

- **Counts:** 22 log rows: 20 in the window, 2 after the end, 0 before the start. Defaults used for all four settings.
- **Ending:** Ended with work open and a question unanswered. Final handoff E19, 23 October 2026, video call, Project manager. 3 criteria met by the handoff (C1, C2, C4); 3 open at the handoff; 2 still open on 11 November (C3 partly met, C6 not recorded). C5 met after the handoff (E22, 29 October). Question unanswered at the handoff: E17 (21 October). Closing words against open work: E19 ("project marked closed") and E20 ("the project is complete"), while C3, C5 and C6 were open. Low score: F1, 5 on 0 to 10. After the end: E21 (unanswered, 15 days open) and E22.
- **Difficult moments (4):**
  - M1, 4 to 14 September, Build: missed date, E03 to E04, 3 days late.
  - M2, 16 September to 1 October, Build: silence of 15 days between E06 and E09; slow reply E07 to E09 (7 days, 5 over the target); asked again E08. Named in feedback: F2. Proposed link: F1 ("promotion", "launch moved").
  - M3, 9 to 27 October, Launch and Handover: missed date E13 to E16 (5 days late); slow reply E15 to E16 (3 days, 1 over); E17 unanswered (21 days open); E21 unanswered (15 days open) and asked again. Open criterion C3. Proposed link: F1 ("express delivery").
  - M4, 23 to 29 October, Handover: missed date E19 to E22 (admin guide due 26 October, sent 29 October, 3 days late).
- **Moments to look at first:** 1. M3 (rule a, C3 open). 2. M2 (rule b, F2 refers to E09). 3. M4 (rule d, 3 days late, level with M1, nearer the handoff).
- **In the customer's words:** F2 (call note) shown as the note-taker's words; F1 quoted exactly in quotation marks with its score.
- **Readings:** one for each of M3, M2 and M4, each starting "The records are consistent with" and ending with how to confirm it (ask the customer whether express delivery still shows zero and who supports the store; check in the project tool when the import problem was first found; ask whether the staff needed the guide before it arrived).
- **Options:** O1 finish C3, O2 finish C6, O3 reply on T5 (E17, E21); O4 to O7 four changes to test (one for each of M3, M2, M4, and one for the ending), each at one stage, with a count over the next 5 journeys; O8 the C6 gap in the records; O9 F1 has no refers_to.
- **Decisions for the customer success lead:** which change to test (O4 to O7); work open (C3, C6); thread T5; the promotion weekend F1 says was lost (whether and how to acknowledge, no amount); records changes (O8, O9); referrals none.
- Nothing under NOT CHECKED. Nothing about a refund, chargeback or legal claim, so no referral.

## What I observed

Compared with the published example's output:

- **Nearly identical.** The counts, the ending, the criteria lines, the four moments and their day counts, the ranking of moments, the quoted feedback, the options O1 to O3, O8 and O9, and the decisions agree. Differences were small.
- **Difference 1, a proposed link.** The example links F1 to M4 on "the training was clear" (E19, "two staff trained"). I did not: "training" and "trained" are not the same words, and the template says to quote the shared words. The template does not say whether a shared word stem counts. Also, F1 links to two moments in my output and three in the example; the output format has room for only one link per item.
- **Difference 2, wording of the changes and readings.** My O4 to O7 differ in wording from the example's (for example my change for M3 concerned replies to a reported fault, the example's concerned giving every open customer question a named owner before the handover call). Both fit the rules. The template leaves the choice of change to the assistant, so this will vary from run to run.
- **Difference 3, the M4 reading.** The example says the two trained staff were "working without the admin guide for six days"; I did not say that. The records show the guide arrived six days after the handover but do not show anyone working without it. That phrase is a step beyond the records.
- **Facts not in the inputs.** In my output, none beyond the readings' inferences, which are marked as readings to confirm. In the example, "working without the admin guide" is the one statement that goes beyond the records. The example's O1 also says "no test order for it is recorded", which is true of the log but an inference from silence.

Where the instructions were ambiguous and I had to choose:

1. **"Any event in it" (open criterion, after the end).** It does not say whether a moment's events are only the events named in its findings or every log row dated inside its span. For M2 the internal note E10 sits inside the silence; I used only the events named in findings. The result was the same here.
2. **A feedback item with two or more proposed links.** F1 matches M2 and M3. The format line allows one; I listed both.
3. **A stage named in `refers_to` for a moment that spans two stages.** "Lies wholly in that stage" is clear, but M3 spans Launch and Handover so no stage reference could name it. This did not arise here.
4. **A promised date not in the summary.** E19 has a `due_date` of 26 October but its summary does not say the date was told to the customer. The missed-date rule is mechanical and counted it. The reading for M4 therefore cannot say the customer was told 26 October; the "to confirm" line asks about it.
5. **A `fulfils` link to a partial fix.** E16 is marked as fulfilling E13 (the test order promised by 15 October) although the live-order test was only partly done (C3 is "partly met"). The rule counts the promise as 5 days late and delivered; a person may think the promise was not truly kept.
6. **"Unanswered on the handoff date".** I read this as: asked on or before the handoff and not answered by the handoff date. E17 qualifies either way, so the ambiguity did not change the result.
7. **Tie in rule (d).** M1 and M4 were both 3 days late; the "nearer to the final handoff" rule settled it. This worked as written.

I was told to stop for nothing: all headers matched, ids were unique, dates were readable, E19 is in the log, and the log has items from the customer. I did not test any stop condition, the refund referral, the fault question or the contact limits, because the example holds none of them.

One shortcoming of the trial: it was one run on one small example by one model, and the day counts were worked by hand. It shows the instructions can be followed to a result almost the same as the published one. It does not show how a different model, or a messy real export, would behave.
