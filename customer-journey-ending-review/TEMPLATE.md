# Customer journey ending review

Workflow template, version 0.1.0.

## Purpose

Review how one customer's journey ended, from the records the team supplies: whether the final handoff came after the work was actually done, the difficult moments along the way with the evidence and the days involved, what the customer said in their own words, readings of what the customer may have experienced (kept as readings to confirm), and follow-up options in three kinds: for this customer, changes to test in the journey for future customers, and changes to the records. The journey is one offboarding, one cancellation, one project close, one delivery or one onboarding milestone. The customer experience owner reads it, and the customer success lead chooses which change to test. The assistant prepares; it never contacts the customer, sends or promises anything, offers money, judges a member of staff or changes a record.

## When to use it and when not to

Use it when one customer's journey has reached its last planned handoff and something about the ending needs a closer look: a low close survey score, an unhappy exit comment, a complaint in the final weeks, a handoff that slipped, or a routine look at a sample of recent endings. Run it once per journey, after the final handoff, with the records of that journey.

Do not use it:

- to answer a customer who is asking to cancel today. Responding to a live request is Cancellation request response;
- to find why customers leave across a quarter. The pattern across many leavers is Churn risk and save plan; this review reads one journey closely;
- to check that a deliverable is ready before it is handed over. That is Project handover readiness check, run before the handoff; this review runs after it;
- to review a project's scope, schedule and budget. That is Project lessons review; this review follows the customer's side of the journey;
- to write the apology, the reply or an offer to the customer. A person writes and sends those, with Customer reply drafting if they want help;
- to assess a member of staff. The review names roles and describes what the records show; it rates no one.

## Roles

- **Runs it and reads it first:** the customer experience owner, such as the customer experience lead or a customer success manager, for the journey under review.
- **Chooses which change to test, and with which customers:** the customer success lead, or the role named under "Decision by" in the brief.
- **Finishes any work still open:** the owner named against each completion criterion.
- **Replies to the customer, if anyone does:** the person the customer success lead names. Always a person, after approval.
- **Refers anything about a refund, a chargeback or a legal claim:** the account owner, to whoever handles those in the organization.

## Inputs

1. **The review brief,** typed notes with these fields:
   - **Customer:** the customer's name or code.
   - **Journey type:** offboarding, cancellation, project close, delivery or onboarding milestone.
   - **Journey start:** the date the journey began.
   - **Final handoff:** the `event_id` in the journey log of the last planned handoff to the customer, such as the closing call, the data export, the delivery or the last training session.
   - **Review date:** today's date.
   - **Review owner:** name and role.
   - **Decision by:** the role that chooses which change to test. Default: customer success lead.
   - **Reason for review:** one line.
   - **Contact limits:** anything that rules out contact, such as a request not to be contacted or a matter handled by someone else. "None" if none.
   - **Settings,** each with a default used when blank: reply target, 2 days; silence limit, 10 days; low score, 6 or below on a 0 to 10 scale and 2 or below on a 1 to 5 scale; journeys to measure a change on, the next 5 of the same type.

   If Customer, Journey start, Final handoff or Review date is missing, stop and ask. Write which defaults were used in the header.
2. **The completion criteria,** what "done" meant for this journey, one row per criterion. Default column headers: `criterion_id`, `criterion`, `status_at_end` (met, partly met, not met or not recorded), `evidence_event` (the `event_id` of the item that shows it, may be blank), `owner`. If the file is missing, stop: without it the review cannot tell finished work from a finished-sounding message.
3. **The journey log,** one row per item between the team and the customer, plus internal notes, exported from the CRM, help desk, project tool or inbox. Default column headers: `event_id`, `date`, `thread`, `stage`, `channel`, `direction` (from customer, to customer or internal), `owner` (the role on the team who owns the item; for an item from the customer, the role it was sent to), `summary`, `criterion` (a `criterion_id` the item concerns, may be blank), `due_date` (a date the team promised in this item, may be blank), `fulfils` (the `event_id` of the promise this item delivers, may be blank). If the log is missing, stop.
4. **The customer feedback,** one row per comment, score or note about this journey. Default column headers: `feedback_id`, `date`, `source` (survey, email, review, chat or call note), `person`, `score` (may be blank), `scale` (0 to 10 or 1 to 5, blank when there is no score), `refers_to` (an `event_id` or a stage, may be blank), `text`. If there is no feedback at all, write "no feedback supplied" and continue.

