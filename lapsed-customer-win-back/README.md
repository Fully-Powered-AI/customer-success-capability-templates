# Lapsed-customer win-back

Once a month, the owner or account manager sees which regular customers have gone far longer than usual without ordering, ranked by what each bought in their last active year, with open complaints set aside for a call and a short note drafted for the rest, using only approved offers. A person approves every note.

*Workflow template · Customer success and account management · version 0.1.0 · [Workflows Directory](https://fullypowered.ai/workflows/lapsed-customer-win-back/)*

## The outcome

Good customers stop drifting away unnoticed. The yardstick is each customer's own habit: a café that orders every fortnight is flagged after a few quiet weeks, while a salon that restocks once a quarter is left alone until its pause is genuinely long. Customers who are slipping but not yet lapsed are listed too, with the date they would cross the line, so the account team can act early.

The list puts the customers worth the most at the top. Anyone with an open complaint is pulled out first and handed to their account owner for a phone call, because a cheerful note on top of an unresolved problem makes things worse. Everyone else gets a short, personal draft that names their last order and asks an honest question before it offers anything.

Offers come only from the list you have approved, matched to each customer's value. The AI assistant prepares the list and the drafts; it sends nothing, contacts no customer and changes no record. A person reads, edits and approves each note.

## Who starts the work, and when

The owner, an account manager or a sales coordinator runs it once a month, from that day's export of the order history and the customer list. The owner or head of accounts reviews the list, crosses off anyone the business should not write to, and approves each note before its account owner sends it.

## What they supply

- **The order history,** exported from the store, the order system or the accounting software: each order's customer, date, value, status and what was in it.
- **The customer list:** each customer's contact, account owner, and whether they may be contacted.
- **Open issues:** complaints, refund requests, disputes, poor reviews and support tickets, open or recently closed.
- **The win-back log,** so nobody receives a second note too soon.
- **Your approved offers,** each with the customers it is for and how long it lasts. With none, every note is a simple check-in.
- **A few lines on your voice:** how you sign off and the words you never use.

## What comes out

One list in a fixed order. The header shows how every customer was sorted and the total value of those who have lapsed. Then the customers to call first, each with the open issue as written. Then the drafted notes in value order, each with the facts behind it, the offer chosen and why, anything to check before approving, and a line showing it is waiting for approval.

After the notes come the lapsed customers who were deliberately not written to and why, the customers slipping toward lapsed, those gone more than a year for the owner to decide on, those with too few orders to judge, and the gaps in the records as questions for whoever keeps the customer list.

This is about individual regular customers going quiet. For the pattern across everyone who left, [churn risk and save plan](https://fullypowered.ai/workflows/churn-risk-and-save-plan/) reads the reasons; for contracts coming up on a date, [renewal risk review](https://fullypowered.ai/workflows/renewal-risk-review/) works from the contract list.

See the worked example with invented data in [EXAMPLE.md](EXAMPLE.md).

## Where it fits

- [Customer success and account management](https://fullypowered.ai/functions/customer-success-and-account-management/), which owns keeping regular customers buying.
- [Sales](https://fullypowered.ai/functions/sales/), where account managers look after repeat trade accounts alongside new business.
- [E-commerce and retail](https://fullypowered.ai/industries/ecommerce-and-retail/), where repeat buyers of everyday goods are the heart of the business.
- [Consumer brands](https://fullypowered.ai/industries/consumer-brands/), where stockists and direct customers reorder on a rhythm you can read.
- [Manufacturing](https://fullypowered.ai/industries/manufacturing/), where trade customers restock on a pattern and a quiet account is lost revenue.
- [Established businesses](https://fullypowered.ai/situations/established-businesses/), where years of customers sit in the order history and nobody has time to notice who stopped.

## What has to change for your company

Decide how long a pause counts as lapsed for your customers: the starting rule is more than twice their usual gap, and at least 30 days. Write down the offers you are willing to make, who each is for and how long it lasts, and whether an offer may appear in a first note at all. Name who approves the notes, who sends them and who handles complaints. Match your export's column names to the ones the template expects, once, and keep the win-back log up to date after each round. It runs in ChatGPT, Claude, Copilot or Gemini from the files you supply; it needs no connection to your store, CRM or mailbox.

## What has been checked

Fully Powered AI wrote this workflow template. It was editorially reviewed on 10 November 2026. It was tried on its invented example on 10 November 2026 in two runs; the record of the second is published with it. It has not yet been tested in a client environment. It has not yet been tested as a packaged version in ChatGPT, Claude, Copilot or Gemini.

Testing in your environment means running it on a past month whose customers your account team knows well, plus hard cases written in advance: a quarterly buyer who is only a little late, a lapsed customer with an open complaint, a customer who asked not to be contacted, order dates that all fall on the day the records were loaded. The owner checks every figure and every draft against the records before anything is sent. [Pilot acceptance-test preparation](https://fullypowered.ai/workflows/pilot-acceptance-test-preparation/) builds that test set, and [what we test before we call an AI workflow ready](https://fullypowered.ai/insights/what-we-test-before-a-workflow-is-ready/) describes the record we keep.

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
- [Complaint and refund request handling](https://fullypowered.ai/workflows/complaint-and-refund-request-handling/)

## Make it yours

This is the starting version. Fully Powered AI adapts workflow templates to how your company works, proves them on real work and rolls them out to the roles that use them. [Talk with us](https://fullypowered.ai/contact/).
