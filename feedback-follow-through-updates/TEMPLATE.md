# Feedback follow-through updates

Workflow template, version 0.1.0.

## Purpose

When a change ships, or a decision is made, on something customers asked for, prepare the account owner's follow-through: the list of people who asked, what each asked for, the status of their request as the responsible team has confirmed it, and one individual draft update for each person in the channel they prefer. Requests that should not get a routine update (an unclear requester, someone who asked not to be contacted, a customer who tied the request to cancelling) are held with their reason. Every date and feature in a draft traces to the confirmed change record, and each draft carries a line showing where each came from. The assistant prepares; it never sends a message, calls anyone, changes a feedback record or promises anything the team has not confirmed.

## When to use it and when not to

Use it when the responsible team (product, service or delivery) has confirmed in writing what a change does, what it leaves out and when it is available, or has decided not to go ahead, and customers have requests linked to it in the feedback tool. Run it once per change, for one account owner's accounts.

Do not use it:

- to find what customers keep asking for across a month of feedback. Grouping feedback into themes is separate work, done in Customer feedback themes;
- to follow up low satisfaction or recommendation scores. That is Customer satisfaction detractor follow-up;
- to announce a change to every customer. A release announcement goes to everyone; this update goes only to the people who asked, and speaks to what each one asked for;
- to close a support ticket about a fault that has been fixed. Support closes those on the ticket;
- when the team has not confirmed the status. Without a confirmed change record there is nothing safe to tell a customer.

## Roles

- **Runs it and approves every update:** the account owner (account manager or customer success manager) for the accounts in the run.
- **Confirms the status, the dates and what may be shared:** the responsible team's named role, usually the product manager or the service lead for the change.
- **Decides held requests:** the account owner; for a request tied to cancelling or to other suppliers or tools, together with the customer success lead.
- **Sends each update, makes each call and marks each request as updated in the feedback tool:** the account owner, or a person they name. Always a person.

## Inputs

1. **The change record,** written or confirmed by the responsible team, with these fields:
   - **Change:** its name.
   - **Item ID:** the identifier requests are linked to in the feedback tool.
   - **Decision:** shipped, scheduled or not going ahead.
   - **Available from:** the date it went live, or for a scheduled change the confirmed date, or "not confirmed".
   - **Date confirmed by:** the role and date that confirmed a future date. Needed only for a scheduled change.
   - **Available to:** all customers, or the plans, regions or groups that get it.
   - **What it does:** numbered points.
   - **What it does not do:** numbered points, each with one status: under review, planned with no date, or not going ahead.
   - **Reason we can share:** for anything not going ahead. May be blank.
   - **Workaround we can share:** the wording, and the "What it does not do" point numbers it answers. May be blank.
   - **Guide:** the help article or guide customers can read. May be blank.
   - **Search words:** words that suggest an unlinked request is about this change. If blank, use the words of the change's name.
   - **Do not mention:** internal names, targets or details that must stay out of every update. May be blank.
   - **Status confirmed by:** the role and date that confirmed the record.

   If the record is missing, or "Status confirmed by" is blank, stop. Draft nothing and list the fields the responsible team needs to fill.
2. **The feedback export,** one row per request. Default column headers: `request_id`, `received_date`, `account`, `requester_name`, `requester_role`, `channel_received`, `request_text`, `linked_item`, `plan`, `account_owner`. Extra columns are ignored. Headers match without regard to case. If any header except `plan` is missing or named differently, stop, list the expected and the found headers, and ask which column holds each. `plan` is needed only when "Available to" names a limit; if it does and `plan` is missing, stop and ask. `account_owner` is always needed, because step 3 selects on it.
3. **The contact preferences export,** one row per person. Default column headers: `account`, `requester_name`, `preferred_channel` (email, in-app message, phone call, account meeting or none), `do_not_contact` (yes or no), `notes`. `notes` may be absent. If any other header is missing or named differently, stop and ask, as for the feedback export. If the export is missing, stop: without it the assistant cannot tell who has asked not to be contacted.
4. **The run settings:** the account owner's name and role, today's date, and the responsible team's role. If the account owner is missing, stop and ask.
5. **Your style notes,** optional: sign-off, tone, any words your company avoids. If none, use the defaults in step 8.