For every file: headers match without regard to case and extra columns are ignored. If any default header is missing or named differently, stop, show the expected and the found headers, and ask which column holds each. Blank cells are allowed only where the list above says so, except a blank `owner`, which the review lists as a records gap. Dates are read as written; if a date cannot be read, stop and name the row.

The assistant works from the files the person supplies. It needs no connection to any system and never asks for a password or a login code.

## The procedure

1. **Check the inputs.** Check the headers, as in Inputs. Stop if two rows in one file share an id. Confirm the final handoff `event_id` is in the log; if not, stop and ask. Count the log rows, the rows dated from the journey start to the final handoff date (the window), the rows dated after it ("after the end") and any dated before the start, which are left out and counted. If the log has no item from the customer and there is no feedback, stop: the review cannot see the customer's side.
2. **Settle each criterion.** Using the final handoff date:
   - **Met by the handoff:** `status_at_end` is met and the evidence event is in the log, dated on or before the handoff.
   - **Met after the handoff:** met, with the evidence event dated after the handoff. Open at the handoff; closed since.
   - **Met, evidence not found:** met, with the evidence event blank or not in the log. Treat it as open at the handoff and on the review date.
   - **Partly met, not met, not recorded:** open at the handoff and on the review date. Show the evidence event and its summary if one is given.
3. **Pair every item from the customer with its answer.** The answer is the first later item to the customer on the same thread; an item on the same date counts when it comes later in the log. Internal items never count as an answer or as contact.
4. **Find the difficult moments.** Record each finding below with its event ids and its dates:
   1. **Slow reply:** an item from the customer answered after more than the reply target. Give the days taken and the days over the target.
   2. **Unanswered:** an item from the customer with no answer by the review date. Give the days it has been open on the review date.
   3. **Asked again:** a second or later item from the customer on a thread with no item to the customer in between.
   4. **Missed date:** a row with a `due_date` whose fulfilling row (the row whose `fulfils` names it) is dated after the due date; give the days late. With no fulfilling row by the review date, write "not delivered in the records" and the days overdue on the review date. A row that names the promise in `fulfils` counts as delivering it, even when the criterion it concerns is still open (a partial fix); the open criterion shows separately, under the moment.
   5. **Silence:** inside the window, more than the silence limit in days between one item to the customer and the next. A silence belongs to no thread.

   Count days as calendar days, by subtracting one date from the other.
5. **Group findings into moments.** Two findings belong to the same moment when they share an event id or a thread, or when one is a silence and the other has an event dated inside it, the silence's two ends included. Keep joining until no two moments share anything; a silence with no finding inside it is a moment of its own. A moment's events are the events named in its findings, not every log row inside its dates. Number the moments M1, M2 in date order of their earliest event. For each moment, note:
   - the stages it spans;
   - **open criterion:** any event in it carries a criterion still open on the review date;
   - **named in feedback:** a feedback item's `refers_to` names one of its events or, when it names a stage, the moment lies wholly in that stage (a moment that spans two stages can be named only through one of its events);
   - **proposed link:** a feedback item with a blank `refers_to` whose text names the same thing as a summary in the moment. Quote the shared words; words that only share a stem (such as "train" and "trained") are not shared words. A feedback item may have proposed links to several moments. A proposed link is for the review owner to confirm and never counts in step 7;
   - **after the end:** any event in it is dated after the final handoff.
6. **Read how it ended.**
   - Show the final handoff item: date, channel, owner and summary.
   - **Ending:** "Ended complete" when every criterion was met by the handoff and no item from the customer dated on or before the handoff was still unanswered at the end of the handoff date (an answer later the same day counts as an answer). Otherwise "Ended with work open", "Ended with a question unanswered", or "Ended with work open and a question unanswered". When every criterion is "not recorded", write "Cannot tell from the records whether the work was finished" in place of the work part.
   - **Closing words against open work:** the handoff item, and any item to the customer dated on the handoff date or later, whose summary calls the work complete, closed, finished or done while a criterion was open at the handoff. A warm or polished closing message never changes the ending.
   - **Low scores:** each feedback score at or below the low score for its scale.
   - **After the end:** every item dated after the handoff, with whether an item from the customer has been answered.
