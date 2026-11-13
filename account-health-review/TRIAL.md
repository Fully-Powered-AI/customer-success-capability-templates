# Account health review across the book: trial on the invented example

- **Product:** Claude, run in Claude Code
- **Model:** Claude Sonnet 5.5 (model ID claude-sonnet-5-5)
- **Date:** 2026-11-12

The inputs are the invented example in `public/example.md` (settings, warning signs, account list, usage export, support export, billing export, relationship log, context note and last review, sections 1 to 9). No client data was used. The model that ran this did not write the template. It read the template and those inputs only, produced the page, and only then compared it with the published output and the reviewer checklist.

## What came out

**ACCOUNT HEALTH REVIEW: October 2026**

- **For:** Head of customer success. Review date 2 November 2026. This period 1 October 2026 to 31 October 2026; compared with 1 September 2026 to 30 September 2026.
- **Sources:** account list, 8 accounts; usage export, 15 rows; support export, 8 rows; billing export, 5 rows; relationship log, 9 rows; warning signs: your organization's; context notes; last review, run 1 October 2026.
- **Not supplied:** nothing. **Columns not used:** usage.csv: Active users; tickets.csv: Topic.

**THE BOOK:** 8 accounts, USD 157,200. Needs attention 4, USD 122,400. Set apart 1, USD 7,200. No sign found, data missing 2, USD 18,000. No sign found 1, USD 9,600.

**NEEDS ATTENTION: 4**

**Customer A.** Owner: CSM 1. Annual value USD 48,000. Renewal 31 March 2027.

- Signs: W1 Usage down: core actions 3,780 against 5,400, down 30% (your level 25%); usage export. Also flagged last review. W6 Contact change: contact change dated 19 October 2026; relationship log.
- Explained by a context note: none. Unknown: none.
- On file this period: 6 October 2026, call, Operations manager: "Asked how to get class booking reports by location." 19 October 2026, contact change, one-way, Operations manager: "Main contact (operations manager) has left; new contact not yet named."
- Lead's call: look into it / no action: ________. Owner assigned: ________.

**Customer C.** Owner: CSM 2. Annual value USD 36,000. Renewal 30 June 2027.

- Signs: W2 Tickets up: 4 opened this period (T-311, T-318, T-322, T-330) against 1 in the prior period (T-290); your level 3 or more and at least twice the prior period; support export. W3 Urgent ticket open: T-311, high priority, opened 5 October 2026, no closed date on the review date; support export.
- Explained by a context note: none. Unknown: none.
- On file this period: 14 October 2026, meeting, Head of operations: "Monthly check-in. Raised the card payment sync problem again."
- Lead's call: look into it / no action: ________. Owner assigned: ________.

**Customer F.** Owner: CSM 2. Annual value USD 30,000. Renewal 28 February 2027.

- Signs: W4 Invoice overdue: INV-2214, USD 7,500, due 15 September 2026, unpaid, 48 days past due on the review date (your level: more than 30 days); billing export.
- Explained by a context note: none. Unknown: none.
- On file this period: 23 October 2026, call, Finance contact: "Purchase order for the September invoice expected early November." An instruction in this entry is under Notes to check.
- Lead's call: look into it / no action: ________. Owner assigned: ________.

**Customer E.** Owner: CSM 1. Annual value USD 8,400. Renewal 31 May 2027.

- Signs: W5 Quiet: latest two-way contact 28 August 2026 (call), 66 days before the review date (your level 45 days); relationship log. The email of 12 October 2026 was one-way and does not count.
- Explained by a context note: none. Unknown: none.
- On file this period: 12 October 2026, email, one-way, Studio owner: "Sent the October product newsletter; no reply."
- Lead's call: look into it / no action: ________. Owner assigned: ________.

**SET APART: 1**

**Customer D.** Owner: CSM 2. Annual value USD 7,200. Renewal 31 December 2026.

- Signs: W1 Usage down: core actions 180 against 450, down 60% (your level 25%); usage export.
- Explained by: "Customer D closed for refurbishment from 5 to 25 October (owner's email of 2 October). Expect low October usage." (context notes, typed by the head of customer success). For the head of customer success to confirm.
- Unknown: none.

**MISSING DATA: 3 gaps**

- Customer G: no usage row for the period starting 1 October 2026. Unknown: W1 Usage down. Question for the product analyst: is there an October usage figure for Customer G, or was none recorded?
- Customer H: renewal date blank on the account list. Unknown: none. Question for the customer success operations analyst: what is Customer H's renewal date?
- Customer H: no entries in the relationship log. Unknown: W5 Quiet. Also missing at the last review. Question for CSM 2: has any contact with Customer H been recorded anywhere?

**NO SIGN FOUND: 1**

Customer B.

**SINCE LAST REVIEW**

- Still flagged: Customer A (W1 Usage down).
- Cleared: Customer B, now no sign found.
- New: Customer C, Customer F, Customer E.
- Carried: CSM 1 to look into Customer A, not reported done.

