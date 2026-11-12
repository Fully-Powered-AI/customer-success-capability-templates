# Customer onboarding plan: one trial run on the invented example

- **Product:** Claude, run in Claude Code
- **Model:** Claude Opus 5.5 (model ID `claude-opus-5-5`)
- **Date:** 2026-11-09
- **Template version:** 0.1.0

This is a record of one run of the workflow template on its own invented example (Customer K, an invented architecture studio, and an invented seller of time-tracking and invoicing software). The companies, the people, the dates and the notes are invented, and no client data was used. It shows what the template produced once, on one set of inputs. It is not a test in any company's environment.

This is the second run on the same example. An earlier run the same day showed where the instructions left room to guess; the instructions, the output format and the example were revised, and the run recorded here was made on the revised instructions. What the earlier run found, and what was changed, is at the end. Dates inside the plan belong to the invented scenario (today is Thursday 12 November 2026 there); the date above is the day of the trial.

## How it was run

The run was a fresh session started from Claude Code with no tools, no access to any file and no project instructions. The template's instructions for the AI assistant and its output format were given as the session's instructions, and the four inputs were sent as one message. The session was started by the session that revised the template, but the model in the run saw only those instructions and inputs: not the procedure, not the reviewer checklist, not the example's published output and not the earlier run.

## The inputs used

Exactly the four inputs in [the worked example](example.md), under "The inputs": the account handoff record, our facts, the kickoff notes and the settings. Nothing was added or changed. The settings gave no milestone limit or stall threshold, so the defaults applied. This is a first run, so there was no status update and no last-activity date.

## What came out

The complete output, as returned:

```text
CUSTOMER ONBOARDING PLAN: Customer K, plan on Thursday 12 November 2026

For: customer success lead. Run by customer success lead on Thursday 12 November 2026; drafted by the AI assistant, not yet approved.
Sold: Time tracking and invoicing, 18 user seats, annual subscription; included: two 60-minute setup sessions with an onboarding specialist, import of one timesheet spreadsheet, email support; excluded: connection to the studio's accounting software (quoted, not bought) (order form, 9 November 2026).
Start Monday 16 November 2026 (day 1). Window: Monday 16 November 2026 to Tuesday 15 December 2026 (30 days, the start date counted as day 1). Check-ins: weekly, Wednesdays. Closed days: Thursday 26 November 2026, Friday 27 November 2026.
Sources: account handoff record, 10 November 2026; your facts (customer success lead); kickoff notes, Thursday 12 November 2026; not a progress run.
Defaults used: milestone limit 7; stall threshold 10 days.

THE OUTCOME
First real use: The office manager produces the December invoice run's client invoices for November from the hours in the system, in Customer K's own account, without help from our side. The hours are the imported 1 to 13 November timesheet and the hours logged from 16 November. The office manager checks each invoice total against the timesheet report before anything is sent.
Seen when: For every client billed in the December run, a draft invoice exists in Customer K's account. The office manager has compared each total with the timesheet report and recorded it as matching, or named the difference, before any invoice is sent.
Due: Tuesday 1 December 2026 (the December client invoice run, the studio's first working day of the month).
The customer's goal, in their words: "If December's invoices come out of the new system and they're right, that's a win." (managing partner, kickoff notes, Thursday 12 November 2026)

SETTLE FIRST: 1
S1. Create the 18 logins and set each person's role in Customer K's account, using the invitation list format our onboarding specialist sends. Customer owner: studio IT contact. Our owner: onboarding specialist. Due: Monday 16 November 2026. Why it cannot wait: Every user who logs time (M2, M6) needs a login, and the office manager needs her role to check imports, check the template and draft invoices (M3 to M7). The studio IT contact works only on Mondays and Wednesdays.

MILESTONES TO FIRST REAL USE: 7 of a limit of 7

M1 Tuesday 17 November 2026. Office manager sends the client list with billing rates and the 1 to 13 November timesheet spreadsheet, in our import template.
- Customer owner: office manager.
- Our owner: onboarding specialist.
- Waits on: the import template from our onboarding specialist (promised Thursday 12 November 2026).
- Seen when: both files reach the onboarding specialist in the template's format.
- Kept because: nothing can be imported without them. The client list with billing rates is listed as missing in the handoff record, and the office manager gave this date.

M2 Friday 20 November 2026. Architects, designers and every other user log their time for Monday 16 to Friday 20 November.
- Customer owner: office manager (the managing partner sends the note to colleagues, message 4).
- Our owner: onboarding specialist.
- Waits on: S1.
- Seen when: the timesheet report for 16 to 20 November shows hours for every login.
- Kept because: first real use bills tracked hours, and the studio's previous tool failed when "nobody but me used it". This milestone also shows early whether late timesheets are a problem.
- Note: several people complete it over several days, so it is dated to its deadline.

M3 Tuesday 24 November 2026. Office manager checks the imported clients, projects, billing rates and 1 to 13 November hours in the account against her own spreadsheets, in setup session 2.
- Customer owner: office manager.
- Our owner: onboarding specialist, who imports the client list with billing rates and the 1 to 13 November timesheet spreadsheet before it.
- Waits on: S1, M1, our two imports.
- Seen when: on screen, the office manager goes through each client, each rate and each person's 1 to 13 November hours. She says they match, or lists the differences.
- Kept because: the December invoices bill these rates and these hours. A wrong rate gives a wrong total.
- FLAG, undated commitment: needs the import of the client list with billing rates by Monday 23 November 2026; no date has been promised.
- FLAG, date: needs the 1 to 13 November timesheet import by Monday 23 November 2026. The order form promises it only "before the December invoice run".

M4 Tuesday 24 November 2026. Office manager checks the invoice template in the account against a current studio invoice, in setup session 2.
- Customer owner: office manager.
- Our owner: onboarding specialist, who sets up the invoice template before it.
- Waits on: the customer success lead's answer on layout and logo; a logo file and a current invoice (see GAPS).
- Seen when: a test invoice from the account sits beside a current studio invoice. The office manager marks each part as the same or different, and either accepts the template or lists the changes she needs.
- Kept because: the office manager asked to keep the current layout with the logo. If she will not send an invoice from the template, the real run is blocked.
- FLAG, undated commitment: needs the customer success lead's answer on layout and logo by Monday 23 November 2026; no date has been promised.
- FLAG, beyond what was sold: "We'll have your invoices looking just like the ones you send today" is in the account executive's email only, not in the order form. This is for the sales lead.

M5 Wednesday 25 November 2026. Office manager drafts invoices on her own for 1 to 13 November, a period already worked, and checks each total against the timesheet report. This is a rehearsal on past work, not first real use.
- Customer owner: office manager.
- Our owner: onboarding specialist.
- Waits on: M3, M4.
- Seen when: draft invoices for 1 to 13 November exist in the account, none sent. The office manager has recorded each total as matching the timesheet report, or named the difference. This is reviewed at the Wednesday 25 November check-in.
- Kept because: it is your usual step 6. It lets her practise the check before the real run and before the two closed days.

M6 Monday 30 November 2026. Every user has logged all of their November hours from Monday 16 to Monday 30 November.
- Customer owner: office manager.
- Our owner: onboarding specialist.
- Waits on: S1, M2.
- Seen when: the timesheet report for 16 to 30 November shows hours for every login on each working day.
- Kept because: the December run bills every November hour. The managing partner said two senior architects "never fill in timesheets on time".
- Note: dated to its deadline (several people, several days).

M7 Tuesday 1 December 2026. Office manager produces the December run's client invoices for November and checks each total against the timesheet report before anything is sent (first real use; closing session).
- Customer owner: office manager.
- Our owner: onboarding specialist, watching only.
- Waits on: M3, M4, M5, M6.
- Seen when: as in THE OUTCOME.
- Kept because: this is the outcome. It is also your usual step 7, the first live invoice run.

AFTER FIRST REAL USE: 2

A1. Project budget reports (your usual step 8). Owner: customer success lead. By: Wednesday 9 December 2026. Moved here because: it is a usual step every customer gets, but the December invoices do not need it.

A2. Mobile app for site visits (your usual step 9). Owner: onboarding specialist. By: Wednesday 9 December 2026. Moved here because: it is a usual step every customer gets, but time can be logged for the December run without it.

COMMITMENTS

Ours:
- Send the import template and the invitation list format. Owner: onboarding specialist. Due Thursday 12 November 2026. (onboarding specialist, kickoff notes, 12 November 2026)
- Import the studio's timesheet spreadsheet for 1 to 13 November. Owner: onboarding specialist. Due before Tuesday 1 December 2026. Waits on: the office manager sending the spreadsheet (M1). (order form, 9 November 2026)
- Check whether the invoice layout and logo can match, and come back to the studio. Owner: customer success lead. No date set. (customer success lead, kickoff notes, 12 November 2026)
- "We'll have your invoices looking just like the ones you send today." Owner: account executive. No date set. (account executive's email, 4 November 2026)
  FLAG, beyond what was sold: for the sales lead. This is not in the order form, and the handoff record says "sales lead to confirm".

The customer's:
- Send the client list with billing rates and the 1 to 13 November timesheet spreadsheet. Office manager. We check on Tuesday 17 November 2026 (the date they gave). (kickoff notes, 12 November 2026)
- Create all 18 logins once we send the invitation list format. Studio IT contact. We check on Monday 16 November 2026 (no date given: the first day the studio IT contact is available after the invitation list format arrives, which was promised for Thursday 12 November 2026; they work Mondays and Wednesdays). (kickoff notes, 12 November 2026)

MESSAGES: 7

1. Send the invitation list format and ask for the logins. To: studio IT contact. From: onboarding specialist. When: Thursday 12 November 2026. Serves: S1; our commitment to send the invitation list format.
Draft: "Hello. As promised at today's kickoff, attached is the invitation list format for Customer K's 18 logins. Once you have it, please create the logins and set each person's role in the account. The roles are for the office manager, the managing partner, and the architects and designers who log their time [confirm the full list with the customer success lead]. The service starts on Monday 16 November, and we will look for the logins that day. Please do not send us any passwords or login codes; we do not need them. Our first setup session is on Wednesday 18 November [time to be agreed], and you are welcome to join it."

2. Send the import template and confirm the files. To: office manager. From: onboarding specialist. When: Thursday 12 November 2026. Serves: M1; our commitment to send the import template.
Draft: "Hello. As promised at today's kickoff, attached is the import template. Please put the client list with billing rates, and your timesheet spreadsheet for 1 to 13 November, into this format and send both to me by Tuesday 17 November, as you said. If your projects are listed separately from clients, please tell me how you keep them. Once I have the files I will import them, and in our second setup session you will check the clients, rates and hours against your own spreadsheets."

3. Invitation to setup session 1, with the check-in dates. To: managing partner, office manager, studio IT contact. From: onboarding specialist. When: Friday 13 November 2026. Serves: setup session 1; check-ins.
Draft: "Hello. This is an invitation to our first 60-minute setup session on Wednesday 18 November [time to be agreed]. We will confirm that logins and roles are in place, show how time is logged, and walk through the timesheet report the office manager will use to check invoice totals. We will also hold short weekly check-ins on Wednesday 18 November, Wednesday 25 November, Wednesday 2 December and Wednesday 9 December. The aim we are working to, in the managing partner's words: 'If December's invoices come out of the new system and they're right, that's a win.'"

4. Note the managing partner can send to colleagues. To: the 14 architects and designers and every other user who logs time. From: managing partner. When: Monday 16 November 2026. Serves: M2, M6.
Draft: "Hello all. From today we log our time in our new time tracking system. Our studio IT contact is setting up your login. Please log your hours each day from today. By Friday 20 November, everyone's hours for this week should be in. By Monday 30 November, all of your hours from 16 to 30 November should be in. Our office manager will build December's client invoices from these hours. If you have a question, please ask our office manager."

5. Recap of setup session 1 and invitation to setup session 2. To: managing partner, office manager, studio IT contact. From: onboarding specialist. When: Wednesday 18 November 2026. Serves: setup session 1; S1; M2; M3; M4.
Draft: "Thank you for today's session. Logins and roles: [confirm after the session]. What we covered: logging time and the timesheet report [confirm after the session]. Next, everyone logs their time for 16 to 20 November by Friday 20 November. Our second 60-minute setup session is on Tuesday 24 November [time to be agreed], with the office manager. She will check the imported clients, projects, rates and 1 to 13 November hours against her spreadsheets. She will also check the invoice template against one of the studio's current invoices; whether the layout and logo can match is [confirm after the session]."

6. Recap of setup session 2 and invitation to the closing session. To: managing partner, office manager. From: onboarding specialist. When: Tuesday 24 November 2026. Serves: setup session 2; M3; M4; M5; M6; M7.
Draft: "Thank you for today's session.
- Imported clients, rates and hours: [confirm after the session].
- Invoice template: [confirm after the session].
- Next: by Wednesday 25 November, the office manager drafts invoices for 1 to 13 November on her own and checks each total against the timesheet report. None of these drafts are sent. We will look at them together at that day's check-in. By Monday 30 November, all November hours are logged.
- Closing session, Tuesday 1 December [time to be agreed]: the office manager produces the December invoices and checks each total before anything is sent, with our onboarding specialist watching on a shared screen. After that, the managing partner reviews the result and signs off. Please both attend."

7. Recap of the closing session and the notes. To: managing partner, office manager. From: onboarding specialist. When: Tuesday 1 December 2026. Serves: M7; follow-up check.
Draft: "Thank you for today's session. Result: [confirm after the session]. Sign-off by the managing partner: [confirm after the session]. Your notes:
- How to do it: [confirm after the session].
- How to check it: compare each invoice total with the timesheet report before anything is sent.
- What it does not cover: invoices do not go into your accounting software; that connection is not part of this order.
- How to ask for help or a change: email support at [support address].
- What to do by hand if it fails: [confirm after the session].
Our follow-up check is on Wednesday 3 February 2027, after your January and February invoice runs."

RISKS: 7

1. The office manager spends two days each month building invoices from spreadsheets.
   - Source: office manager, call notes, 21 October 2026.
   - What the plan does: rehearses the checking method on past work (M5) before the real run, and has the follow-up check look at whether the office manager built the runs without help.
   - Owner: customer success lead.

2. The previous tool was dropped after a month: "nobody but me used it".
   - Source: office manager, call notes, 21 October 2026.
   - What the plan does: makes every user's logged time a milestone (M2, M6). The note to colleagues comes from the managing partner, not the office manager. The follow-up check looks at whether colleagues use it.
   - Owner: customer success lead.

3. Two senior architects "never fill in timesheets on time".
   - Source: managing partner, call notes, 28 October 2026.
   - What the plan does: sets an early deadline (M2, Friday 20 November) so gaps show before the run, and a final deadline of Monday 30 November (M6). It plans no reminder series. The Friday view of who has not logged is a question under GAPS.
   - Owner: managing partner (customer); onboarding specialist reads the timesheet report.

4. One person, part-time, manages logins (the studio IT contact works Mondays and Wednesdays only).
   - Source: kickoff notes, 12 November 2026.
   - What the plan does: dates S1 on a Monday. If the logins are not done then, Wednesday 18 November still falls before the M2 deadline. Any later access change also waits for a Monday or Wednesday.
   - Owner: onboarding specialist.

5. One person builds the invoices: the office manager is the only invoicing user.
   - Source: handoff record, 10 November 2026.
   - What the plan does: books the closing session on the run day itself and has the office manager practise on past work first (M5). Who covers if she is unavailable is not stated.
   - Owner: customer success lead.

6. Everything depends on one day: all November hours must be in by Monday 30 November, the run is the next day, and Thursday 26 and Friday 27 November are closed.
   - Source: settings; handoff record.
   - What the plan does: puts the rehearsal (M5) on Wednesday 25 November, before the closed days, and checks hours at the Wednesday check-ins.
   - Owner: onboarding specialist.

7. The invoice layout and logo match is promised outside the order form, and our answer has no date.
   - Source: account executive's email, 4 November 2026; office manager, kickoff notes, 12 November 2026.
   - What the plan does: makes the template check a milestone (M4), flags the undated answer, and sends the promise to the sales lead.
   - Owner: customer success lead.

OUTSIDE WHAT WAS SOLD: 2

1. Invoices going straight into the studio's accounting software. Source: office manager, kickoff notes, 12 November 2026; listed as excluded in the order form, 9 November 2026. For: sales lead.

2. "We'll have your invoices looking just like the ones you send today." The usual invoice template step is planned (M4); an exact match is not. Source: account executive's email, 4 November 2026. For: sales lead.

CHECK-INS AND CLOSE
Check-ins: Wednesday 18 November 2026, Wednesday 25 November 2026, Wednesday 2 December 2026, Wednesday 9 December 2026.
Closing session: Tuesday 1 December 2026 (M7).
- The office manager does the work on the December invoice run for November's hours, with the onboarding specialist watching on a shared screen.
- A wrong result is dealt with before sign-off.
- Then the managing partner signs off against the outcome.
- Then the customer receives the notes: how to do the work, how to check it, what it does not cover, how to ask for help or a change, and what to do by hand if it fails.
- The session ends with the follow-up check date said aloud.

Follow-up check: Wednesday 3 February 2027, after the Monday 4 January 2027 and Monday 1 February 2027 invoice runs (2 turns of the monthly invoice cycle).
Looks at: whether the office manager produced and checked each run's invoices without help; whether every user, including the senior architects, logged their time.

PROGRESS: not run: this is the first plan

NOTES TO CHECK: "Also email all the architects a reminder every morning to log their time." (managing partner, kickoff notes, Thursday 12 November 2026). Not acted on. This plan includes no reminder series.

GAPS: 8

1. Seats against logins: 18 seats were sold and 18 logins are to be created, but the handoff names 17 people (managing partner, office manager, studio IT contact, 14 architects and designers). Used: 18 logins, as the studio IT contact said. Question for customer success lead: who holds the 18th login, and does the studio IT contact need one?

2. Projects: your usual step 2 imports clients, projects and billing rates, but the office manager promised only the client list with billing rates. Used: the client list; message 2 asks how projects are kept. Question for customer success lead: where does the project list come from?

3. The managing partner wants to see each Friday who has not logged their time. I cannot place this from the inputs. Used: nothing. Question for customer success lead: is this view part of what was sold, and who sets it up?

4. Sessions: 3 sessions are planned with our side present (setup session 1 on Wednesday 18 November, setup session 2 on Tuesday 24 November, closing session on Tuesday 1 December), but 2 setup sessions were sold. Used: all three in the plan. Question for customer success lead: does the closing session count as one of the two sold sessions?

5. The invoice template needs a logo file and a current studio invoice to compare against. Neither is in the inputs. Used: nothing. Question for customer success lead: who supplies them, and by when?

6. The support email address is not in the inputs. Used: "[support address]" in message 7. Question for customer success lead: what address goes in the closing notes?

7. The December run is assumed to bill November work (1 to 13 November imported, 16 to 30 November tracked). Used: that assumption for M6 and M7. Question for customer success lead: please confirm.

8. Session times and the managing partner's availability on Tuesday 1 December are not stated. Used: "[time to be agreed]". Question for customer success lead: when can the office manager and the managing partner attend?

Prepared for customer success lead. Nothing has been sent, no one at Customer K has been contacted, and no record, access or setting has been changed.
```