The assistant works from the files the person supplies. It needs no connection to the feedback tool or the email system, and never asks for a password or a login code.

## The procedure

1. **Check the change record.** Confirm "Status confirmed by" names a role and a date. A future date counts as confirmed only when "Date confirmed by" is filled; a scheduled change without it is treated as planned with no date. Any other date in the record (in "What it does not do", in a note) is never used in a draft and goes under Questions, unless it sits under "Do not mention", which already keeps it out. List under Questions anything the record leaves contradictory, such as a point that appears under both lists.
2. **Check the exports.** Compare the headers with the defaults and stop on a mismatch, as in Inputs. Count the rows, and count the rows linked to the Item ID.
3. **Select the requests.** A request is in the run when its `linked_item` equals the Item ID. A linked request on an account whose `account_owner` is not the account owner in the settings is counted under Other owners' accounts by owner, and goes no further; a blank owner is counted as "owner not stated". Rows on the account owner's accounts with a blank `linked_item` whose `request_text` contains a search word go under Possible matches, with the word found; they get no status and no draft, because linking a request is the account owner's call. If no row is linked to the Item ID, stop and ask whether the Item ID is right.
4. **Group by requester.** One requester is one `account` and `requester_name` together, compared without regard to case. Rows with the same `request_id` count once. The "on [account owner]'s accounts" count in the header is of linked requests only. Several requests from one requester are merged into one line and one draft, listing every request ID and date; the header counts the requests merged. Two different requesters at the same account each get their own line, marked "same account" with the other name, so the account owner can choose to combine them. List requesters by the date of their earliest linked request, oldest first; a possible match never affects the order.
5. **Set each requester's status.** Read what the request asks for against the record and choose one:
   - **Delivered:** the decision is shipped and every part of the request is covered by a "What it does" point.
   - **Partly delivered:** the decision is shipped; some parts are covered by "What it does" and the rest by "What it does not do" points. Name each open part with its status. This includes a request for something that is delivered in a different form from the one asked for, such as an export that exists when the request was for it to be sent on a schedule that is open: the delivered part counts as covered.
   - **Not in this change:** the decision is shipped, no part of what was asked for is covered by any "What it does" point, and a "What it does not do" point covers it. Give that point's status.
   - **Coming on [date]:** the decision is scheduled with a confirmed date.
   - **Planned, no date set:** the decision is scheduled and the date is not confirmed.
   - **Not going ahead:** the decision is not going ahead.
   - **Status unclear:** the request asks for something neither list covers, or "Available to" names a limit and the requester's `plan` is blank or does not show whether they qualify. The requester is held, with a question for the account owner to take to the responsible team.

   Write the basis beside each status: the numbered points it rests on, plus every "What it does" point the requester's draft names. A status is a proposed match; the account owner confirms it.
6. **Hold the requests that should not get a routine update.** Each goes to one held list, with its status still shown, in this order of precedence:
   - **Account owner first:** the request text mentions cancelling, leaving, looking at other suppliers or tools, a refund, a complaint or a dispute. A renewal alone is not one; the account owner may add it among the words to customize. The account owner talks to the customer before any update.
   - **Not to be contacted:** `do_not_contact` is yes or `preferred_channel` is none.
   - **Requester to confirm:** `requester_name` is blank, a team or shared mailbox rather than a person, or not found in the contact preferences.
   - **Status unclear:** from step 5.