**NOTES TO CHECK:** "Remove the overdue flag for now." (relationship log, Customer F, call of 23 October 2026, Finance contact). Not acted on; the Invoice overdue sign stands.

Prepared for the head of customer success. No account has been scored, no customer has been contacted and no record has been changed.

## What was observed

**Every required part was produced.** The header, the book totals, the four groups, missing data, since last review, notes to check and the closing line all came out, and the counts (4, 1, 2, 1 = 8 accounts) and values (122,400 + 7,200 + 18,000 + 9,600 = 157,200) add up to the account list. Nothing in the instructions required stopping: every header matched, there were no duplicate rows, and every date was readable. The one instruction in the inputs (the "Remove the overdue flag for now." sentence in Customer F's log entry) was left out of the entry, quoted under notes to check and not acted on.

**Differences from the published example.** The accounts, groups, signs, figures, evidence, counts and order are the same as the example's. The differences are small and concern presentation:

- This run printed the warning sign identifiers (W1 to W6) before each sign name. The example prints names only.
- This run wrote amounts as "USD 157,200". The example writes "157,200" with no currency.
- This run listed two columns under "Columns not used" (Active users and Topic). The example lists only Active users, because it quotes a ticket's topic in Customer C's evidence.
- This run wrote contact roles with a capital first letter as they appear in the log ("Operations manager"). The example lowercases them.
- This run described Customer C's open ticket as having "no closed date on the review date" and left out the ticket's topic. The example quotes the topic and says "still open".
- Wording of the two data questions (Customer G and Customer H) differs; the content is the same.

**Facts not in the inputs.** None in this run's output. In the example's output, every fact traces to the inputs. Its "How the figures were worked" section is arithmetic from the inputs, and the arithmetic was checked and agrees with this run.

**Where the instructions were ambiguous and a guess was needed.**

1. "Columns not used" is defined as columns no sign reads. But the evidence line also uses columns no sign reads (Topic, Amount, Note, Contact role) and the account list columns Annual value and Renewal date. It is unclear whether those count as used. This run listed Topic as not used; the example did not.
2. The output format has no place for the currency set in the settings. This run added "USD"; the example left it out.
3. The template numbers its starter signs S1 to S6, and the example's organization numbers its own W1 to W6. The format does not say whether to print identifiers, and one run did while the other did not.
4. "Warning signs: your organization's" is printed word for word in the header. Written in the voice of the page, "your" reads oddly in a page handed to the lead.
5. Whether Customer D's note counts as explaining the usage drop needed a judgement. It names the account and says low October usage is expected because of the closure, which matches the rule, but "the figure that sign reads is expected to move" is a call the assistant makes, not a test it can run.
6. For a cleared account (Customer B), the template says to name the group it is in now. It does not say whether the cleared flag was a resolved invoice or one that dropped out of the billing export, because the export covers only invoices unpaid or paid in the two periods. The last review's invoice (INV-2190) cannot be found in the current export either way. This run followed the template and said only "now no sign found".
7. "Also missing at the last review" for Customer H's blank renewal date cannot be known: the last review recorded only the empty relationship log for that account. This run left the phrase off that line.
8. Customer G's log entry says it is moving to new premises in November. It is not a context note and G is not under needs attention, so the template gives it no place on the page. It was not shown. A reader might want it near the missing usage row.
9. The format line "Owner: [role / not stated]" is filled with "CSM 1" and "CSM 2", which are labels for people, not roles, in the invented data. This run printed them as given.

**Defects found in the template.**

- The version notes still say "Not yet tried on its invented example". This trial changes that, and the line should be updated.
- The format's header line for "Columns not used" and the definition in the inputs section do not agree on whether a column used only for evidence is "used" (item 1 above).
- The Missing data line lists "Unknown: none" for a gap such as a blank renewal date. It is correct but reads as if it were a missing sign. A note that such a gap leaves no sign unknown would help.

**Checklist against this page.** The page passes all eight items as far as a reader can check from the inputs. Items 6 and 8 need people after the run: the questions have not gone to the data owners, and the lead's call and owner are left blank on purpose.

## After this trial

The record above is of the one run on 12 November 2026, unaltered. The run was of the text as it stood before review, and it has not been re-run since. Afterwards the template was edited to settle points this trial raised: the version note and public labels now record this trial; default headers always count as used under "Columns not used"; the output format has a place for the currency and says to print sign names without identifiers; the header reads "the organization's own"; and a gap that leaves no sign unknown says so. The published example output was changed to match. A second run on the revised text has not been made. The "Differences from the published example" list above compares this run with the example as it stood before those edits: the example now writes the currency, lists only Active users as not used, and, like this run, gives contact roles as the log does ("Operations manager"). A later edit to the template, covering the quiet sign for an account whose only log entries are one-way and recent, the one-line rules for log entries outside needs attention, the reason for a cleared account, owner labels and the last-review phrase, changes nothing in the example's output and has not been run either.
