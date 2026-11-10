# Account handoff

Capability template, version 0.1.0.

## Purpose

When a deal closes, prepare one shared record that hands the account from sales to client success: what was sold, what was promised, the people on both sides, the dates, the billing terms as agreed, the risks the seller heard and what is missing. Every next action has one owner and one due date. The client success manager reviews the record and runs the kickoff. The assistant prepares; it never contacts the client, changes billing or updates a system.

## When to use it and when not to

Use it when a contract or order form is signed (or at the handoff moment your company sets), when an account moves to a new client success manager, or when a renewal or expansion adds scope delivery has not seen.

Do not use it when:

- the agreement is unsigned. Nothing should treat a draft as agreed;
- the question is what a clause means or whether it is enforceable. That goes to the contracts reviewer;
- the client is already raising a delivery problem. Handle that first.

## Roles

- **Runs it:** the account executive who closed the deal.
- **Reviews and owns the account from handoff:** the client success manager.
- **Confirms billing terms against the agreement:** the finance or contracts reviewer.
- **Answers for promises made outside the contract:** the sales lead.
- **Confirms delivery dates and scope commitments:** the solutions lead.
- **Acts on each next action:** the owner named on it.

## Inputs

1. **Signed agreement and order form.** From the contract store. The authority for what was sold, dates and billing. If missing, stop.
2. **Final proposal and evidence checklist,** or the approved account brief. If missing, continue and note that promises were checked only against the agreement and notes.
3. **Call notes and emails from the sale.** If none, ask the account executive for a written note of what the client was told and what risks they heard.
4. **Known contacts** on both sides, with roles. A required contact that is missing goes under Missing.
5. **Your onboarding checklist** for this client type, from client success. If missing, use the record's sections and note that no checklist was applied.

## The procedure

1. **Confirm the trigger.** Check both parties have signed and record the date. If not, stop.
2. **Set the authority order.** Unless your company sets another: signed agreement, order form, final proposal, emails, call notes. The higher source governs the record; every disagreement is still listed.
3. **Sold.** Every service, quantity, service level, term and exclusion, with clause or schedule references. Keep service levels in their exact words.
4. **Promised.** Commitments in the agreement, then commitments found only in the proposal or emails. Mark each "in agreement" or "outside agreement: sales lead to confirm".
5. **People.** Client side: signer, sponsor, day-to-day contact, billing contact, others named. Your side: account executive, client success manager, solutions lead, finance reviewer. Write "not yet known" for a role with no person.
6. **Dates.** Signature, service start, kickoff, first deliverable, first invoice. Mark each "confirmed" (in the agreement, or confirmed in writing by your side) or "requested". A requested date never appears as confirmed.
7. **Billing as agreed.** Frequency, timing, fees by schedule reference, payment terms, first invoice date, billing contact. Copy; never calculate.
8. **Risks the seller heard.** In the client's words where possible, with source and date: previous-provider failures, client-side disagreement, deadlines, expectations beyond the agreement.
9. **Discrepancies.** Quantities, dates, scope, contacts and terms that differ between sources: what each says, which governs, who resolves it.
10. **Missing.** Items the onboarding checklist requires that no source supplies.
11. **Next actions.** One per discrepancy, gap and unconfirmed date, each with one owner and a due date within [your handoff window] of signature. Default owners: the account executive for anything the client must supply; the finance reviewer for billing; the solutions lead for delivery dates and scope; the sales lead for promises outside the agreement; the client success manager for kickoff.
12. **Return the record** to the client success manager for review and the account executive for corrections.

## Exceptions and stop conditions

- **Agreement unsigned or missing:** stop; tell the account executive.
- **A promise outside the agreement changes scope, price or a service level:** flag it to the sales lead and the finance or contracts reviewer before kickoff.
- **The order form's billing terms contradict the agreement:** list both; nothing about billing is marked confirmed until the finance or contracts reviewer decides.
- **No client success manager assigned:** the first next action, owned by [your client success lead role].
- **The notes record a complaint, a threat to cancel or a dispute:** put it first under Risks; flag it to the client success manager and sales lead the same day.
- **Asked to send the record or a message to the client:** decline; the client success manager sends client communications.

## Output format

```
ACCOUNT HANDOFF: [Client]
Prepared [date] from: [sources with dates]

SOLD
[Service, quantity, service level, term]. Excluded: [exclusions]. ([source, clause])

PROMISED
[Commitment] ([source]) [in agreement / outside agreement: sales lead to confirm]

CLIENT PEOPLE
[Role]: [person or "not yet known"]: [part in the account]

OUR PEOPLE
[Role]: [part in the account]

DATES
[Event]: [date] [confirmed / requested] ([source])

BILLING AS AGREED
[Frequency, timing, fees by schedule reference, payment terms, first invoice, billing contact] ([source])

RISKS THE SELLER HEARD
[Risk, in the client's words where possible] ([source, date])

DISCREPANCIES
[Item]: [source A says]; [source B says]. Governs: [source]. Resolves: [role].

MISSING
[Item required by the onboarding checklist]

NEXT ACTIONS
[n]. [Action]. Owner: [role]. Due: [date].

Status: Prepared for the client success manager's review. Nothing has been sent to the client and no system has been changed.
```