7. **Choose the channel.** Use `preferred_channel`. If it is blank, use `channel_received` and mark "channel assumed". For an account meeting, take the meeting date from `notes` if it is there; otherwise write "next meeting, date not supplied". Copy any timing note for calls from `notes`.
8. **Draft one update per requester not held.** Number the drafts D1, D2 in the order of the requester list. Each draft:
   1. Opens with what this person asked for, in plain words close to their own, and the month they asked. With merged requests, it says they asked more than once.
   2. States the status plainly and consistently with their requester line; open parts use the exact status words in item 4.
   3. In the words the customer reads or hears, names only features in "What it does" and uses only two kinds of date: the "Available from" date of a shipped change or a confirmed scheduled one, and the months the person's own requests were received. A day or time the person asked for may be repeated as part of their request, never as a commitment.
   4. Gives each open part the exact status words: "under review, no date set", "planned, no date set" or "not going ahead", with the "Reason we can share" if one is supplied and no reason at all if not. "No date set" here means the record gives no confirmed date; the record's status of "under review" or "planned, no date" carries none. A reason or workaround is quoted without any word that suggests timing, even when the record's own wording has one ("for now", "at the moment", "yet"): drop that word and keep the rest.
   5. Never uses words that suggest timing for anything open, such as "soon", "shortly", "in the coming weeks", "next release", "on the way", "we expect", "we will add", "for now", "yet", "at the moment" or "in the meantime". This holds for the open part, the workaround and the closing question.
   6. Never mentions other customers, how many people asked, anything under "Do not mention", or "What it does not do" points the person did not ask about.
   7. Offers the workaround only if the record supplies one, names the open part it answers, and the person has that open part; if the record does not say which part it answers, offers nothing and puts the question under Questions. Offers the guide whenever one is supplied. Adds no detail about who may use the workaround beyond the record's words.
   8. Follows the channel: an email has a subject line and a body of 150 words at most, greeting and sign-off included, subject line not counted; an in-app message has a body of 60 words at most, greeting and sign-off included, and no subject; a phone call has three to six talking points and a "Not to say" line; an account meeting has an agenda line, three to six talking points and a "Not to say" line. "Not to say" lists any date or detail the conversation must avoid for this person's open parts and any "Do not mention" item that touches their request, or "nothing beyond the promise check".
   9. Ends an email or message with an invitation to reply, and is signed by the account owner unless the style notes say otherwise. A spoken draft may end with one question to the customer about fit.
   10. Ends with a promise check: every date in the draft with the field or request it came from, and every feature named with its "What it does" point. A meeting date taken from `notes` for the Meeting line is not a date the draft tells the customer, so it is not listed unless the draft's own words state it.
9. **List what a person does after sending.** For each draft, the request IDs to mark as updated in the feedback tool once the update has gone. The assistant changes no record.
10. **Return the draft** to the account owner. They check each status with the responsible team where the record left a question, edit and approve each update, and send it or hand it to the person who will.

## Exceptions and stop conditions

- **No change record, or no "Status confirmed by":** stop; list the fields the responsible team must fill. Draft nothing.
- **A header in either export missing or named differently:** stop; show the expected and found headers and ask which column holds each.
- **No contact preferences export:** stop and ask for it.
- **No request linked to the Item ID:** stop and ask whether the Item ID is right.
- **A future date without "Date confirmed by":** treat the change as planned with no date; put the date under Questions; never use it.
- **The record gives the same point under both lists:** status unclear for every requester it touches; put it under Questions.
- **A request text includes card details, a password, a login code or other personal data beyond the requester's name and role:** do not repeat it; refer to the request by its ID and tell the person to remove it from the source.
- **Asked to promise a date or a feature the record does not confirm, or to add a reason the team has not approved:** decline; put the question for the responsible team under Questions.
- **Asked to send, post, schedule a call, mark a request as updated or close it:** decline and name the account owner as the person who does it.

## Output format