## What was observed

**What held.** Every section of the output format was produced, in order, and nothing in the inputs called for a stop. The points the earlier run had to guess at came out as the revised instructions intend:

- The window runs from Monday 16 November to Tuesday 15 December 2026, with the start date counted as day 1.
- Settle first has one item, the logins. The office manager's client list and timesheet file is M1. Our own sending of the import template and the invitation list format is under Commitments and named in M1's "Waits on" and in S1's wording, not as a settle-first item.
- Budget reports and the mobile app are planned after first real use, as usual steps every customer gets. The past-timesheet import, marked "when bought", was sold and is planned.
- The seats, the annual subscription and email support are on the Sold line only. The 18 seats against the 17 people named is a question under Gaps.
- The three sessions planned with our side present (two setup sessions and the closing session) against the two sold is a question under Gaps, and no message offers an extra session.
- Both requests that were not sold go to the sales lead.
- The studio IT contact's undated promise is checked on Monday 16 November, with the basis written beside it.
- The check-in dates go once into an early invitation (message 3), and no check-in has a recap of its own.
- The closing session has the onboarding specialist "watching only", the sign-off after the run and before the notes, and the follow-up date (Wednesday 3 February 2027) said aloud at the end.
- The kickoff note asking for a reminder email every morning is quoted under Notes to check, and no reminder series was drafted.
- The layout answer, which has no date, is not dated; M4, which waits on it, carries the new flag.

