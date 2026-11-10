# Expansion whitespace review

For one account or a whole book, the account manager sees what each customer holds against what it could also use, the evidence for every gap, the plays ranked, and one next step and owner for each. A person decides what to propose; nothing goes into the sales system without approval.

*Capability template · Customer success and account management · version 0.1.0 · [Capabilities Directory](https://fullypowered.ai/capabilities/expansion-whitespace-review/)*

## The outcome

Growth from existing customers stops depending on who happens to remember what. For each account, the page lays what the customer already holds beside everything else on your own offer list it could use, across four directions: offers it has never bought, teams that do not use what a neighbouring team uses, sites still missing an add-on, and licences close to their limit.

A gap only becomes a play when something on record backs it: the customer asked, the customer described the need, usage is near the limit, or the customer's structure shows the team or site. Every play shows that evidence with its source, an estimated value from your own catalogue, and a score for evidence, size and how well you know the people involved. The plays arrive ranked, each with whom to approach, what to raise, a result the customer has already reported where there is one, and one next step with an owner and a date. Gaps with nothing behind them are kept apart, each with the signal that would make them worth raising.

New customers still settling in, and accounts whose renewal is at risk, have their plays held back rather than pushed. The account manager and their lead decide what to propose and when. The AI assistant prepares the page; it contacts no customer, sets no price and creates nothing in the sales system.

## Who starts the work, and when

The account manager or the customer success lead starts it once a quarter across their book, before an account planning meeting, or for one large account in depth. The head of customer success, or whoever leads the accounts, reviews the page, agrees the next steps with each account owner and approves any proposal or sales-system record before anyone acts on it.

## What they supply

- **Your offer catalogue:** each offer, whether it is priced per user, per site or per account, its typical annual value, and which teams it suits or what an account must have for a higher tier.
- **The holdings export** from the sales system or billing: what each account holds, where, how many against its limit, and since when.
- **Where they have them:** each customer's teams and sites, the contacts you know there and how well, each account's health from the last renewal review, and dated notes of what customers have asked for, described or reported.
- **The settings:** the run date, the account or book to review, and your own thresholds for usage, size and the hold on new customers. Defaults are included for teams that have not set theirs.

## What comes out

One page in a fixed order. At the top, the sources, the settings used and the counts: accounts reviewed, plays ranked, plays held and gaps with no evidence yet. For a book, a ranking of accounts by their best play comes next.

Then a section for each account: what it holds today, the whitespace map in four lines, the ranked plays with their evidence, estimate, score, approach and next step, the plays held and why, and the gaps with no evidence yet. After the accounts come the sales-system records proposed for the strong and moderate plays, written out for the head of customer success to approve and a person to create; the gaps in the export, written as questions for whoever keeps it; and any note that asked for something to be done, quoted and left undone.

See the worked example with invented data in [EXAMPLE.md](EXAMPLE.md).

## Where it fits

- [Customer success and account management](https://fullypowered.ai/functions/customer-success-and-account-management/), which owns the relationship and the growth of each account.
- [Sales](https://fullypowered.ai/functions/sales/), where account managers carry expansion targets alongside new business.
- [Software technology](https://fullypowered.ai/industries/software-technology/), where products are sold in seats, modules and tiers that customers grow into.
- [Professional services](https://fullypowered.ai/industries/professional-services/), where a client served by one practice or office could use the services of another.
- [Marketing and advertising](https://fullypowered.ai/industries/marketing-and-advertising/), where an agency serving one brand or region of a client could serve its others.
- [Growth & scaling](https://fullypowered.ai/situations/growth-and-scaling/), when growing existing customers is the cheaper way to reach the next target.
- [Established businesses](https://fullypowered.ai/situations/established-businesses/), where a long customer list holds more room to grow than anyone has mapped.

## What has to change for your company

Write your offer catalogue once: how each offer is priced, its typical annual value and what it suits. Decide which directions matter in your business, whether teams, sites, subsidiaries or volume. Set the usage threshold, the size bands that make a play large or small, and how long a new customer settles in before anyone raises more. Name who reviews the page, who approves a proposal and who keeps the sales system. Match the column names in your exports to the ones the template expects, once. It runs in ChatGPT, Claude, Copilot or Gemini from the files you supply; it needs no connection to your sales system.

## What has been checked

Fully Powered AI wrote this capability template. It was editorially reviewed on 10 November 2026. It was tried once on its invented example in Claude on 10 November 2026; the record of that run is published with it, and lists the clarifications made afterward that have not been run again, among them that only per-user offers are checked for volume. That run did not reach any stop condition. It has not yet been tested in a client environment. It has not yet been tested as a packaged version in ChatGPT, Claude, Copilot or Gemini.

Testing in your environment means running it on a past quarter's book whose expansion outcomes your team already knows, plus hard cases written in advance: an offer in the export that the catalogue lacks, licences near the limit with no number of new users on record, a customer still inside its first months, a note that asks for a record to be changed. The head of customer success checks every holding, estimate and score against the exports before anyone acts. [Pilot acceptance-test preparation](https://fullypowered.ai/capabilities/pilot-acceptance-test-preparation/) builds that test set, and [what we test before we call an AI workflow ready](https://fullypowered.ai/insights/what-we-test-before-a-workflow-is-ready/) describes the record we keep.

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

- [Renewal risk review](../renewal-risk-review/)
- [Quarterly business review preparation](../quarterly-business-review-preparation/)
- [Sales pipeline review](https://fullypowered.ai/capabilities/sales-pipeline-review/)

## Make it yours

This is the starting version. Fully Powered AI adapts capabilities to how your company works, proves them on real work and rolls them out to the roles that use them. [Talk with us](https://fullypowered.ai/contact/).