```
FEEDBACK FOLLOW-THROUGH UPDATES: [Change] ([Item ID])

For: [account owner, role]. Prepared [date] from: change record confirmed by [role] on [date]; feedback export ([n] rows; [n] linked to [Item ID]; [n] of those on [account owner]'s accounts); contact preferences ([n] rows).

STATUS TO VERIFY WITH [responsible team role]
Decision: [shipped / scheduled / not going ahead]. Available from: [date / not confirmed]. Available to: [...].
What it does: [numbered points].
What it does not do: [numbered points, each with its status / none].
Reason we can share: [... / none supplied]. Workaround we can share: [... / none supplied]. Guide: [... / none supplied].
Questions before anything is sent: [numbered questions / none].

REQUESTERS: [n] requesters at [n] accounts, from [n] linked requests ([n] merged as repeat requests)
[n]. [Requester], [role / role not stated], [Account]. Requests [IDs], received [dates], via [channel]. [Same account: name.] Asked for: [plain summary]. Status: [status, with each open part and its status]. Basis: [numbered points]. Update by: [channel][, channel assumed][, timing note / meeting date] / none while held. Draft: [D(n) / held: list name].

DRAFT UPDATES (for [account owner] to edit and approve)
D[n]. To: [Requester], [Account]. Channel: [...].
[email] Subject: [...]  Body: [...]
[in-app message] Body: [...]
[phone call] Call: [timing note / no timing note]. Talking points: [3 to 6]. Not to say: [...].
[account meeting] Meeting: [date / next meeting, date not supplied]. Agenda line: [...]. Talking points: [3 to 6]. Not to say: [...].
Promise check: dates [each with its source / none]; features [each with its point / none].
[No drafts: every requester is held.]

HELD, NO DRAFT
Account owner first: [request IDs, requester, account, reason, status / none]
Not to be contacted: [request IDs, requester, account, reason, status / none]
Requester to confirm: [request IDs, requester, account, reason, status / none]
Status unclear: [request IDs, requester, account, question / none]

POSSIBLE MATCHES NOT INCLUDED
[Request ID, account, requester, received date: summary; search word found. Account owner decides whether to link it.] / none

OTHER OWNERS' ACCOUNTS
[Owner / owner not stated]: [n] requesters ([request IDs]) / none

AFTER SENDING (for a person to do in the feedback tool)
[D(n)]: mark [request IDs] as updated once sent. / nothing to mark

Drafts for [account owner]'s approval. Nothing has been sent and no record has been changed.

If stopped:
STOPPED: [reason]. Needed: [fields, headers or files]. Nothing has been drafted.
```

## Reviewer checklist

1. The change record names who confirmed it and when, and every question it leaves open is listed. (Account owner)
2. Every request linked to the Item ID on the account owner's accounts appears once, merged with its requester's other requests. (Account owner)
3. Each status matches the record, and its basis names the right points. (Account owner, with the responsible team where a question was raised)
4. No draft contains a date or a feature the promise check does not trace to the record or to the person's own request. (Account owner)
5. No draft mentions another customer, how many asked, or anything under "Do not mention". (Account owner)
6. Nobody marked do-not-contact has a draft, and every request tied to cancelling or a dispute is held for the account owner. (Account owner)
7. Each draft follows the person's preferred channel and its length limit. (Account owner)
8. Possible matches have been linked or dismissed in the feedback tool by a person. (Account owner)
9. Each update has been approved before it is sent, and its requests are marked as updated afterwards. (Account owner)

## Acceptance tests

Proposed tests. None has been run.

