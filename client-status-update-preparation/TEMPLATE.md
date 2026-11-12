# Client-status update preparation

Workflow template 0.1.0. Written by Fully Powered AI.

## Purpose

Draft a client-status update from the matter or project notes, the task list and the last update sent, so the responsible person can review, edit and send an accurate update on schedule. Every update says what moved since last time, which dates are confirmed, which are estimates, what the client must decide and by when, and the next step. A reviewer note travels with the draft and shows every judgment left for the reviewer.

The draft is never sent by the AI assistant. An estimate never becomes a commitment in the draft.

## When to use it and when not to

Use it on the agreed update day for each client, and between updates when a date the client relies on moves or a new decision falls to the client.

Do not use it:

- to announce a change in fees, scope or staffing. Those messages belong to the responsible person, written by them;
- in a law firm, to explain legal options or the merits of a matter, or to work out a court, filing or limitation date. Advice and legal deadlines stay with the responsible attorney;
- to reply to a client complaint.

## Roles

- **Runs it:** the person who owns the client relationship (project manager, responsible attorney, account director or engagement lead), or a coordinator on their behalf.
- **Reviews, edits and sends:** the responsible person. No one else sends.
- **Decides:** the responsible person (what the client hears, whether an estimate is firm enough to share, whether an internal issue is mentioned).
- **Keeps the inputs current:** the team keeping the notes; the lead keeping the task list.

## Inputs

1. **Notes since the last update.** Meeting notes, call notes and internal comments. If there are none, the reviewer note asks for a progress summary.
2. **Task list or plan.** Each task with its date and status: confirmed (agreed with the client as the firm defines it), estimate, or at risk. If a date has no status, treat it as an estimate and flag it.
3. **Last update sent.** The message the client last received. If missing, draft without a "since last update" comparison and flag it.
4. **Update standard.** Length, greeting, sign-off, section order and what never goes in. If absent, use the output format below and flag that no standard was supplied.
5. **Client decisions log (optional).** Open decisions, who on the client side owns each, and the date requested.

## The procedure

1. **Set the baseline.** From the last update, list every date and promise the client was given.
2. **Compare.** For each baseline item, find its current state in the task list. Classify: delivered as promised; delivered late; still on track; moved; dropped. A moved or dropped item always appears in the draft and in the reviewer note.
3. **Classify every date.** Confirmed only if the task list marks it confirmed under the firm's definition. Everything else is an estimate. If the notes and the task list disagree on a date, write "[date to confirm]" in the draft and put both dates in the reviewer note.
4. **Find client decisions.** List each decision only the client can make, the options as the team describes them and the needed-by date, or "[needed-by date to confirm]". Never invent one.
5. **Name the consequence of each decision date** only when the notes state it (for example, "a choice by 13 November keeps the 11 December estimate").
6. **Sort internal content.** Leave out anything marked internal or under "what never goes in". If it bears on a client date or decision, list it under "Left out on purpose".
7. **Write the draft** in the order: progress since last update; confirmed dates; estimates, each labelled "Estimate"; decisions needed from the client with needed-by dates; next step. Keep to [N] words. Plain sentences, no adjectives about the team's performance.
8. **Write the reviewer note:** what changed, every date and its status with source, anything left out on purpose, and every placeholder left in the draft.
9. **Mark the draft** "DRAFT for [responsible person] to review and send".

## Exceptions and stop conditions

- **A confirmed date has passed without delivery.** Stop. Ask the responsible person how the client should hear it before drafting.
- **The notes record client dissatisfaction or a complaint.** Draft nothing about it; flag it at the top of the reviewer note for the responsible person.
- **Fees, scope or staffing changes appear in the notes.** Leave them out and flag them.
- **Law firms: the notes contain advice, strategy or privileged discussion.** Leave it out; flag it for the responsible attorney.
- **Law firms: a court, filing or limitation date.** Include it only as the task list records it, list it in the reviewer note for the responsible attorney to check, and never work one out.
- **Inputs belong to two different clients or projects.** Stop and ask the person who ran it.

## Output format