**Where the run went wrong or the instructions still leave room to guess.**

- The undated-commitment flag was also put on M3 for the import of the client list, which is our own usual setup step, not a promise listed under Commitments. The instructions said "a commitment with no date set" without saying which. Clarified after this run (see the end); not run again.
- Each milestone and risk was set out as a short bullet list rather than the single line the output format gives. The fields are the same.
- The note to colleagues (message 4) is sent by the managing partner; the inputs do not say who should send it. It opens "From today we log our time in our new time tracking system" and asks people to log their hours each day; neither is in the inputs, though the first follows from the start date and the logins.
- The run split the users' logging into two milestones, the first week by Friday 20 November (M2) and all November hours by Monday 30 November (M6), using the rule that a milestone several people complete is dated to its deadline. That makes seven milestones, the limit.
- It placed setup session 2 on Tuesday 24 November rather than on a Wednesday check-in, and rehearsed the invoices on the imported 1 to 13 November hours, with the office manager on her own on Wednesday 25 November.
- It made M4, the invoice template check, wait on the customer success lead's undated answer on the layout and on a logo file and a current invoice. The published example uses the standard layout until the sales lead confirms and does not wait.
- It asked under Gaps for confirmation that the December run bills November's work. The inputs imply this (the 1 to 13 November import is promised "before the December invoice run") but never state it.

