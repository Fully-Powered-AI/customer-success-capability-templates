# Account commitments check

Before the next customer conversation, the account manager gets one list of what each side promised in recent meetings and emails, each linked to its source and marked open, done or unclear, with a suggested owner. Nothing goes to the customer.

*Capability template · Customer success and account management · version 0.1.0 · [Capabilities Directory](https://fullypowered.ai/capabilities/account-commitments-check/)*

## The outcome

The account manager walks into the next conversation knowing what has been promised on both sides since the last review, and what became of each promise. Our own promises are in the list as plainly as the customer's. Nobody is surprised by something said six weeks ago in a meeting they did not attend.

Every line points to the meeting or email where it was said, in the words used. A promise whose date moved shows both dates and who agreed the change. A promise that has been kept shows the record that says so. A promise with no record of completion is marked open, not failed: the notes supplied may cover only part of the relationship, and the list says where they do not. Wording that was only a hope ("we'll try") is marked unclear until someone firms it up.

The list ends with the items that need a decision, each as a question for the account manager, who chooses whether to chase, complete or renegotiate. The AI assistant prepares the list. It writes nothing to the customer and changes no record.

## Who starts the work, and when

The account manager or customer success manager who owns the account starts it a few days before a customer conversation, such as a renewal discussion, an escalation call or a regular check-in. It can run again when new notes arrive or the date of the conversation moves. The account manager reads the list, confirms or changes each owner and decides what to do about each open or unclear item.

## What they supply

- **Notes and emails from recent customer conversations,** each with its date, type and attendees, for the period you set.
- **Follow-through records,** such as support tickets, release notes, delivery logs or sent files, with a date for each.
- **The people on both sides,** with each person's side and role.
- **The settings:** the account name, the period, today's date and the date of the next conversation.
- **Where they have them:** the draft agenda for that conversation.

## What comes out

One list in a fixed order. At the top, the sources used, any stretch of time or meeting the sources do not cover, and the counts of commitments by side and by status. Then our commitments, the customer's, and any whose side the notes do not state. Each line gives the words, who said them and when, the due date and any change to it, the status with its evidence, and a suggested owner.

After the list come the open and unclear items that are not on the draft agenda, and the questions for the account manager. A commitment that touches price, scope or service levels is marked so it can be checked against the agreement; the assistant does not interpret the agreement.

See the worked example with invented data in [EXAMPLE.md](EXAMPLE.md).

## Where it fits

- [Software technology](https://fullypowered.ai/industries/software-technology/): fixes, access and training promised in support calls are easy to lose before the renewal.
- [Professional services](https://fullypowered.ai/industries/professional-services/): promises about deliverables and dates are made by several people across a long engagement.
- [Marketing and advertising](https://fullypowered.ai/industries/marketing-and-advertising/): a retainer collects small promises in weekly calls and email threads.
- [Customer success and account management](https://fullypowered.ai/functions/customer-success-and-account-management/): the check an account manager makes before facing the customer.
- [Growth & scaling](https://fullypowered.ai/situations/growth-and-scaling/): more accounts per manager means more promises held only in memory.
- [Established businesses](https://fullypowered.ai/situations/established-businesses/): long relationships carry promises from before the current team.

It is separate from [meeting agenda, notes and follow-ups](https://fullypowered.ai/capabilities/meeting-agenda-notes-and-follow-ups/), which serves one internal meeting, and from [quarterly business review preparation](https://fullypowered.ai/capabilities/quarterly-business-review-preparation/), which builds the review around the customer's goals. It is also separate from the [sales call preparation brief](https://fullypowered.ai/capabilities/sales-call-preparation-brief/), which is a sales brief for one prospect that includes what has been said and promised so far; this is a two-sided list of promises with a status for each, for an existing customer. [Account handoff](https://fullypowered.ai/capabilities/account-handoff/) records what was promised in the sale.

## What has to change for your company

Decide how far back the period reaches and where the notes live. Set the owner you suggest by default for each kind of promise, such as support fixes, billing corrections and training. Decide which kinds of promise count as touching terms. Agree how long a gap in the sources is worth reporting. Decide which follow-through records the assistant may read. The account manager remains the person who confirms the list.

## What has been checked

Fully Powered AI wrote this capability template. It was editorially reviewed on 10 November 2026. It was tried once on its invented example in Claude on 10 November 2026; the record is published with it. It has not yet been tested in a client environment. It has not yet been tested as a packaged version in ChatGPT, Claude, Copilot or Gemini.

Testing in your environment means running it on an account whose history your account manager already knows, with cases agreed first: a promise whose date moved, a promise kept but never written down, a hopeful remark, a note with no speaker named. The account manager checks every line against its source before anyone relies on the list. [Pilot acceptance-test preparation](https://fullypowered.ai/capabilities/pilot-acceptance-test-preparation/) sets those cases up, and [what we test before we call an AI workflow ready](https://fullypowered.ai/insights/what-we-test-before-a-workflow-is-ready/) describes the record we keep.

- Written by Fully Powered AI.
- Sources and rights reviewed.
- Editorially reviewed on 10 November 2026.
- Package format checked by script on every release.
- Tried once on its invented example in Claude on 10 November 2026. The record is in [TRIAL.md](TRIAL.md).
- Not yet tested in a client environment.

## What is in this folder

- [TEMPLATE.md](TEMPLATE.md): the complete capability template. Roles, inputs, the procedure, exceptions and stop conditions, the output format, a reviewer checklist, acceptance tests, the instructions for an AI assistant and what to customize.
- [EXAMPLE.md](EXAMPLE.md): a worked example with invented data.
- [TRIAL.md](TRIAL.md): what came out when the template was tried on its example.
- [SKILL.md](SKILL.md): the technical file, for AI products that load packaged instructions from a folder.
- [SOURCES.md](SOURCES.md): what the capability drew on, with licences.
- [LICENSE](LICENSE): MIT. Use it, change it, make it yours.

## Start using it

1. Read [EXAMPLE.md](EXAMPLE.md) to see what a good result looks like.
2. Open [TEMPLATE.md](TEMPLATE.md) and set every item under "What to customize" to your own rules, roles and limits.
3. Give your AI assistant the instruction block and the output format from the template, with your own limits in place of the ones the instructions leave open in square brackets. Paste them in as custom instructions in ChatGPT, Claude, Copilot or Gemini, or copy this whole folder into a product that loads `SKILL.md` packages. This folder stands alone; you do not need the rest of the repository.
4. Run it on past work first, using the reviewer checklist and acceptance tests in the template, before anyone relies on it.

## Related capabilities

- [Meeting agenda, notes and follow-ups](https://fullypowered.ai/capabilities/meeting-agenda-notes-and-follow-ups/)
- [Quarterly business review preparation](../quarterly-business-review-preparation/)
- [Account handoff](../account-handoff/)
- [Sales call preparation brief](https://fullypowered.ai/capabilities/sales-call-preparation-brief/)

## Make it yours

This is the starting version. Fully Powered AI adapts capabilities to how your company works, proves them on real work and rolls them out to the roles that use them. [Talk with us](https://fullypowered.ai/contact/).
