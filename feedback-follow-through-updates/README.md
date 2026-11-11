# Feedback follow-through updates

When a change ships or a decision lands on something customers asked for, your account owner gets the list of who asked, the confirmed status of each request, and an individual draft update for each person in the channel they prefer. No update promises a date or feature the team has not confirmed.

*Capability template · Customer success and account management · version 0.1.0 · [Capabilities Directory](https://fullypowered.ai/capabilities/feedback-follow-through-updates/)*

## The outcome

Every customer who took the time to ask hears back, personally, about what they asked for. The update speaks to their request, in their terms: what is live now, what part is still open and where that part stands. It arrives by email, in a call, in a message or at their next account meeting, whichever they prefer.

Nothing in it runs ahead of the team. Each date and each feature in a draft is traced to the change record the product or service team confirmed, and the draft shows where each one came from. Internal targets stay internal. A customer who has asked not to be contacted, or who tied the request to cancelling or to looking at other tools, is held back for the account owner to handle in person.

The account owner approves every update and sends it. The AI assistant sends nothing and changes no record.

## Who starts the work, and when

The account manager or customer success manager starts it once the responsible team has confirmed, in writing, what a change does, what it leaves out and when it is available, or has decided not to go ahead. That is usually the day a change goes live or the week a decision is made. It runs once per change, across the account owner's own accounts.

The product manager or service lead who owns the change confirms the status. The account owner checks any open question with them before anything is sent.

## What they supply

- **The change record.** What the change does and does not do, the status of each part left out, who gets it and from when, what may be shared, any workaround and guide, and what must not be mentioned, with the name of the role that confirmed it.
- **The feedback export.** One row per request, with its link to the change, the requester and the account owner.
- **The contact preferences export.** Each person's preferred channel, whether they have asked not to be contacted, and any timing notes.
- **The run settings.** The account owner, today's date and the responsible team.
- **Style notes,** if you have them: sign-off, tone and words you avoid.

## What comes out

A single draft for the account owner, in a fixed order:

1. **The status to verify,** restated from the change record, with any question the record leaves open.
2. **The requesters,** one line per person: what they asked for and when, their status and the points it rests on, and how they will hear. Repeat requests from one person are merged.
3. **The draft updates,** one per person, each in their channel, each ending with a check that traces every date and feature it mentions.
4. **The held requests,** with the reason: account owner first, not to be contacted, requester to confirm, status unclear.
5. **Possible matches** not linked to the change, requests on other owners' accounts, and the requests a person marks as updated after sending.

See the worked example with invented data in [EXAMPLE.md](EXAMPLE.md).

## Where it fits

- [Customer success and account management](https://fullypowered.ai/functions/customer-success-and-account-management/), where the account owner closes the loop with the customers they look after.
- [Product management](https://fullypowered.ai/functions/product-management/), which confirms what shipped, what is still open and what may be shared.
- [Software technology](https://fullypowered.ai/industries/software-technology/), where feature requests are tracked against a product and customers watch for what changes.
- [Professional services](https://fullypowered.ai/industries/professional-services/), where clients ask for changes to a portal, a report or a way of working.
- [Marketing and advertising](https://fullypowered.ai/industries/marketing-and-advertising/), where an agency's clients ask for changes to reporting and dashboards.
- [Growth & scaling](https://fullypowered.ai/situations/growth-and-scaling/), when requests outnumber the account owner's memory of who asked for what.
- [Established businesses](https://fullypowered.ai/situations/established-businesses/), where a long feedback backlog has customers who have never heard back.

It sits between two other capabilities. [Customer feedback themes](https://fullypowered.ai/capabilities/customer-feedback-themes/) finds what customers keep asking for; [Customer satisfaction detractor follow-up](https://fullypowered.ai/capabilities/customer-satisfaction-detractor-follow-up/) follows up low scores. This one answers each person who asked once a change or decision lands.

## What has to change for your company

- **Your columns.** Map your feedback tool's and contact list's headers to the defaults once; the capability stops and asks when a header does not match.
- **The change record.** Agree who on the product or service team fills it in and confirms it, and where it is kept.
- **Your status words,** if you already use others with customers.
- **The words that hold a request** for the account owner, such as your own terms for escalations.
- **Channels and tone.** Message lengths, sign-off, and whether two people at one account get one combined update.
- **Your platform.** It runs in ChatGPT, Claude, Copilot or Gemini, from files you supply; it needs no connection to your feedback tool.

## What has been checked

Fully Powered AI wrote this capability template from its own published map of the work. It was editorially reviewed on 10 November 2026. It was tried on its invented example in Claude on 10 November 2026 in two runs; the record of the second, made on the instructions as revised after the first, is published with it. It has not yet been tested in a client environment. It has not yet been tested as a packaged version in ChatGPT, Claude, Copilot or Gemini.

Testing in your environment means running it on a change your team shipped recently, with hard cases written in advance: a person who asked twice, a customer who has opted out, a request tied to a renewal, an internal target date in the record, an export with a renamed column. The account owner checks every draft against the change record before anyone relies on it. [Pilot acceptance-test preparation](https://fullypowered.ai/capabilities/pilot-acceptance-test-preparation/) builds that test set, and [What we test before we call an AI workflow ready](https://fullypowered.ai/insights/what-we-test-before-a-workflow-is-ready/) shows the record.

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

- [Customer feedback themes](https://fullypowered.ai/capabilities/customer-feedback-themes/)
- [Customer satisfaction detractor follow-up](https://fullypowered.ai/capabilities/customer-satisfaction-detractor-follow-up/)
- [Client-status update preparation](../client-status-update-preparation/)

## Make it yours

This is the starting version. Fully Powered AI adapts capabilities to how your company works, proves them on real work and rolls them out to the roles that use them. [Talk with us](https://fullypowered.ai/contact/).
