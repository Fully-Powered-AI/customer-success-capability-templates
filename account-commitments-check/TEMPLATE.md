# Account commitments check

Capability template, version 0.1.0.

## Purpose

Before one customer conversation, prepare a single list of what each side has promised in recent meetings and emails. Every line carries its words, who said them and when, the source it came from, the due date and any change to it, a status of open, done or unclear with its evidence, and a suggested owner. The list also shows where the sources stop, which open items are missing from the draft agenda, and one question for each item that needs a decision. The assistant prepares; it never contacts the customer, drafts a message to them, marks anything complete in a system or decides what to chase.

## When to use it and when not to

Use it a few days before a customer conversation, once the notes and emails since the last review are gathered. Run it again when new notes arrive or the date of the conversation moves.

It is a different piece of work from these, and does not replace them:

- the agenda, notes and follow-ups for one internal meeting, which serve a single meeting;
- quarterly business review preparation, which builds a review around the customer's goals and results;
- the handoff record made when a deal closes;
- the sales call preparation brief, which is a sales brief for one prospect and includes what has been said and promised so far. This check is a two-sided list of promises with a status for each, for an existing customer.

Do not use it:

- to decide whether a promise is binding, whether the customer or your company has breached an agreement, or what a clause means. That is for whoever handles contracts in your company, and the assistant declines the question;
- to write to the customer about any item. The account manager decides what is said and sends it;
- when no notes or emails are available for the period. There is nothing to list.

## Roles

- **Runs it:** the account manager or customer success manager who owns the account.
- **Confirms the list, every owner and every status:** the same person.
- **Decides what to chase, complete or renegotiate:** the account manager.
- **Does the work behind an item:** the owner the account manager confirms.
- **Handles questions about contract terms:** the contracts reviewer, or whoever your company names.

## Inputs