**Differences from the published example** (compared after the run; the example's output was revised after the run, as listed at the end, and this comparison is against the revised example):

- Milestones: seven in the run, six in the example. Both start with the office manager's file on Tuesday 17 November and end with first real use on Tuesday 1 December. The example has one users' logging milestone (16 to 19 November, by Friday 20 November) and keeps the 30 November cut-off as something M6 waits on; the run makes that cut-off its own milestone.
- Setup session 2: Tuesday 24 November in the run, Wednesday 25 November in the example. The rehearsal: imported 1 to 13 November hours in the run, 1 to 19 November in the example.
- After first real use: the same two steps; the mobile app is due Wednesday 9 December in the run and Tuesday 15 December in the example.
- Commitments: the run keeps the account executive's "just like the ones you send today" as its own line, owned by the account executive; the example folds it into the layout line.
- Messages: seven in the run, six in the example. The run sends the template and the format as two messages, one to each recipient, and has the managing partner send the note to colleagues; the example combines the first two and has the office manager send the note.
- Risks: seven in the run, four in the example. The run adds the office manager as the only person who invoices, the single day before the run after the closed days, and the layout promise.
- Gaps: eight in the run, four in the example. Both raise the eighteenth seat, the third session and the Friday view of who has not logged. The run adds the project list (our usual step imports projects, but the office manager promised only the client list), the logo file and current invoice, the support address, the December run billing November's work, and the session times. The example lists the missing client list, which the run handles as M1 without a gap.
- Outside what was sold, Notes to check, the check-ins and the follow-up check: the same.

**Facts in the outputs that are not in the inputs.**

- In the run's output: message 4's "from today" and "each day"; the managing partner as its sender; message 1's line asking the IT contact not to send passwords or login codes (from the template's rules, not the inputs); the office manager as the only person who invoices, sourced to the handoff record, which says she builds the invoices today; M6's "hours for every login on each working day"; the account executive as owner of the email promise. No result, figure or name was invented.
- In the example's output: "billing November's hours" on the Due line, and message 2's "once they match, the team can log their hours for this week". Both follow from the inputs and the plan; neither is stated in the inputs.