```
DRAFT for [responsible person] to review and send

Subject: [Project or matter identifier] status, week of [date]

Since our update on [date], [progress, one or two sentences].

Confirmed: [task] on [date]. [Who confirmed, if the standard asks.]

Estimate: [task] by [date]. [Dependency, if any.]

Your decision, needed by [date]: [decision and options as described].
[Consequence, only if stated in the notes.]

Next step: [what the team does next].

[Sign-off per update standard]

---
REVIEWER NOTE
Changed since [last update date]: [list].
Dates and their status: [date]: [confirmed | estimate | to confirm]
  ([source]).
Left out on purpose: [item]: [why it may matter to the client].
Placeholders in the draft: [list | none].
Flags: [stop conditions met | none].
Nothing has been sent.
```

## Reviewer checklist

- Every promise in the last update is accounted for in the draft.
- Each confirmed date carries confirmed status in the task list.
- Every estimate is labelled "Estimate".
- Every client decision has a needed-by date or a visible placeholder.
- No internal note, fee, staffing or advice content appears in the draft.
- The reviewer note lists every placeholder and every omission that touches a client date.
- The responsible person, and only that person, sends it.

## Acceptance tests

Proposed tests. None has been run.

1. **Quiet week.** Expected: short draft with progress and next step; reviewer note says "no changes".
2. **Confirmed, estimate and decision.** Project 7731: submission 20 November confirmed; drawings 11 December estimate; tank decision needed by 13 November. Expected: each on its own line, the estimate labelled, the decision with its date and stated consequence.
3. **Notes and task list disagree** (20 versus 27 November). Expected: "[date to confirm]" in the draft; both dates with sources in the note.
4. **Undated decision.** Expected: "[needed-by date to confirm]", listed under placeholders.
5. **Missed confirmed date.** Expected: stop and ask the responsible person; no draft.
6. **Internal resourcing note.** Expected: left out of the draft; listed under "Left out on purpose" with its link to the 11 December estimate.
7. **Missing last update.** Expected: no "since our update" line; flagged.
8. **Law firm notes with strategy discussion.** Expected: left out; flagged for the responsible attorney.

## Instructions for the AI assistant

```
You draft client-status updates for review by the responsible person.
You prepare; people decide. You never send a message, never present an
estimate as a commitment, never invent or calculate a date, and never
include advice, fees, staffing or internal notes in the draft.

Inputs: notes since the last update, the task list with date statuses,
the last update sent, the firm's update standard, and any client
decisions log.

1. List every date and promise in the last update. If there is no last
   update, omit the "since our update" line and flag it.
2. For each, find its current state in the task list: delivered as
   promised, delivered late, on track, moved or dropped. Moved and
   dropped items always appear in the draft and the reviewer note.
3. A date is "Confirmed" only if the task list marks it confirmed. All
   other dates are estimates and are labelled "Estimate". In a law firm,
   give a court, filing or limitation date only as the task list records
   it and list it for the responsible attorney to check. If notes and
   task list disagree on a date, write "[date to confirm]" in the draft
   and give both dates with sources in the reviewer note.
4. List each decision only the client can make, with options as the
   team describes them and the needed-by date. If none is recorded,
   write "[needed-by date to confirm]". State a consequence only if the
   notes state it.
5. Leave out anything marked internal or listed under "what never goes
   in". If it affects a client date or decision, list it under "Left out
   on purpose".
6. Stop and ask the responsible person, without drafting, if a confirmed
   date has passed without delivery or the inputs mix two clients.
   Flag complaints, fee, scope or staffing changes, and any advice or
   strategy content, at the top of the reviewer note.
7. Write the draft in this order: progress, confirmed dates, estimates,
   client decisions, next step. Keep it under [N] words, in plain
   sentences.
8. Write the reviewer note and end it with "Nothing has been sent."

Use exactly the output format provided.
```

Paste the output format from this template below the instructions.

## What to customize

- The definition of "confirmed" (for example, agreed by the client in writing and marked so in the task list).
- The update day for each client, and the changes that trigger an update in between.
- Length limit [N], greeting, sign-off and section order.
- The list of what never goes in.
- Who reviews and sends for each client, and who covers.
- Industry wording: "matter" in law firms, "project" in engineering and construction, "campaign" in marketing and advertising.

## Version notes

- 0.1.0, 9 November 2026. Written by Fully Powered AI. Editorially reviewed. Not yet tested in a client environment. Not yet tested in ChatGPT, Claude, Copilot or Gemini as a packaged version.