## Reviewer checklist

1. Sold matches the signed agreement and order form, with references. (Client success manager)
2. Every promise outside the agreement is marked and has gone to the sales lead. (Client success manager)
3. No requested date is shown as confirmed. (Client success manager)
4. Billing terms match the signed agreement. (Finance or contracts reviewer)
5. Every discrepancy names which source governs and who resolves it. (Client success manager)
6. Every next action has one owner and a due date. (Client success manager)
7. The risks include everything the account executive heard. (Account executive)
8. The record is accepted and the kickoff scheduled. (Client success manager)

## Acceptance tests

Proposed tests. None has been run.

1. **Clean handoff.** All sources agree; every contact known. Expected: complete record; only kickoff actions; no discrepancies.
2. **Quantity conflict.** Proposal says up to 320 devices; order form says 300. Expected: 300 recorded as sold; both quoted; order form governs; account executive confirms with the client.
3. **Requested date.** The client asked for kickoff in the week of 26 October; nobody confirmed. Expected: shown as requested, with an action for the client success manager. Fails if shown as confirmed.
4. **Promise only in an email.** The account executive wrote "we'll waive the setup fee". Expected: outside agreement; flagged to the sales lead and finance or contracts reviewer.
5. **Missing billing contact.** Expected: under Missing; action owned by the account executive.
6. **Unsigned agreement.** Expected: stops; no record prepared.
7. **Risk in the notes.** Notes say the previous provider left new starters waiting a week. Expected: under Risks with source and date.
8. **Asked to send.** Expected: declines; names the client success manager as sender.

## Instructions for the AI assistant

```
You prepare account handoff records from sales to client success. You never
contact the client, change billing or update any system.

The user supplies: the signed agreement and order form; the final proposal
and evidence checklist or the approved account brief; call notes and emails
from the sale; known contacts; the onboarding checklist.

1. Check both parties have signed. If not, stop and say so.
2. Authority order, unless the user gives another: signed agreement, order
   form, final proposal, emails, call notes. The higher source governs the
   record; list every disagreement anyway.
3. SOLD: every service, quantity, service level, term and exclusion, with
   clause or schedule references, service levels in their exact words.
4. PROMISED: commitments in the agreement, then those found only in the
   proposal or emails, marked "in agreement" or "outside agreement: sales
   lead to confirm".
5. CLIENT PEOPLE and OUR PEOPLE by role; "not yet known" for a role with no
   person.
6. DATES: each marked "confirmed" (in the agreement or confirmed in writing
   by our side) or "requested". Never show a requested date as confirmed.
7. BILLING AS AGREED: copy terms; never calculate.
8. RISKS THE SELLER HEARD: the client's words where possible, with source
   and date. Put any complaint, cancellation threat or dispute first.
9. DISCREPANCIES: what each source says, which governs, who resolves it.
10. MISSING: items the onboarding checklist requires that no source supplies.
11. NEXT ACTIONS: one per discrepancy, gap and unconfirmed date, each with
    one owner by role and a due date. Default owners: account executive for
    anything the client must supply; finance reviewer for billing; solutions
    lead for delivery dates and scope; sales lead for promises outside the
    agreement; client success manager for kickoff.
12. End with: "Status: Prepared for the client success manager's review.
    Nothing has been sent to the client and no system has been changed."

Start with "ACCOUNT HANDOFF: [Client]" and "Prepared [date] from: [sources]",
then the headings above in order. Cite the source in brackets after every
line. If asked to send the record or any message, decline and name the
client success manager as the sender.

If a promise outside the agreement changes scope, price or a service
level, flag it for the sales lead and the finance or contracts reviewer.
If the order form's billing terms contradict the agreement, list both and
mark nothing about billing confirmed. If no client success manager is
assigned, make assigning one the first next action.
```

## What to customize

- The handoff moment (signature, countersignature or first payment) and [your handoff window].
- The authority order, if yours differs.
- The onboarding checklist for each client type.
- Default owners by role, and [your client success lead role] for unassigned accounts.
- Where the shared record lives and who may edit it.
- Which deal records the assistant may read in ChatGPT, Claude, Copilot or Gemini.

## Version notes

- 0.1.0, 9 November 2026. Written by Fully Powered AI. Not yet tested in a client environment.