1. **Delivered, one request.** A shipped change covers everything one customer asked for; preferred channel email. Expected: status Delivered; one email of 150 words at most naming only "What it does" points; promise check lists the live date and the request month.
2. **Repeat requests.** The same person asked twice, linked to the same item. Expected: one requester line with both IDs, one draft saying they asked more than once, and the header counting one merged request.
3. **Partly delivered.** The request asks for the change plus something under "What it does not do" with status planned, no date. Expected: Partly delivered; the open part says "planned, no date set"; no date or timing word for it.
4. **Internal target in the record.** "Do not mention" holds an internal target quarter. Expected: it appears in no draft and is named on the "Not to say" line of any spoken draft for that request.
5. **Scheduled without confirmation.** Decision scheduled, "Available from" 1 March, "Date confirmed by" blank. Expected: every requester shows "Planned, no date set"; 1 March appears only under Questions.
6. **Do not contact.** The requester's `do_not_contact` is yes. Expected: held under Not to be contacted with the status; no draft.
7. **Tied to cancelling.** The request says the customer will look at other tools if the change is not done before renewal. Expected: held under Account owner first; no draft.
8. **Team name as requester.** `requester_name` is "Accounts team" and not in contact preferences. Expected: held under Requester to confirm.
9. **Header mismatch.** The feedback export has `customer` instead of `account`. Expected: stops, shows expected and found headers, asks which column holds the account; drafts nothing.
10. **Limited availability.** "Available to" is one plan and the requester's `plan` is blank. Expected: held under Status unclear with a question.
11. **Unlinked request with a search word.** Expected: listed under Possible matches with the word found; no status, no draft.
12. **Asked to send or promise.** "Send these now" or "tell them it's coming next month". Expected: declines; names the account owner as sender; the date question goes under Questions.
13. **Timing word in the record.** The workaround reads "For now, anyone with access to Reports can run the export by hand." Expected: drafts offer the workaround as "anyone with access to Reports can run the export by hand", with no "for now", and no draft uses "yet".

## Instructions for the AI assistant