7. **Choose up to three moments to look at first.** Place each moment by the first of these that applies to it: (a) it has an open criterion; (b) it is named in feedback; (c) it holds an unanswered item; (d) it holds a slow reply or a missed date, the most days over target or late first; (e) it is a silence alone, the longest first. Within one rule, the moment nearer to the final handoff comes first, because the review is about the ending. State the rule that placed each.
8. **Quote the customer.** List every feedback item in date order, with its id, date, source, person and score. Quote the text exactly. A call note is the note-taker's words, not the customer's: label it "the note-taker's words" and never put it in quotation marks as the customer's speech. Show the link: the `refers_to` value, the proposed link with its shared words, or "not linked".
9. **Write the readings, to confirm.** One reading for each moment to look at first. Start with "The records are consistent with" and say what the customer may have experienced, citing the event and feedback ids it rests on. Never state a feeling as fact: words such as frustrated, angry, upset or let down appear only inside the customer's own quoted words. End each reading with what would confirm or rule it out: a question a person could ask the customer, or a record to check.
10. **List the follow-up options,** numbered O1, O2 across all three kinds, in this order:
    - **For this customer:** one option to finish each criterion still open on the review date, owned by the criterion's owner ("owner not stated" if blank); then one option per thread with unanswered items, for a person to reply, owned by the owner of the latest unanswered item. If the contact limits rule out contact, write each reply option as "Not offered" with the limit. Never propose money, a credit, a refund, a discount or a gift.
    - **Changes to test in the journey:** one change for each moment to look at first, and one more for the ending when it was not "Ended complete". Each change is one sentence, at one stage, aimed at what the records show happened and never at a person. Give how you would know: a count taken from the same kind of record over the next journeys of this type (the number in the settings). Owner if chosen: "owner to choose", unless the brief names a stage owner. Mark each "proposed, untested".
    - **For the records:** one option for each gap the review met: a criterion "not recorded" or "met, evidence not found", feedback with a blank `refers_to`, a blank `owner`, or a whole column left blank.
    Write "none" under a kind with no option.
11. **Write the decisions** for the role under "Decision by": which change, if any, to test, and with which journeys; for each criterion still open, who finishes it and whether the customer is told; for each thread with unanswered items, whether a person replies now and who; for each loss the customer names in feedback (a booking, a sale, time, money), whether and how to acknowledge it, with no amount proposed; whether to adopt the records options; and each referral under the exceptions. Write "none" for any that does not arise. Recommend nothing.
12. **Return the review** to the review owner, for the role under "Decision by". Nothing goes to the customer from the review.

## Exceptions and stop conditions

- **Brief fields missing, the completion criteria or the log missing, a header that does not match, two rows with one id, a date that cannot be read, or the final handoff not in the log:** stop; print the STOPPED line with what is needed. Draft nothing.
- **No item from the customer and no feedback:** stop and ask whether more records exist.
- **The records mention a refund, a chargeback, a complaint handled formally, or a legal claim or threat:** continue the review, but offer no option for this customer that touches the matter; list it under the decisions as a referral to the account owner. Say nothing about who is right.
- **Asked who was at fault, to rate a member of staff, or to judge someone's performance:** decline. The review names roles and what the records show, and suggests changes to the journey only.
- **Asked to write the reply, the apology or an offer, or to send, post or schedule anything:** decline and name the person who does it.
- **Asked to state how the customer felt, or whether they will come back:** decline to state it as fact; give the reading with what would confirm it.
- **The records hold card details, a password, a login code, health details or a home address:** do not repeat them; refer to the row by its id and tell the person to remove it from the source.
- **A whole optional column is blank** (`criterion`, `due_date`, `fulfils` or `refers_to`): run every other rule, list the rule that could not run under "Not checked", and add a records option.

## Output format

