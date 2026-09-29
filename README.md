# B2B Cold Outreach Campaign Prep with Email Awesome Verification | Agent Skill

A reviewable campaign brief, reconciled contact list, message narrative, and proposed touches by channel before any email is sent.

This public Agent Skill addresses **b2b cold outreach campaign** with Email Awesome email verification where the job requires it. It is an independent use-case package, not an MCP or a claim that the product has completed an authenticated task.

**Product role:** Email Awesome is the verification and row-reconciliation step before this deliverable is marked verified. Without an authorized account and final observed results, the agent may prepare the brief or file but must label verification pending.

## What you can ask an agent to do

> Prepare a cold outreach campaign for SaaS operations leaders using my 120-contact CSV and this case study. Verify addresses, split into two segments, and draft the first email plus two follow-up angles.

**Example result (illustrative, not a live run):** Campaign pack: 120 source rows; 91 VALID, 8 INVALID, 9 CATCH_ALL, 7 UNKNOWN, 5 unresolved. Two segments and three draft touches per segment. No messages sent. Claims that lack support in the supplied case study are flagged for review.

## Install

```bash
npx skills add EmailAwesome/emailawesome-b2b-cold-outreach-skill --skill b2b-cold-outreach-campaign
```

Or copy this prompt into an agent that supports skill installation:

> Install the `b2b-cold-outreach-campaign` skill from https://github.com/EmailAwesome/emailawesome-b2b-cold-outreach-skill and use it to help with: [describe your task]. Confirm installation, ask for my authorized inputs, and show me the proposed output before any external action.

Read the [skill instructions](skills/b2b-cold-outreach-campaign/SKILL.md). The agent needs compatible tools and access to your authenticated account to operate Email Awesome; installation alone does not provide that access.

## Scope and trust

- **Input:** A user-supplied or authorized prospect list, offer, ICP, evidence about each segment, permitted channels, and target outcome.
- **Output:** A reviewable campaign brief, reconciled contact list, message narrative, and proposed touches by channel before any email is sent.
- **Product:** [Email Awesome Cold Sales use case](https://www.emailawesome.com/use-cases) and the [main product skill](https://github.com/EmailAwesome/emailawesome-email-verification-agent-skills).
- **Current verification:** skill format and installation discovery are tested locally. An authenticated live product run has not yet been demonstrated for this repository.

The skill does not authorize purchases, scraping behind access controls, email sending, CRM writes, or publication. Third-party sites and product interfaces can change; the agent must observe the current state and report uncertainty.

## Access and privacy

The user must have authority to process and submit each list and to share any client deliverable. A verified address does not establish consent or permission to contact. Sender rules vary by jurisdiction; see the [FTC CAN-SPAM guide](https://www.ftc.gov/business-guidance/resources/can-spam-act-compliance-guide-business) and [ICO B2B marketing guidance](https://ico.org.uk/for-organisations/direct-marketing-and-privacy-and-electronic-communications/business-to-business-marketing/). Keep contact data and credentials out of this public repository and issues.

## Review checklist

1. Does the agent request the right inputs and distinguish this job from the other use cases?
2. Does it make the product step observable and avoid inventing results?
3. Does the output preserve source rows/URLs, time, uncertainty, and a clear decision for the user?

Feedback and improvements can be filed as a GitHub issue in this repository.
