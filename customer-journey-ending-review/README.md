# Customer journey ending review

When a customer's journey ends on a sour note, your customer experience lead gets one review built from the records: whether the work was really finished at the final handoff, each difficult moment with its dates, the customer's own words, and follow-up options. The customer success lead chooses what to change.

*Workflow template · Customer success and account management · version 0.1.0 · [Workflows Directory](https://fullypowered.ai/workflows/customer-journey-ending-review/)*

## The outcome

The last weeks of a journey are often what a customer remembers and tells others about. This review takes one ending (an offboarding, a cancellation, a project close, a delivery, an onboarding milestone) and reads it from the records rather than from memory.

It starts with the ending itself. It checks the final handoff against what "done" meant for that customer, so a warm closing email never passes for finished work: if anything was still open, the review says so plainly and names the message that called the work complete. Then it walks back through the journey and finds the moments that were hard on the customer, from facts in the log: a question that waited too long for an answer, a customer who had to ask twice, a promised date that slipped, a long stretch with no word from the team. Each moment carries its dates and the number of days involved.

What the customer said is quoted exactly. What the customer may have felt is offered only as a reading, with the question or record that would confirm it. The review closes with options in three kinds: what could still be done for this customer, changes to test in the journey for the customers who come next, each with a count that would show whether it helped, and gaps in the records worth closing.

The customer success lead chooses which change to test and whether anyone contacts the customer. The AI assistant contacts no one, offers no money, judges no member of staff and changes no record.

## Who starts the work, and when

The customer experience lead or a customer success manager starts it after a journey's last planned handoff, when the ending deserves a closer look: a low close survey score, an unhappy exit comment, a complaint in the final weeks, a handoff that slipped, or a regular look at a few recent endings. It covers one customer's journey per run. The customer success lead reads the result and decides what happens next.

## What they supply

- **A short review brief:** the customer, the kind of journey, its start date, which logged item was the final handoff, the reason for the review, any limits on contacting the customer, and a few settings with defaults included.
- **The completion criteria:** what "done" meant for this journey, with the status of each at the end, the item that shows it and its owner.
- **The journey log:** an export of the messages, calls, meetings, deliveries and internal notes, with the thread, stage, direction and owner of each, plus any date the team promised.
- **The customer feedback:** survey scores, exit comments, emails and call notes about the journey.

Each export has default column headers. When a header does not match, the review stops and asks which column is which.

## What comes out

One review in a fixed order:

1. **How it ended:** the final handoff, a plain verdict on whether the work was finished and every question answered, each criterion with its evidence, any closing words that ran ahead of the work, low scores, and what has happened since.
2. **Difficult moments,** in date order, each with the facts, the dates and the days, and whether it touches unfinished work or the customer's feedback.
3. **The moments to look at first,** up to three, chosen by a fixed rule, with the moment nearer the ending first when two are level.
4. **In the customer's words,** quoted exactly, with call notes labelled as the note-taker's.
5. **Readings to confirm,** each with what would confirm or rule it out.
6. **Follow-up options** for this customer, changes to test in the journey, and changes to the records.
7. **Decisions for the customer success lead,** with "none" wherever one does not arise.

It reviews one journey after it ends. To answer a customer asking to leave today, use [Cancellation request response](https://fullypowered.ai/workflows/cancellation-request-response/); to read the pattern across everyone who left in a quarter, use [Churn risk and save plan](https://fullypowered.ai/workflows/churn-risk-and-save-plan/); to check a deliverable before it is handed over, use [Project handover readiness check](https://fullypowered.ai/workflows/project-handover-readiness-check/).

See the worked example with invented data in [EXAMPLE.md](EXAMPLE.md).

## Where it fits

- [Customer success and account management](https://fullypowered.ai/functions/customer-success-and-account-management/), where the customer experience owner looks after how customers are treated from the first week to the last.
- [Project and delivery](https://fullypowered.ai/functions/project-and-delivery/), where a project's close and final delivery are the handoff the customer judges the whole project by.
- [Software technology](https://fullypowered.ai/industries/software-technology/), where offboarding a customer at the end of a contract or plan is the last impression of the product and the team.
- [Professional services](https://fullypowered.ai/industries/professional-services/), where an engagement's close, the final deliverable and the last invoice decide whether a client comes back or refers others.
- [Marketing and advertising](https://fullypowered.ai/industries/marketing-and-advertising/), where an agency hands over a site, a campaign or an account and the client remembers how that handover felt.
- [Established businesses](https://fullypowered.ai/situations/established-businesses/), where long-standing customers expect a good ending, and a poor one travels.
- [Growth & scaling](https://fullypowered.ai/situations/growth-and-scaling/), when more journeys are ending each month than the customer experience lead can follow by hand.

## What has to change for your company

- **Your completion criteria.** Write down what "done" means for each kind of journey before it starts; the review reads the ending against them.
- **Your columns.** Map your CRM, help desk or project tool headers to the defaults once.
- **One thread per topic** in the log, so separate problems stay separate moments.
- **Your settings:** how many days a reply may take, how long a quiet spell may run, what counts as a low score, and how many journeys a change is measured on.
- **Who handles refunds, chargebacks and formal complaints,** so the review refers those to the right role and leaves them alone.
- **Your platform.** It runs in ChatGPT, Claude, Copilot or Gemini, from files you supply; it needs no connection to your systems.

## What has been checked

Fully Powered AI wrote this workflow template from its own published map of the work. It was editorially reviewed on 11 November 2026. It was tried once on its invented example in Claude on 11 November 2026, and the record of that run is published with it. Afterwards the wording of the instructions was clarified on several points the run raised, and the example was edited to drop one link that the instructions did not support and one phrase that went beyond the records; it was not run again after those edits. It has not yet been tested in a client environment. It has not yet been tested as a packaged version in ChatGPT, Claude, Copilot or Gemini.

Testing in your environment means running it on two or three endings your team remembers well, with hard cases written in advance: a closing message sent while work was open, a customer who asked twice, a call note that sounds like the customer's words, a feedback comment asking for a refund, an export with a renamed column. The review owner recomputes every day count from the log before anyone relies on the review. [Pilot acceptance-test preparation](https://fullypowered.ai/workflows/pilot-acceptance-test-preparation/) builds that test set, and [What we test before we call an AI workflow ready](https://fullypowered.ai/insights/what-we-test-before-a-workflow-is-ready/) shows the record.

- Written by Fully Powered AI.
- Sources and rights reviewed.
- Editorially reviewed on 11 November 2026.
- Package format checked by script on every release.
- Tried once on its invented example in Claude on 11 November 2026. The record is in [TRIAL.md](TRIAL.md).
- Not yet tested in a client environment.

## What is in this folder

- [TEMPLATE.md](TEMPLATE.md): the complete workflow template. Roles, inputs, the procedure, exceptions and stop conditions, the output format, a reviewer checklist, acceptance tests, the instructions for an AI assistant and what to customize.
- [EXAMPLE.md](EXAMPLE.md): a worked example with invented data.
- [TRIAL.md](TRIAL.md): what came out when the template was tried on its example.
- [SKILL.md](SKILL.md): the technical file, for AI products that load packaged instructions from a folder.
- [SOURCES.md](SOURCES.md): what the workflow template drew on, with licences.
- [LICENSE](LICENSE): MIT. Use it, change it, make it yours.

## Start using it

1. Read [EXAMPLE.md](EXAMPLE.md) to see what a good result looks like.
2. Open [TEMPLATE.md](TEMPLATE.md) and set every item under "What to customize" to your own rules, roles and limits.
3. Give your AI assistant the instruction block and the output format from the template, with your own limits in place of the ones the instructions leave open in square brackets. Paste them in as custom instructions in ChatGPT, Claude, Copilot or Gemini, or copy this whole folder into a product that loads `SKILL.md` packages. This folder stands alone; you do not need the rest of the repository.
4. Run it on past work first, using the reviewer checklist and acceptance tests in the template, before anyone relies on it.

## Related workflow templates

- [Cancellation request response](../cancellation-request-response/)
- [Churn risk and save plan](../churn-risk-and-save-plan/)
- [Project handover readiness check](https://fullypowered.ai/workflows/project-handover-readiness-check/)

## Make it yours

This is the starting version. Fully Powered AI adapts workflow templates to how your company works, proves them on real work and rolls them out to the roles that use them. [Talk with us](https://fullypowered.ai/contact/).