```
JOURNEY ENDING REVIEW: [Customer], [journey type]

For: [review owner, role]. Decision by: [role]. Prepared [review date] from: brief; completion criteria ([n]); journey log ([n] rows: [n] in the window, [n] after the end, [n] before the start, left out); feedback ([n] items / no feedback supplied).
Reason for review: [as given]. Settings: reply target [n] days; silence limit [n] days; low score [cut-offs]; changes measured on the next [n] journeys. [Defaults used: ... / No defaults used.] Contact limits: [as given / none].

HOW IT ENDED
Final handoff: [event id], [date], [channel], [owner]: [summary].
Ending: [Ended complete / Ended with work open / Ended with a question unanswered / Ended with work open and a question unanswered / Cannot tell from the records whether the work was finished[, and a question unanswered]].
Criteria: [n] met by the handoff; [n] open at the handoff; [n] still open on [review date].
[criterion id] [criterion]: [met by the handoff, [event] on [date] / met after the handoff, [event] on [date] / met, evidence not found / partly met, [event] on [date]: [summary] / not met / not recorded]. Owner: [role / owner not stated].
Questions unanswered at the handoff: [event ids, with dates / none].
Closing words against open work: [event id, date: summary, while [criterion ids] were open / none].
Low scores: [feedback id, score on scale, cut-off / none].
After the end: [event id, date, direction: summary[, answered by [id] / unanswered]] / none.

DIFFICULT MOMENTS ([n]), in date order
M[n]. [first date] to [last date], [stages]. [Each finding: kind, event ids, dates, days.] Open criterion: [criterion ids / none]. Named in feedback: [feedback ids / none]. Proposed link: [feedback id, "shared words" / none]. [After the end: event ids.]
[No difficult moments found in the records.]

MOMENTS TO LOOK AT FIRST
[n]. M[n], placed by rule [(a) to (e)]: [the reason in a few words].
[none]

IN THE CUSTOMER'S WORDS
[feedback id], [date], [source], [person][, score n on scale]: "[text exactly]" / [call note], the note-taker's words: [text]. Link: [refers_to value / proposed links to M[n], "shared words"; M[n], "shared words" / not linked].
[No feedback supplied.]

READINGS, TO CONFIRM
[n]. M[n]: The records are consistent with [reading]. Rests on: [ids]. To confirm: [question to ask or record to check].
[none]

FOLLOW-UP OPTIONS (for [Decision by role] to choose; none is recommended)
For this customer:
O[n]. [Finish [criterion id]: what remains] / [Reply on [thread] to [event ids]: what the reply would need to cover]. Rests on: [ids]. Owner if chosen: [role / owner not stated]. [Not offered: [contact limit].]
[none]
Changes to test in the journey (proposed, untested):
O[n]. At [stage]: [the change]. Rests on: [M ids / the ending]. How you would know: [the count, from which record, over the next [n] journeys of this type]. Owner if chosen: [owner to choose / named stage owner].
[none]
For the records:
O[n]. [The gap, and the record change that would close it]. Rests on: [ids].
[none]

NOT CHECKED
[Rule that could not run, and why / nothing]

DECISIONS FOR [Decision by role]
1. Which change, if any, to test, and with which journeys: [O ids / none proposed].
2. Work still open: [for each criterion id, who finishes it and whether the customer is told / none].
3. Unanswered items: [for each thread, whether a person replies now, and who / none].
4. Losses the customer names: [feedback id and the loss, whether and how to acknowledge it; no amount is proposed / none].
5. Records changes: [O ids, whether to adopt / none].
6. Referrals: [item, to the account owner / none].

Review for [review owner] and [Decision by role]. Nothing has been sent, no customer has been contacted and no record has been changed.

If stopped:
STOPPED: [reason]. Needed: [fields, headers, rows or files]. Nothing has been drafted.
```

## Reviewer checklist

1. Every criterion's line matches the criteria file and the date of its evidence event. (Review owner)
2. The ending follows the rule: no journey is called complete while a criterion was open or a question unanswered at the handoff, whatever the closing message said. (Review owner)
3. Every reply time, delay and silence is recomputed from the log dates and is right. (Review owner)
4. Every finding is grouped into exactly one moment, and the moments to look at first follow rules (a) to (e). (Review owner)
5. Only the customer's written words appear in quotation marks; call notes are labelled as the note-taker's. (Review owner)
6. No reading states a feeling as fact, and each says how it would be confirmed. (Customer success lead)
7. No option names a person as the cause, and none proposes money, a credit, a refund, a discount or a gift. (Customer success lead)
8. Each change to test is at one stage and has a count that would show whether it helped. (Customer success lead)
9. Any contact with the customer is approved and made by a person, after the decisions. (Customer success lead)

## Acceptance tests

Proposed tests. None has been run.

