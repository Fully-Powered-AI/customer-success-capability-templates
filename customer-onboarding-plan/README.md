# Customer onboarding plan

For every new customer, your customer success lead gets one plan for the first weeks: the result the customer must reach, the fewest milestones that get them there with an owner on each side, the promises both sides made, and each message as a draft. Nothing is sent until a person approves it.

*Workflow template · Customer success and account management · version 0.1.0 · [Workflows Directory](https://fullypowered.ai/workflows/customer-onboarding-plan/)*

## The outcome

Every new customer starts with a plan built around one moment: the first time their own person does the work they bought you for, on their own real work, without your help, and checks the result. The plan names that moment in the customer's words and dates it to the first real piece of their work that falls inside the onboarding window.

Between today and that moment sit only the milestones it needs, each written as something a person can be seen doing, with an owner at the customer and an owner on your side. Everything else that was sold still has a date, after first real use. Promises made at the sale and the kickoff are listed with who owes them and by when, so nothing said on a call is quietly lost.

Onboarding ends on the customer's own success: their person runs the work, the sponsor signs off, the customer keeps written notes, and the date of the next check is agreed before anyone leaves the call.

Your customer success lead still runs the onboarding. The AI assistant prepares the plan and the drafts; it sends nothing, contacts no one and changes no record.

## Who starts the work, and when

The customer success lead or onboarding manager starts it once the account handoff is done, ideally right after the kickoff call. They run it again during onboarding, usually before each weekly check-in, with the latest status, to see which milestones are done, which are late and what is stalling. The customer success lead approves the plan and every message before anything reaches the customer.

## What they supply

- **The account handoff record:** what was sold, what was promised, who is involved, the dates and the risks the seller heard.
- **Your facts:** a few lines on what you sell, your usual onboarding steps, what first real use means for this kind of customer, and words you never use with customers.
- **The kickoff notes,** when the kickoff has happened: the customer's goal in their own words and what each side said it would do.
- **The settings:** the start date, how long onboarding runs, the check-in day and how often the customer's work comes round.
- **For a progress run:** the approved plan and the latest status of each milestone.

## What comes out

One plan in a fixed order: the outcome and its date; what must be settled before the first milestone; the milestones to first real use, each with both owners, a date, what it waits on and what you will see when it is done; what was moved to after first real use; both sides' commitments; each message as a draft; the risks; anything asked for that was not sold; the check-ins, the closing session and the follow-up check.

On a progress run, each milestone is marked done by the customer, done with your help, not done or not reported, and anything stalling comes with its likely cause, the honest fix and an owner. A status nobody reported is a question, never assumed done.

See the worked example with invented data in [EXAMPLE.md](EXAMPLE.md).

## Where it fits

- [Customer success and account management](https://fullypowered.ai/functions/customer-success-and-account-management/), which owns the first weeks of every account and the renewal that follows them.
- [Software technology](https://fullypowered.ai/industries/software-technology/), where the first weeks decide whether a subscription is part of the customer's working week by renewal time.
- [Professional services](https://fullypowered.ai/industries/professional-services/), where a new client's first weeks set the working rhythm for the engagement.
- [Marketing and advertising](https://fullypowered.ai/industries/marketing-and-advertising/), where an agency's new retainer needs access, assets and approvals before any work can show.
- [Growth & scaling](https://fullypowered.ai/situations/growth-and-scaling/), when new customers arrive faster than one person can plan each start by hand.

## What has to change for your company

Write your facts once: your usual onboarding steps, who on your team owns each, which steps a customer gets only when bought, and what first real use means for each kind of customer you serve. Set the onboarding window, the check-in day and the number of milestones you allow before first real use. Decide which messages your team sends at each step and who approves them. Agree how your team records milestone status, and match its column names to the template once. It runs in ChatGPT, Claude, Copilot or Gemini from the files and notes you supply; it needs no connection to your CRM or your product.

## What has been checked

Fully Powered AI wrote this workflow template. It was editorially reviewed on 9 November 2026. It was tried on its invented example on 9 November 2026 in two runs. The first showed where the instructions left room to guess, such as how the window's last day is counted, whether a customer's data file comes before the first milestone or is the first milestone, and what to do with usual steps or sessions beyond what was sold; the instructions and the example were revised. The record of the second run is published with it: the plan held every section, the window, the settle-first item, the routing of unsold requests and the questions about seats and sessions came out as intended, and the record lists the small edits made afterward that have not been run again. The progress run, the check for a customer gone quiet and the list of reasons a customer stalls have not been tried. It has not yet been tested in a client environment. It has not yet been tested as a packaged version in ChatGPT, Claude, Copilot or Gemini.

Testing in your environment means running it on two or three customers whose onboarding your team remembers well, plus hard cases written in advance: a promise made only in an email, a kickoff request that was never sold, a customer who goes quiet in week two, a status sheet with a column the template does not know. Your customer success lead checks every date, owner and draft before anything goes out. [Pilot acceptance-test preparation](https://fullypowered.ai/workflows/pilot-acceptance-test-preparation/) builds that test set, and [what we test before we call an AI workflow ready](https://fullypowered.ai/insights/what-we-test-before-a-workflow-is-ready/) describes the record we keep.

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
- [Renewal risk review](../renewal-risk-review/)

## Make it yours

This is the starting version. Fully Powered AI adapts workflow templates to how your company works, proves them on real work and rolls them out to the roles that use them. [Talk with us](https://fullypowered.ai/contact/).
