# Renewal risk review

Once a month, the account manager sees every contract coming up for renewal on one page: the dates that matter, the warning signs your organization watches for, which accounts are at risk, and the next step for each with an owner and a date. A person decides and makes every contact.

*Workflow template · Customer success and account management · version 0.1.0 · [Workflows Directory](https://fullypowered.ai/workflows/renewal-risk-review/)*

## The outcome

No renewal arrives as a surprise. Every contract ending in the next four months sits on one page, sorted by the date that matters most: the last day the customer can give notice, or the contract end when there is no notice date. Each account carries a start-by date, so a conversation that should have opened last month shows up as late instead of quietly slipping.

Each account gets one of three verdicts, at risk, watch or steady, and every verdict shows the evidence behind it. The warning signs are your own: the ones your team has learned to take seriously, such as a customer who has gone quiet, a new decision-maker or an open complaint. Each at-risk account leaves the page with its next steps, each owned by one person and due on a date.

The account manager and their lead still run every renewal. The AI assistant prepares the page; it contacts no customer, changes no record and sets no price.

## Who starts the work, and when

The account manager, the head of customer success or the owner of a smaller company runs it once a month, usually in the first week, from that day's export of the contract list. The head of customer success, or whoever leads the accounts, reviews the page and agrees the next steps with each account owner before anyone acts on them.

## What they supply

- **The contract list,** exported from the CRM, the billing system or a spreadsheet: each account, its owner, the contract end, the notice date, how it renews, its annual value, and the fields your team uses for warning signs, such as last contact and open issues.
- **Your warning signs and next steps.** Which signs count, how they turn into a verdict, and the usual next step for each. A starter set is included for teams that have not written theirs down yet, and the page says when it was used.
- **Account owners' notes,** where they have them: something a customer said, a budget review, a new contact.
- **Last month's review,** so the page shows what moved and which next steps were never reported done.
- **The settings:** the run date, how far ahead to look, and how many days before the deadline a renewal conversation should start.

## What comes out

One page in a fixed order. At the top, the totals: how many accounts renew in the window and the annual value at risk, on watch and steady. Then the at-risk accounts, each with its dates, its warning signs and the evidence for each, and its next steps. Then the accounts on watch, the steady ones, and a calendar of every deadline in date order.

After the calendar come the expansion signs for each owner to consider, the gaps in the contract list written as questions for whoever keeps it, and what changed since last month. A blank field is shown as unknown, never treated as good news.

See the worked example with invented data in [EXAMPLE.md](EXAMPLE.md).

## Where it fits

- [Customer success and account management](https://fullypowered.ai/functions/customer-success-and-account-management/), which owns the renewal and the relationship behind it.
- [Sales](https://fullypowered.ai/functions/sales/), where account managers carry renewals alongside new business.
- [Software technology](https://fullypowered.ai/industries/software-technology/), where subscriptions renew every year and many renew automatically.
- [Professional services](https://fullypowered.ai/industries/professional-services/), where retainers and service agreements come up on fixed dates.
- [Marketing and advertising](https://fullypowered.ai/industries/marketing-and-advertising/), where an agency's retainers are its revenue and a quiet client is the first warning.
- [Established businesses](https://fullypowered.ai/situations/established-businesses/), where renewals have run on one person's memory and a calendar reminder.

## What has to change for your company

Write down your warning signs: which fields show them, and how many it takes to call an account at risk. Name the usual next step for each sign and who owns it. Set how far ahead to look, and how many days before the notice date a renewal conversation should start. Match the column names in your export to the ones the template expects, once. Name who reviews the page and who keeps the contract list. It runs in ChatGPT, Claude, Copilot or Gemini from the files you supply; it needs no connection to your CRM.

## What has been checked

Fully Powered AI wrote this workflow template. It was editorially reviewed on 9 November 2026. It was tried on its invented example on 9 November 2026 in two runs and a shorter check of its starter warning signs: the instructions were revised after the first run, and the record of the second, a blind run, is published with it. Its verdicts, dates, next steps and totals matched the example, with small departures from the page layout that the record lists. The instructions were tightened after that run, and the record says how. It has not yet been tested in a client environment. It has not yet been tested as a packaged version in ChatGPT, Claude, Copilot or Gemini.

Testing in your environment means running it on two or three past months whose renewals your team already knows the outcome of, plus hard cases written in advance: a notice date after the contract end, a blank warning-sign field, a customer who has already given notice. The head of customer success checks every date and verdict against the contract list before anyone acts. [Pilot acceptance-test preparation](https://fullypowered.ai/workflows/pilot-acceptance-test-preparation/) builds that test set, and [what we test before we call an AI workflow ready](https://fullypowered.ai/insights/what-we-test-before-a-workflow-is-ready/) describes the record we keep.

- Written by Fully Powered AI.
- Sources and rights reviewed.
- Editorially reviewed on 9 November 2026.
- Package format checked by script on every release.
- Tried once on its invented example in Claude on 9 November 2026. The record is in [TRIAL.md](TRIAL.md).
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

- [Account handoff](../account-handoff/)
- [Client-status update preparation](../client-status-update-preparation/)
- [Stalled-deal review](https://fullypowered.ai/workflows/stalled-deal-review/)

## Make it yours

This is the starting version. Fully Powered AI adapts workflow templates to how your company works, proves them on real work and rolls them out to the roles that use them. [Talk with us](https://fullypowered.ai/contact/).