1. **Clean ending.** Every criterion met with evidence before the handoff, every customer item answered within the target, a close score of 9 out of 10. Expected: "Ended complete"; no difficult moments; no options for this customer; no change for the ending.
2. **Warm close, open work.** The handoff item says the project is complete while one criterion is partly met. Expected: "Ended with work open"; the item listed under "Closing words against open work"; an option to finish the criterion; a change for the ending.
3. **Evidence after the handoff.** A criterion is marked met, with its evidence event three days after the handoff. Expected: "met after the handoff", counted as open at the handoff and not still open on the review date.
4. **Asked again during a silence.** The customer writes twice on one thread across a 15-day gap in messages to them. Expected: one moment holding the slow reply, the asked-again finding and the silence.
5. **Silence at the limit.** Exactly 10 days between two items to the customer, with the default limit. Expected: no silence.
6. **Missed promise never delivered.** A due date with no fulfilling row. Expected: "not delivered in the records", with the days overdue on the review date.
7. **Call note.** A call note says the customer was unhappy. Expected: shown as "the note-taker's words", not quoted as the customer's words; "unhappy" does not appear in any reading except as the note's own text.
8. **Header mismatch.** The log has `customer_or_team` in place of `direction`. Expected: stops, shows expected and found headers, asks which column holds each.
9. **Final handoff not in the log.** Expected: stops and asks.
10. **No customer side.** A log with only items to the customer and internal notes, and no feedback. Expected: stops and asks whether more records exist.
11. **Refund in the feedback.** The exit comment asks for a refund. Expected: review completed; no option for this customer touches the refund; listed as a referral to the account owner; nothing said about who is right.
12. **Fault question.** "Which of our people dropped the ball?" Expected: declines; keeps to roles and records.
13. **Do not contact.** The contact limits say the customer asked not to be contacted. Expected: reply options shown as "Not offered" with the limit; options to finish work stay.
14. **Ranking tie.** Two moments each three days late, one near the start and one at the handoff. Expected: the one at the handoff placed first under rule (d).

## Instructions for the AI assistant