```
You prepare an account owner's follow-through on customer feedback after
a change ships or a decision is made: who asked, what each asked for, the
confirmed status of their request, and one individual draft update per
person in the channel they prefer. You prepare; people decide. You never
send a message, call anyone, change or close a feedback record, or promise
a date or feature the responsible team has not confirmed. You never ask
for a password or a login code and need no access to any system.

The user supplies: the change record (Change, Item ID, Decision, Available
from, Date confirmed by, Available to, What it does, What it does not do
with a status per point, Reason we can share, Workaround we can share with the point numbers it answers,
Guide, Search words, Do not mention, Status confirmed by); the feedback
export (request_id, received_date, account, requester_name,
requester_role, channel_received, request_text, linked_item, plan,
account_owner); the contact preferences export (account, requester_name,
preferred_channel, do_not_contact, notes); the run settings (account
owner, today's date, responsible team role); optional style notes.

Stop, draft nothing, and print the STOPPED line if: the change record or
its "Status confirmed by" is missing; a required header in either export
is missing or named differently (show expected and found headers and ask
which column holds each; account_owner is always required; plan is
required only when "Available to" names a limit; notes is optional); the contact preferences export is missing;
the account owner is not named; or no row is linked to the Item ID.

1. A future date counts only if "Date confirmed by" is filled; otherwise
   treat a scheduled change as planned, no date set. Any other date in
   the record goes under Questions and is never used, unless it is under
   "Do not mention". List contradictions under Questions; a point under
   both lists makes the status unclear for every requester it touches.
2. Select rows whose linked_item equals the Item ID. Linked rows on
   another owner's accounts: count them by owner under OTHER OWNERS'
   ACCOUNTS ("owner not stated" if blank) and go no further. Rows on the
   account owner's accounts with a blank linked_item whose request_text
   contains a search word (default: the words of the change's name):
   list under POSSIBLE MATCHES with the word found; no status, no draft;
   they never affect the order. The header count "of those on the account
   owner's accounts" is of linked rows only.
3. One requester = account + requester_name, ignoring case. Count a
   repeated request_id once. Merge one requester's requests into one
   line and one draft. Mark different requesters at one account "same
   account" with the other name. List requesters by their earliest
   linked request, oldest first.
4. Status per requester, with its basis (the numbered points it rests on
   plus every "What it does" point its draft names):
   Delivered (shipped; every part covered by "What it does"); Partly
   delivered (some parts covered, the rest under "What it does not do",
   each open part with its status; this includes a delivered thing in a
   different form from the one asked for, such as an export when a
   scheduled export was asked for); Not in this change (no part of the
   request covered by "What it does", a "does not do" point covers it); Coming on [date] (scheduled,
   confirmed date); Planned, no date set; Not going ahead; Status
   unclear (neither list covers it, or "Available to" is limited and
   plan does not show the requester qualifies).
5. Hold, with the status still shown, first match wins: Account owner
   first (text mentions cancelling, leaving, other suppliers or tools, a
   refund, a complaint or a dispute; a renewal alone is not one); Not to be contacted (do_not_contact
   yes or preferred_channel none); Requester to confirm (blank name, a
   team or shared mailbox, or not in contact preferences); Status
   unclear.
6. Channel: preferred_channel, else channel_received marked "channel
   assumed". Account meeting date and call timing come from notes.
7. Draft D1, D2... in requester order, one per requester not held. Open
   with what they asked and the month; state the status plainly and
   consistently with their line. In the words the customer reads or
   hears, name only "What it does" features and use only the live or
   confirmed date and the months of their own requests; a day or time
   they asked for may be repeated as their request, never as a
   commitment. Give open parts as "under review, no date set", "planned, no date set" or
   "not going ahead" plus the shareable reason if any ("no date set"
   means the record gives no confirmed date). Never write "soon",
   "shortly", "in the coming weeks", "next release", "on the way", "we
   expect", "we will add", "for now", "yet", "at the moment", "in the
   meantime" or any other timing word for an open part, a workaround, a
   reason or a closing question. Quote a workaround or reason without its
   timing words even if the record's own wording has them. Never mention other customers, how many asked, "Do not mention"
   items, or "does not do" points they did not ask about. Offer the
   workaround only for the open part the record says it answers, in the
   record's words with nothing added about who may use it; if the record
   does not say, offer nothing and ask under Questions. Give the guide if
   supplied. Email: subject and body of 150 words at most, greeting and
   sign-off counted. In-app message: 60 words at most, greeting and
   sign-off counted, no subject. Phone call: 3 to 6 talking
   points and a "Not to say" line. Account meeting: agenda line, 3 to 6
   talking points, "Not to say" line. The "Not to say" line lists any
   date or detail to avoid for this person's open parts and any "Do not
   mention" item that touches their request, or "nothing beyond the
   promise check". If the notes give no meeting date, write "next
   meeting, date not supplied". End an email or message with an
   invitation to reply; a spoken draft may end with one question about
   fit. Sign as the account owner. End each draft with the promise
   check: every date with its source, every feature with its point. A
   meeting date taken from notes for the Meeting line is not listed
   unless the draft's own words state it.
8. List, per draft, the request IDs a person marks as updated after
   sending.
9. Use the output format exactly, with "none" in any empty list, and end
   with: "Drafts for [account owner]'s approval. Nothing has been sent and
   no record has been changed."

Do not repeat card details, passwords, login codes or other personal
data found in request text; refer to the request ID and tell the user to
remove it. If asked to promise a date or feature the record does not
confirm, or to add a reason the team has not approved, decline and put
the question under Questions. If asked to send, post, schedule, mark or
close anything, decline and name the account owner as the person who
does it.
```

## What to customize

- Your column headers, if your feedback tool or contact list uses other names, and the values your tool uses for channels and do-not-contact.
- The change record fields: who on the responsible team confirms them, and where the record is kept.
- The status words, if your company already uses others with customers.
- The words that send a request to Account owner first, such as your own terms for complaints or escalations.
- Channel lengths, sign-off and tone, in your style notes.
- Whether a run covers one account owner or a team lead's whole book, with drafts grouped by owner.
- Whether two requesters at one account get one combined update by default.
- Which exports the assistant may read in ChatGPT, Claude, Copilot or Gemini.

## Version notes

- 0.1.0, 10 November 2026. Written by Fully Powered AI from its own published map of the work. Editorially reviewed. Tried on its invented example in Claude on 10 November 2026 in two runs: the instructions were revised after the first, following review, and the second, made by the model that made those revisions, is the run recorded and published with it. Not run again after any later edits. Not yet tested in a client environment, and not yet tested as a packaged version in ChatGPT, Claude, Copilot or Gemini.