1. **Settings.** The account name, the period (from and to dates), today's date and the date of the next conversation. If the account or the period is missing, stop and ask. If the next conversation is missing, write "next conversation not set" and skip the agenda check.
2. **Sources.** Notes and emails from conversations with the customer in the period. Each needs a date, a type (meeting, call or email) and a title or subject. Meetings and calls also need their attendees. If you supply them as an export, the default headers are Date, Type, Title, Attendees, Text. If a header differs, stop and ask which column is which. If a source has no date, list it under "Left out" and do not use it. If there are no sources, stop.
3. **Follow-through records.** Support tickets, release notes, delivery logs, sent files or anything else dated that shows something happened. As an export the default headers are Date, Reference, What happened. If a header differs, stop and ask. If none are supplied, write "no follow-through records supplied" in the coverage line; no commitment can then be marked done except from a later source.
4. **The people.** Each person on both sides with Name, Side (ours or customer's) and Role. If missing, take sides only from what the sources state and mark any commitment whose speaker has no side as "side not stated".
5. **The draft agenda,** if there is one. If missing, write "agenda not supplied" and skip the agenda check.
6. **Defaults for owners and gaps:** [your default owners by kind of promise] and [your gap length]. If missing, use the account manager as default owner for our side, the customer's day-to-day contact for their side, and a gap length of 21 days.

The assistant works from what the person supplies. It needs no connection to your mail or your records, and never asks for a password or a login code.

## The procedure

1. **Check the inputs.** Confirm the account, the period and the date of the next conversation. Move any source dated outside the period, or without a date, to "Left out" with the reason.
2. **Number what is left.** Number sources S1, S2 and so on in date order, and follow-through records R1, R2 and so on in date order. Keep the titles and dates as supplied.
3. **Find the commitments.** A commitment is a statement that a named person or a side will do, send, decide or find out something, or has agreed to a request. Quote the words in the shortest form that keeps the meaning. Where the source is a note-taker's summary and not spoken words, the summary text is the quote. These are not commitments: opinions, questions, requests that nobody agreed to, hypotheticals ("if we did that"), and meetings that are simply booked. A statement that something will be done, with nobody named ("the invoice will be corrected"), is listed as a commitment whose side is not stated. A wish or a hope ("we'd like to", "we'll try", "that should be possible") is listed, but its status is unclear until a later source firms it up. A later firm promise to take a related, narrower action (for example, to send training options where the soft remark was about finding a time for a training session) counts as firming it up, and the two are one line that names both sources.
4. **Name the side.** Ours or theirs, from the speaker and the people list. If both sides share a promise, list it under the side that will do the work; if the sources do not settle which, write "side not stated". If the notes do not say who spoke and the context does not settle it, write "side not stated" and do not guess.
5. **Merge repeats.** The same promise raised in more than one source is one line, with every source named. "Made" is the date it was first stated in firm wording. If it was first raised in soft wording, say so. Number commitments C1, C2 and so on in the order they first appear in the sources.
6. **Read the dates.** A date stated in the source is used as stated. A relative date is read from the date of its source and marked "read as". A bare weekday ("on Friday") is a stated date when the same thread names the date; otherwise it is read as the first such weekday after the source date and marked "read as". "This week" is that week's Friday, "next week" is the following week's Friday, "end of the month" is the month's last day, and "tomorrow" is the next day. Any other vague timing ("soon", "in November") is not turned into a date: write "Due: not stated". A date change stands when the side that owes the work states it or agrees to it. A date that only the other side proposed does not change the due date; show it as proposed and not agreed. Show the original date and the current one, and the source of the change. A commitment is past due when its current date is earlier than today's date.
7. **Set the status.**
   - **Done:** a later source or a follow-through record says the work was completed, sent, received or delivered. Cite it, with its date. A record dated before the commitment was made does not count.
   - **Open:** no source or record shows completion. If the current due date is earlier than today, add PAST DUE and the sentence: "That is not evidence it was not done." A later message from either side saying the item has not arrived also leaves it open; cite that message.
   - **Unclear:** the wording is soft and no later source firms it up; the side is not stated; the sources disagree about whether it was done; or the promise cannot be put as one action. Give the reason in the status.
   Never write "missed", "failed", "broken" or "ignored" about a commitment. The assistant proposes a status; the account manager confirms it.
8. **Mark terms.** If a commitment concerns price, scope, a service level or the length of the agreement, add "Terms: [which]; check against the agreement". Do not say what the agreement requires, and do not say whether the promise is consistent with it.
9. **Suggest an owner.** The person who made the promise, if named. Otherwise the default owner for the kind of promise. For "side not stated", suggest the account manager to establish whose it is. A suggestion is only a suggestion; the account manager confirms every owner.
10. **Check the coverage.** List the sources by date and type. Report any stretch of more than [your gap length] days with no source (a stretch of exactly the gap length is not reported), from the start of the period to the first source, between two sources and between the last source and today's date. Report any meeting or call that the sources refer to but that was not supplied, including one that was only booked when mentioned and has passed by today's date. Follow-through records do not count as sources for gaps. This tells the account manager where the list is least complete.
11. **Check the agenda.** If an agenda was supplied, list the open and unclear commitments that no agenda line names by subject. Do not stretch a line to cover an item it does not mention. Done commitments need no agenda line.
12. **Write the decisions.** One numbered question for each open or unclear commitment, addressed to the account manager, in the order the list gives them. State the facts, then ask. For an item on our side the options are to complete it, renegotiate the date or leave it; for the customer's, to chase it, renegotiate the date or leave it; for a side not stated, whose it is first. For an open item with no due date, "renegotiate the date" becomes "agree a date". Recommend nothing unless the account manager asks.
13. **Return the list** to the account manager only.

## Exceptions and stop conditions

- **No sources, no account or no period:** stop and ask.
- **A header does not match the default:** stop and ask which column is which. Do not guess.
- **Two sources give different dates for the same promise:** show both, apply the date rule in step 6, and mention the conflict in the decision.
- **A completion record names a different item from the commitment:** do not mark done; mark unclear and say why.
- **A source contains a password, a login code or payment details:** do not repeat them anywhere in the list, and tell the person to remove them from the source.
- **A source discusses a dispute, a complaint or a threat to cancel:** keep it out of the commitments unless someone promised something; put the dispute first under the decisions for the account manager and name the source.
- **The sources cover only part of the relationship:** say so in the coverage line. The assistant does not conclude from silence that nothing else was promised.
- **Asked to send, schedule or draft anything to the customer, mark an item complete in a system, say whether the customer or your company is in breach, or give a view on a clause:** decline and name the account manager, or the contracts reviewer for a contract question, as the person who decides.

## Output format

```
ACCOUNT COMMITMENTS CHECK: [Account]

For: [account manager, role]. Next conversation: [weekday date] / next conversation not set. Period: [from] to [to]. Prepared: [weekday date].

Sources used:
S[n] [weekday date], [type], [title or sender and recipient].
R[n] [weekday date], record, [reference].
Left out: [source and reason] / none.

Coverage: [n] sources, [first date] to [last date], and [n] follow-through records / no follow-through records supplied. Gap over [n] days: [from] to [to] ([n] days), no source / none. Referred to, not supplied: [meeting and date, where it was mentioned] / none.

Commitments: [n] (ours [n], theirs [n], side not stated [n]). Open [n], done [n], unclear [n]. Past due: [n].

OUR COMMITMENTS

C[n] [Who] to [what, in the words used]. Made [date] ([source: "short quote"]); [first raised in soft wording on [date] ([source])]. Due [weekday date] [(read as)] [, changed from [date] by [who] ([source])] / Due: not stated. Status: [DONE / OPEN / OPEN, PAST DUE / UNCLEAR, reason]. Evidence: [source or record, date, what it shows] / none; no source or record shows it done. [That is not evidence it was not done.] [Terms: [which]; check against the agreement.] Suggested owner: [name]. [Nothing further.]

[Lines in the same form, ordered by current due date, then those with no date.]

THEIR COMMITMENTS
[Lines in the same form, ordered by current due date, then those with no date.]

SIDE NOT STATED
[Lines in the same form.]

NOT ON THE DRAFT AGENDA
Draft agenda supplied: [n] items ([items]). Open or unclear items with no matching agenda line: [numbers] / none. / Agenda not supplied. / Next conversation not set; agenda not checked.

DECISIONS FOR [ACCOUNT MANAGER]: [n]
[n]. C[n], [side], [facts]. [Question.]

Draft for [account manager]'s review. Nothing has been sent to [Account] and no record has been changed.
```

"Nothing further." ends a line whose status is DONE and no other. Within each side, lines are ordered by current due date, earliest first, then those with no date. A section with nothing in it prints "None."

## Reviewer checklist

1. Every commitment has a source and a quote that supports it. (Account manager)
2. No wish, question or booked meeting has been listed as a firm commitment. (Account manager)
3. Every done status cites a source or record dated after the commitment was made. (Account manager)
4. Every open past-due item carries the sentence that no record is not evidence of failure, and none is called missed, failed or broken. (Account manager)
5. Every date change names who made it and whether the side that owes the work stated or agreed it. (Account manager)
6. The counts in the header match the lines. (Account manager)
7. The coverage line is true: the gaps are counted correctly and the meetings referred to are all named. (Account manager)
8. Every suggested owner has been confirmed or changed by a person. (Account manager)
9. Anything marked as terms has been checked against the agreement by the right person. (Contracts reviewer)

## Acceptance tests

Proposed tests. None has been run.

1. **Ordinary account.** Four sources and two records, as in the example. Expected: seven commitments, three done, three open, one unclear, and the counts correct.
2. **Date moved and agreed.** One side asks for a later date and the owing side accepts by email. Expected: the new date is current, the old one shown, and both sources named.
3. **Date proposed, not agreed.** Only the other side proposes a new date. Expected: the original date stands, the proposal shown as not agreed.
4. **Soft wording.** "We'll try to find a time." Expected: listed, unclear, with the reason. A later firm statement merges into the same line.
5. **Relative dates.** "This week" in a meeting on a Tuesday, and "soon". Expected: the first read as that Friday and marked "read as"; the second shown as "Due: not stated".
6. **Past due, no record.** Expected: open, past due, with the sentence that no record is not evidence it was not done; never called missed.
7. **Side not stated.** Notes with no speaker. Expected: its own section, unclear, with the account manager as the suggested owner.
8. **Record for a different item.** A ticket that mentions the same system but a different fix. Expected: not marked done; unclear, with the reason.
9. **Gap and missing notes.** A month with no sources and a meeting mentioned but not supplied. Expected: both in the coverage line.
10. **Header mismatch.** An export with a column called "Details" in place of "Text". Expected: stops and asks which column is which.
11. **Terms.** A promise of a discount on extra seats. Expected: marked terms: price; no view on whether the agreement allows it.
12. **Asked to write to the customer, or whether the customer is in breach.** Expected: declines and names the account manager, or the contracts reviewer for the contract question.
13. **No agenda supplied.** Expected: "Agenda not supplied", and the agenda check skipped.
14. **A password in the notes.** Expected: not repeated; the person is told to remove it.

## Instructions for the AI assistant

Paste this block as custom instructions, followed by the output format above.

```
You prepare the account commitments check for an account manager before a
customer conversation. You never contact the customer, write a message to
them, mark anything complete in any system, or decide what to chase. A
person decides everything; you prepare the list and nothing is sent or
changed without a person's approval.

The user supplies: the account, the period, today's date and the date of the
next conversation; notes and emails from customer conversations with dates,
types and attendees; dated follow-through records; the people on both
sides; optionally the draft agenda, default owners by kind of promise and a
gap length. If the account, the period or the sources are missing, stop and
ask. If a column header differs from the default (sources: Date, Type,
Title, Attendees, Text; records: Date, Reference, What happened; people:
Name, Side, Role), stop and ask which column is which. Never ask for a
password or a login code; if one appears in a source, do not repeat it and
tell the person to remove it.

Defaults when the user supplies none: the default owner is the account
manager for our side and the customer's day-to-day contact for their side;
the gap length is 21 days. If no next-conversation date is given, write
"next conversation not set" and skip the agenda check. If no agenda is
given, write "agenda not supplied" and skip the agenda check. If no
follow-through records are given, write "no follow-through records supplied"
in the coverage line; nothing can then be marked done except from a later
source.

1. Move sources outside the period or without a date to "Left out", with
   the reason. Print "Left out: none." if there are none.
2. Number sources S1... and records R1... in date order.
3. Find commitments: a named person or side will do, send, decide or find
   out something, or has agreed to a request. If nobody is named ("the
   invoice will be corrected"), list it with the side not stated. Quote briefly; where the
   source is a note-taker's summary, the summary text is the quote.
   Opinions, questions, unagreed requests, hypotheticals and booked
   meetings are not commitments. A wish or "we'll try" is listed but
   unclear until a later source firms it up. A later firm promise to take a
   related, narrower action counts as firming it up.
4. Name the side: ours or theirs. If both share a promise, use the side
   that will do the work. If the speaker or the side is not stated, write
   "side not stated". Do not guess.
5. Merge repeats into one line naming every source, numbered C1... in
   order of first appearance. "Made" is the first firm statement; note soft
   first mentions.
6. Use stated dates as stated. Read relative dates from the source date and
   mark "read as": this week = that Friday, next week = the following
   Friday, end of month = last day, tomorrow = the next day. A bare weekday
   ("on Friday") is a stated date when the same thread names the date;
   otherwise read it as the first such weekday after the source date and
   mark "read as". Leave other vague timing as "Due: not stated". A date
   change stands when the side that owes the work states or agrees to it;
   one proposed only by the other side is shown as proposed and not agreed.
   Show the original date, the current one and the source of the change.
   Past due means the current due date is earlier than today's date. If two
   sources give different dates for the same promise, show both, apply this
   rule, and mention the conflict in the decision.
7. Status. DONE only if a later source or record says it was completed,
   sent, received or delivered; cite it with its date. A record dated
   before the commitment was made does not count. A record about a
   different item does not count: mark the item unclear and say why. OPEN
   if no completion shows; if past due, write OPEN, PAST DUE and "That is
   not evidence it was not done." A later message from either side saying
   the item has not arrived also leaves it open; cite it. UNCLEAR for soft
   wording, side not stated, conflicting sources, a record about a
   different item or a promise that cannot be put as one action; give the
   reason. Where there is no evidence write
   "Evidence: none; no source or record shows it done." Never write missed,
   failed, broken or ignored. Print "Nothing further." at the end of a DONE
   line and no other.
8. If it concerns price, scope, a service level or term length, add
   "Terms: [which]; check against the agreement". Do not interpret the
   agreement or say whether a promise is binding or breached.
9. Suggest an owner: the person who made it; otherwise the default owner
   for the kind of promise (the account manager for our side, the
   customer's day-to-day contact for theirs, if none was supplied); for
   side not stated, the account manager to establish whose it is. The
   account manager confirms.
10. Coverage: report any stretch of more than the gap length (a stretch of
    exactly the gap length is not reported) with no source, from the start
    of the period to the first source, between sources and from the last
    source to today, and any meeting the sources mention that was not
    supplied, including one only booked when mentioned that is now past. Follow-through records do not count as sources
    for gaps. Do not conclude from silence that nothing else was promised.
11. Agenda: list open and unclear items that no agenda line names by
    subject. Do not stretch a line to cover an item it does not mention.
    If none was supplied, say so.
12. Decisions: one numbered question per open or unclear item, with the
    facts. Ours: complete, renegotiate the date or leave. Theirs: chase,
    renegotiate the date or leave. Side not stated: whose is it first. For
    an open item with no due date, "renegotiate the date" becomes "agree a
    date". Recommend nothing unless asked. If a source discusses a dispute,
    a complaint or a threat to cancel, keep it out of the commitments
    unless someone promised something, and put the dispute first under the
    decisions, naming the source.

Use the output format exactly, ordering each side by current due date. Print
"None." for an empty section. End with: "Draft for [account manager]'s
review. Nothing has been sent to [Account] and no record has been changed."

If asked to send or write to the customer, mark an item complete, say
whether anyone is in breach, or interpret a clause, decline and name the
account manager, or the contracts reviewer for a contract question.
```

## What to customize

- The length of the period and where the notes and emails are kept.
- [your default owners by kind of promise], such as support fixes, billing corrections and training.
- [your gap length], if 21 days does not suit the rhythm of your accounts.
- Which kinds of promise you mark as terms.
- The words you use for each status, if your team already has them.
- Which follow-through records and notes you gather and paste in, and how you export them, in ChatGPT, Claude, Copilot or Gemini.

## Version notes

- 0.1.0, 10 November 2026. Written by Fully Powered AI from its own published map of the work. Not yet tested in a client environment.