**Against the reviewer checklist,** the run's plan meets items 1 to 8 as far as they apply to a first plan. Item 3 needs attention for the stray flag on M3, and item 6 for message 4's "each day from today", an ask the plan itself does not make. Item 9 is the progress run and was not exercised.

**What this run does not show.** It is one run on one invented example, by one model. It did not exercise a progress run, the silent-account check, a stall, an unmatched column or any decline or stop rule. The template's acceptance tests have not been run.

## The earlier run, and what was changed

The first run, on 9 November 2026 in Claude Code with Claude Sonnet 5.5 (`claude-sonnet-5-5`), used the template as first written and the same four inputs. The model had not written the template; it read it, took only the inputs, and compared with the example's output afterwards. It produced every section, and differed from the example then published in these ways:

- It put three items under Settle first (our sending of the template and format, the logins, and the office manager's file), where the example had one (the logins) and made the file M1. The template had given "a data file" as a settle-first example while also asking for a first milestone the customer can finish in the first few days.
- It wrote ten messages to the example's six, with separate requests for the logins and the file and an invitation and recap for each session.
- It raised six gaps to the example's two, including the budget reports and the mobile app not being on the sold list, the closing session as a possible third session, and 18 seats against 17 people.
- It sent the accounting connection to the sales lead; the example sent it to the account executive.

It named these as places where it had to guess: how the window's last day is counted; settle first against first milestone; whether our own prerequisite belongs under Settle first; watching against helping at the closing session; a milestone that is really our setup work; a usual step that was not clearly sold; sold items that are not steps; the sessions sold; whether check-ins need messages and whether requests may be combined; a milestone waiting on an undated commitment; the date to check a customer's undated promise; a milestone several people complete over several days; where requests outside the sale go; and "Prepared by" when the assistant prepares. It also found two statements in the example's output that the inputs do not support, one of them made to the studio's staff: that hours missing on 30 November are not billed, and that they leave the December invoices short.

Changed after the first run, before the run recorded above:

- **The window** is counted with the start date as day 1, in the procedure and the pasted instructions.
- **Settle first** is access the customer grants (logins, roles, permissions). A file the customer prepares and sends is a milestone, often the first. Our own prerequisites are commitments, named in "Waits on".
- **Usual steps and sold items.** Your facts mark steps "when bought"; what is planned is what was sold plus usual steps every customer gets; a "when bought" step that was not sold is a question under Gaps. Sold items that need no step go on the Sold line, and the seats are checked against the logins. The reviewer checklist's item 4 says the same.
- **Sessions** planned with our side present are counted against those sold, with a question under Gaps if there are more; no message offers an extra session.
- **Milestones.** Setup only we can do is not a milestone of its own; a milestone several people complete is dated to its deadline; a milestone waiting on an undated commitment is dated where the plan needs it and flagged.
- **Commitments.** The check date for a customer's undated promise is the first day that role is available after what it waits on has arrived, or the next check-in, with the basis written.
- **Messages.** Check-in dates go once into an early invitation; messages to the same people on the same day may be combined; no message states a consequence the inputs do not give.
- **The closing session.** Watching is not helping; a step our specialist does or talks the lead user through is dealt with as a wrong result is.
- **The header** says who ran the plan and that the AI assistant drafted it, not yet approved. Requests outside the sale always go to the sales lead.
- **The pasted instructions** now carry "no kickoff notes yet", "your facts not supplied; usual steps not applied" and "silent-account check not run".
- Two acceptance tests were added (a usual step not bought; more sessions than sold). None has been run.

Changed after the run recorded above, and not run again:

- **The undated-commitment flag** now applies only to a promise listed under Commitments, not to our own usual setup work, in the procedure and the pasted instructions.
- **The example's published output** was revised the same day to follow the revised rules and the independent review. The run did not see it before or after. The changes: message 3 to the architects and designers and the risk on late timesheets no longer say what happens to hours that are missing (message 3 now says December's invoices are drafted from the hours logged by Monday 30 November, which is the plan's own cut-off); message 1 no longer says the whole team can start logging that week; the rehearsal (M5) covers 1 to 19 November, matching the hours M3 asks for; M4 is the office manager's check of the template our specialist sets up; message 2 carries the check-in dates; message 5 confirms the follow-up date the plan already fixes rather than asking to set one; the accounting connection goes to the sales lead; the studio IT contact's check date gives its basis; the window line counts the start date as day 1; the header names who ran it; the eighteenth-seat and third-session questions were added under Gaps; and M6 names the specialist as "watching only", the run's wording.

Changed after the independent review on 10 November 2026, and not run again. The comparison with the published example above was made before these changes, so it no longer matches the example on the points marked:

- **The pasted instructions and the procedure.** The note to colleagues comes from the customer's lead user unless the inputs name another sender (the run chose the managing partner; see above). A message asks for nothing the plan does not ask for (the run's message 4 asked for hours "each day from today"). A wrong result at the closing session is explained, then either run again on another piece of work or recorded as a defect with an owner, as the procedure already said. A step after first real use counts against the sessions sold when the plan holds it as a session with our side present, and one whose delivery the plan leaves open is named in the sessions question. The step "List every step" is now "Set out the whole path", with the same content. The column mapping for a status sheet is listed among the settings.
- **The example's published output.** The account executive's emailed promise is now its own line under Commitments, owned by the account executive and flagged for the sales lead, as the run had it (this changes the Commitments difference noted above). Our first commitment no longer names recipients the kickoff notes do not state. The office manager's commitment gives its basis, "the date they gave". Gaps now has five items: the sessions question also asks whether A1 and A2 are sessions, and a new gap asks the customer success lead to confirm that the December run bills November's hours, which the run also raised and which the observation on the example's facts above notes (this changes the Gaps difference noted above).
- The output format still sets each milestone and risk on a single line; the run's bullet lists are left as recorded.