```
You review how one customer's journey ended (an offboarding, a
cancellation, a project close, a delivery or an onboarding milestone),
from the records the user supplies, for the customer experience owner.
You prepare; people decide. You never contact the customer, send, post
or promise anything, propose money, a credit, a refund, a discount or a
gift, judge or rate a member of staff, or change any record.
You never ask for a password or a login code, and you need no access
to any system.

The user supplies:
- The brief: Customer, Journey type, Journey start, Final handoff (an
  event_id), Review date, Review owner, Decision by (default customer
  success lead), Reason for review, Contact limits, and settings with
  defaults: reply target 2 days; silence limit 10 days; low score 6 or
  below on 0 to 10, 2 or below on 1 to 5; changes measured on the next
  5 journeys of the same type.
- Completion criteria: criterion_id, criterion, status_at_end (met,
  partly met, not met, not recorded), evidence_event, owner.
- Journey log: event_id, date, thread, stage, channel, direction (from
  customer, to customer, internal), owner, summary, criterion,
  due_date, fulfils.
- Feedback: feedback_id, date, source (survey, email, review, chat,
  call note), person, score, scale, refers_to, text.

Stop, draft nothing and print "STOPPED: [reason]. Needed: [...].
Nothing has been drafted." if: Customer, Journey start, Final handoff
or Review date is missing; the criteria file or the log is missing; any
default header is missing or named differently (show expected and found
headers and ask which column holds each; ignore case and extra
columns); a cell is blank outside the optional columns (evidence_event,
criterion, due_date, fulfils, score, scale, refers_to; a blank owner is
a records gap, not a stop); two rows in one file share an id; a date cannot be read; the
final handoff is not in the log; or the log has no item from the
customer and there is no feedback.

1. Count log rows: in the window (journey start to the final handoff
   date), after the end, and before the start (left out).
2. Criteria, against the handoff date: met by the handoff (met, evidence
   in the log on or before it); met after the handoff (open at the
   handoff, closed since); met, evidence not found (evidence blank or
   not in the log: open); partly met, not met, not recorded (open).
3. An item from the customer is answered by the first later item to the
   customer on the same thread (same date counts if later in the log).
   Internal items are never an answer or contact. Count calendar days.
4. Findings: slow reply (answered after more than the reply target;
   days and days over); unanswered (no answer by the review date; days
   open); asked again (a second item from the customer on a thread with
   no item to the customer between); missed date (the row that fulfils
   a due_date is later; days late; or "not delivered in the records"
   and days overdue; a row that names it in fulfils delivers it even if its
   criterion is still open); silence (inside the window, more than the silence
   limit between consecutive items to the customer; it has no thread).
5. Moments: two findings are in one moment if they share an event id
   or a thread, or if one is a silence and the other has an event dated
   inside it, ends included. Keep joining until nothing more joins; a
   silence with nothing inside stands alone. A moment's events are those
   named in its findings. Number M1, M2 by earliest event date.
   Note stages, open criterion (still open on the review date), named in
   feedback (refers_to names one of its events, or a stage it lies
   wholly in; a moment spanning two stages is named only through an event),
   proposed link (blank refers_to, text names the same thing as a summary
   in it; quote the shared words, a shared stem is not a shared word;
   several moments allowed; never used for ranking),
   and events after the end.
6. How it ended: show the final handoff item. Ending: "Ended complete"
   only if every criterion was met by the handoff and no customer item
   dated on or before it was unanswered at the end of the handoff date
   (a later answer the same day counts); otherwise
   "Ended with work open", "Ended with a question unanswered", or both.
   If every criterion is "not recorded", say the records cannot tell
   whether the work was finished. List closing words against open work:
   the handoff item and any later or same-day item to the customer whose
   summary calls the work complete, closed, finished or done while a
   criterion was open. A polished closing message never changes the
   ending. List low scores and every item after the end.
7. Up to three moments to look at first, placed by the first rule that
   applies: (a) open criterion; (b) named in feedback; (c) holds an
   unanswered item; (d) slow reply or missed date, most days over or
   late first; (e) silence alone, longest first. Within a rule, nearer
   to the final handoff first. State the rule.
8. List feedback in date order and quote its text exactly. A call note
   is the note-taker's words: label it "the note-taker's words" and
   never quote it as the customer's speech.
9. One reading per moment to look at first, starting "The records are
   consistent with", citing ids, ending with how to confirm it. Feelings
   (frustrated, angry, upset, let down) appear only inside the
   customer's own quoted words.
10. Options O1, O2...: for this customer, one per criterion still open
    (its owner) then one per thread with unanswered items (owner of the
    latest one), or "Not offered" with the contact limit; changes to
    test, one per moment to look at first plus one for the ending if it
    was not complete, each at one stage, aimed at what happened and
    never at a person, with a count over the next journeys and "owner
    to choose", marked "proposed, untested"; for the records, one per
    gap met (a criterion not recorded or met with evidence not found, a
    feedback item with a blank refers_to, a blank owner, or a whole
    column left blank). Write "none" under an empty kind.
11. Decisions for the Decision by role: which change to test; who
    finishes each open criterion and whether the customer is told;
    whether a person replies on each unanswered thread, and who; each
    loss the customer names, whether and how to acknowledge it, with no
    amount; whether to adopt records options; referrals. "none" where
    one does not arise. Recommend nothing.
12. Use the output format exactly. If a whole optional column
    (criterion, due_date, fulfils, refers_to) is blank, list the rule
    that could not run under NOT CHECKED, else write "nothing". End
    with: "Review for [review owner] and [Decision by role]. Nothing has
    been sent, no customer has been contacted and no record has been
    changed."

If the records mention a refund, a chargeback, a formal complaint or a
legal claim or threat, finish the review, offer no customer option that
touches it, and list it as a referral to the account owner, saying
nothing about who is right. If asked who was at fault or to rate a
person, decline and keep to roles and records. If asked to write or
send a reply, apology or offer, decline and name the person who does
it. If asked how the customer felt or whether they will return, give a
reading with how to confirm it, never a fact. Do not repeat card
details, passwords, login codes, health details or home addresses found
in the records; refer to the row id and tell the user to remove them.
Recheck every day count against the log before returning the review.
```

## What to customize

- Your column headers, if your CRM, help desk or project tool exports other names, and your words for `direction` and feedback `source`.
- The completion criteria for each journey type you run: offboarding, cancellation, project close, delivery or an onboarding milestone. Agree them before the journey starts, so the review has something firm to read the ending against.
- One thread per topic in your log. A single thread that runs the whole journey makes every finding one moment.
- The reply target, silence limit and low score, and whether you count calendar or working days.
- How many journeys a change is measured on before the customer success lead judges it.
- The words that mark closing language in your summaries, if your team writes "signed off" or "wrapped" rather than complete or closed.
- Who handles refunds, chargebacks and formal complaints, so referrals name the right role.
- Which exports the assistant may read in ChatGPT, Claude, Copilot or Gemini.

## Version notes

- 0.1.0, 11 November 2026. Written by Fully Powered AI from its own published map of the work. Editorially reviewed. Tried once on its invented example in Claude on 11 November 2026 (record in the public trial); afterwards the wording was clarified on the points the trial raised and the example was edited to drop one link and one unsupported phrase, and it was not run again. Not yet tested in a client environment, and not yet tested as a packaged version in ChatGPT, Claude, Copilot or Gemini.
