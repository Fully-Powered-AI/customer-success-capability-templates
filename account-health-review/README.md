# Account health review across the book

Each week or month, the customer success lead sees which accounts in the book need attention, what changed since the last period and the evidence, judged by your own warning signs across usage, support, billing and relationship exports, and which accounts are missing data. A person decides who looks into each.

*Workflow template · Customer success and account management · version 0.1.0 · [Workflows Directory](https://fullypowered.ai/workflows/account-health-review/)*

## The outcome

The whole book comes into view in one sitting, not just the accounts someone happens to be worried about. Every account is checked against the same warning signs, the ones your team already trusts: usage falling against the last period, a jump in support tickets, an urgent ticket still open, an invoice long overdue, a customer nobody has spoken with in weeks, a main contact who has left. Each account that needs attention arrives with the signs it shows, this period's figure beside last period's, and the ticket, invoice or log entry behind it, so the lead can check any line against its source.

A drop your team already expects, such as a customer closed for refurbishment, is set apart rather than raised as a fresh alarm, and only when your own note says so. Gaps are as visible as signs: an account with no usage figures this period, or no contact ever recorded, is listed with the question that would close the gap, never quietly treated as healthy.

There is no health score and no colour. The workflow template adds nothing up, weighs no sign against another and predicts nothing. It lists what changed and the evidence, and leaves a blank beside each account for the lead's call: look into it or not, and who owns it. It contacts no customer and changes no record.

## Who starts the work, and when

The head of customer success runs it, or a customer success operations analyst runs it for them, once a period: weekly for a large book of smaller accounts, monthly for most. It starts when the period's exports are in. The head of customer success reads the page, decides which accounts need a closer look and assigns each to an owner before anyone acts.

## What they supply

- **The account list:** each account, its owner, its annual value and its renewal date.
- **The usage export:** one figure per account for each of the two periods, counting whatever your team treats as real use, such as bookings made, reports run or hours used.
- **The support export:** tickets with the dates they were opened and closed and their priority.
- **The billing export:** invoices with due dates, amounts and the date each was paid.
- **The relationship log:** calls, meetings, emails and contact changes, each marked as two-way or not.
- **Your warning signs:** each sign, the column it reads and the level that sets it off. A starter set is included for teams that have not written theirs down, and the page says when it was used.
- **Context notes,** where you have them: a closure, a known incident, a seasonal pattern you expect.
- **Last period's review,** so the page shows what is still flagged and which assignments were never reported done.

Each export has set column headings. When a heading the review needs is missing, the workflow template stops and asks which column holds it, and checks nothing until that is settled.

## What comes out

One page in a fixed order. At the top, the book in four groups with a count and annual value for each: needs attention, set apart, no sign found but data missing, and no sign found. Then each account needing attention, with its signs, the evidence for each, what is on file this period and a blank for the lead's call. Then the set-apart accounts with the note that explains them, every missing piece of data with the person to ask, and the accounts with no sign. It ends with what moved since the last review and any note that asked for something to be changed, quoted and left undone.

See the worked example with invented data in [EXAMPLE.md](EXAMPLE.md).

## Where it fits

- [Customer success and account management](https://fullypowered.ai/functions/customer-success-and-account-management/), which owns the health of every account between onboarding and renewal.
- [Software technology](https://fullypowered.ai/industries/software-technology/), where usage, tickets and invoices sit in three different systems and a falling usage count is often the first warning.
- [Professional services](https://fullypowered.ai/industries/professional-services/), where retained clients go quiet or stop paying on time long before they say anything.
- [Marketing and advertising](https://fullypowered.ai/industries/marketing-and-advertising/), where an agency's account leads need to know which retained clients have changed contacts or stopped answering.
- [Growth & scaling](https://fullypowered.ai/situations/growth-and-scaling/), when the book grows past what the team can keep in its head.
- [Established businesses](https://fullypowered.ai/situations/established-businesses/), where long-standing accounts are assumed healthy because nobody has looked.

## What has to change for your company

Write down your warning signs: the export and column each reads and the level that sets it off, such as how far usage must fall or how many days of silence count. Choose the usage figure that means real use for your product or service. Map your exports' column headings to the ones the workflow template expects, once. Decide the period, weekly or monthly, and how the needs-attention list is ordered; by default it runs largest annual value first. Name who keeps each export, so every gap goes to someone. It runs in ChatGPT, Claude, Copilot or Gemini from the files you supply; it needs no connection to your CRM, help desk or billing system and never asks for a password.

It looks at the whole book for change. Contracts coming up for renewal, with notice dates and next steps, are the [renewal risk review](https://fullypowered.ai/workflows/renewal-risk-review/); why customers have already left is the [churn risk and save plan](https://fullypowered.ai/workflows/churn-risk-and-save-plan/); regular customers who have stopped buying are [lapsed customer win-back](https://fullypowered.ai/workflows/lapsed-customer-win-back/).

## What has been checked

Fully Powered AI wrote this workflow template. It was editorially reviewed on 12 November 2026. It was tried once on its invented example on 12 November 2026, in Claude, and the record is published. It has not been tested in a client environment and has not been tested as a packaged version in ChatGPT, Claude, Copilot or Gemini.

Testing in your environment means running it on two or three past periods whose problem accounts your team already knows, with hard cases written in advance: an account missing from the usage export, a drop your context notes explain, a customer whose only recent contact was a newsletter, a note asking for a flag to be cleared. The head of customer success checks every sign against the exports before anyone acts. [Pilot acceptance-test preparation](https://fullypowered.ai/workflows/pilot-acceptance-test-preparation/) sets those cases up, and [what we test before we call an AI workflow ready](https://fullypowered.ai/insights/what-we-test-before-a-workflow-is-ready/) describes the record we keep.

- Written by Fully Powered AI.
- Sources and rights reviewed.
- Editorially reviewed on 12 November 2026.
- Package format checked by script on every release.
- Tried once on its invented example in Claude on 12 November 2026. The record is in [TRIAL.md](TRIAL.md).
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

- [Renewal risk review](../renewal-risk-review/)
- [Churn risk and save plan](../churn-risk-and-save-plan/)
- [Quarterly business review preparation](../quarterly-business-review-preparation/)

## Make it yours

This is the starting version. Fully Powered AI adapts workflow templates to how your company works, proves them on real work and rolls them out to the roles that use them. [Talk with us](https://fullypowered.ai/contact/).
