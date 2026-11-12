# Cancellation request response

When a customer asks to cancel or cut back, the account manager gets one page: the request and the reason in the customer's words, the account's recent history, only the options your business already approved that fit that reason, and a reply that confirms the choice and what happens next. A person sends it.

*Workflow template · Customer success and account management · version 0.1.0 · [Workflows Directory](https://fullypowered.ai/workflows/cancellation-request-response/)*

## The outcome

Every customer who asks to leave gets a fast, clear, gracious answer, and your account manager writes it with the whole account in view. The page restates exactly what the customer asked for and from when, quotes the reason they gave, and lays out the account's recent story: plan changes, tickets, usage, any earlier request or open complaint.

If your business has an approved option that genuinely fits that reason, such as a smaller plan for a customer who mentions cost or a pause for one with a quiet season, it appears with the record that shows the account qualifies. Nothing is invented: no discount nobody approved, no deadline, no call the customer has to sit through first. When the customer is closing down, has said no to offers or has a dispute open, no option is shown at all.

The reply confirms the customer's choice in plain words, with the end date, fees, final invoice and data steps exactly as your service owner confirmed them. Any option sits in a separate paragraph the account manager may keep or delete, and the customer's request goes ahead either way. The AI assistant prepares; your account manager decides, edits and sends, and nothing changes on the account until the outcome is confirmed.

## Who starts the work, and when

The account manager who owns the account, or whoever handles cancellations, runs it the day a request arrives by email, form, chat or phone, before anyone replies. The service owner confirms the ending facts for the account first: when it would end, any fee, the last invoice and how the customer gets their data. The account manager decides which option to mention, if any, and confirms the outcome with the service owner before billing or access changes.

## What they supply

- **The request,** exactly as the customer sent it, or the note of the call, with its date.
- **The account record,** one row from your CRM or billing system: plan, fee, users, start date, billing, the account manager, the service owner and the contact preference.
- **The account history** for the last year: notes, tickets, billing notes and usage reports.
- **The ending facts** for this account, written or confirmed by the service owner.
- **Your approved options list:** each option in plain words, the reasons it fits, its conditions, who may offer it and until when.
- **A few settings,** such as the sign-off and who handles billing changes, data and disputes. Defaults are included.

## What comes out

One page in a fixed order: the request, the stated reason with its reason group, the account history, the ending facts as supplied, the options that fit and the ones left out with why, the reply draft with any optional paragraphs, what to confirm before sending, the steps for billing, support and the account record once the outcome is settled, and questions for named roles. Any note asking for a pressure tactic or an unapproved offer is quoted and not followed.

This handles one customer's request on the day it arrives. To read the pattern across everyone who left in a quarter, use [churn risk and save plan](https://fullypowered.ai/workflows/churn-risk-and-save-plan/); to prepare the month's renewals, use [renewal risk review](https://fullypowered.ai/workflows/renewal-risk-review/).

See the worked example with invented data in [EXAMPLE.md](EXAMPLE.md).

## Where it fits

- [Customer success and account management](https://fullypowered.ai/functions/customer-success-and-account-management/), which owns the account and the conversation about its future.
- [Customer support and service](https://fullypowered.ai/functions/customer-support-and-service/), where many cancellation requests first arrive and where access and data steps are carried out.
- [Software technology](https://fullypowered.ai/industries/software-technology/), where monthly plans, seats and tiers make cancelling and cutting back everyday requests.
- [Professional services](https://fullypowered.ai/industries/professional-services/), where a retainer that shrinks or ends deserves a considered reply from the person who knows the client.
- [Marketing and advertising](https://fullypowered.ai/industries/marketing-and-advertising/), where agency retainers are reduced or paused as clients' budgets and seasons change.
- [Established businesses](https://fullypowered.ai/situations/established-businesses/), where long-standing customers expect to be treated well on the way out.
- [Growth & scaling](https://fullypowered.ai/situations/growth-and-scaling/), when requests arrive faster than the senior account manager can answer each one.

## What has to change for your company

Write down your approved options, with the reasons each fits, its conditions, who may offer it and who approved it; if you have none, the workflow template shows none. Agree who confirms the ending facts for an account and how quickly, since every date and term in the reply comes from them. Use your own reason groups if your cancellation form already has a list. Name the roles for billing changes, access and data, and disputes. Match your export headers to the ones the template expects, once. It is written to run in ChatGPT, Claude, Copilot or Gemini from what you paste or upload; it needs no connection to your CRM or billing system.

## What has been checked

Fully Powered AI wrote this workflow template. It was editorially reviewed on 10 November 2026. It was tried on its invented example in Claude on 10 November 2026, a second time after earlier fixes, and the record of that run is published with it. The example's output was edited after the first run and the record was rewritten for the second run. No edit has been made since. It has not yet been tested in a client environment, and it has not yet been tested as a packaged version in ChatGPT, Claude, Copilot or Gemini.

Testing in your environment means running it on past requests your account team remembers well, plus hard cases written in advance: a customer closing down, one who says no offers, an option whose condition the records cannot show, a note asking for a deadline to be added. The account manager checks every date and term in the reply against the service owner's ending facts before anything is sent. [Pilot acceptance-test preparation](https://fullypowered.ai/workflows/pilot-acceptance-test-preparation/) builds that test set, and [what we test before we call an AI workflow ready](https://fullypowered.ai/insights/what-we-test-before-a-workflow-is-ready/) describes the record we keep.

- Written by Fully Powered AI.
- Sources and rights reviewed.
- Editorially reviewed on 10 November 2026.
- Package format checked by script on every release.
- Tried once on its invented example in Claude on 10 November 2026. The record is in [TRIAL.md](TRIAL.md).
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

- [Churn risk and save plan](../churn-risk-and-save-plan/)
- [Renewal risk review](../renewal-risk-review/)
- [Customer reply drafting](https://fullypowered.ai/workflows/customer-reply-drafting/)

## Make it yours

This is the starting version. Fully Powered AI adapts workflow templates to how your company works, proves them on real work and rolls them out to the roles that use them. [Talk with us](https://fullypowered.ai/contact/).
