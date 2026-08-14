---
description: How we use AI responsibly at SixPivot.
---

# Responsible Use of AI

## Why this exists

AI is part of how we work at SixPivot.

We encourage Pivots to explore and use AI where it helps us work more effectively, whether that's building software, researching a problem, analysing information, creating content or automating parts of our work.

With that capability comes responsibility.

Using AI can mean sharing information with another service, giving a tool access to a codebase or allowing an agent to take actions on our behalf. We need to understand those boundaries and make sensible decisions about what we give AI access to.

The principle is simple:

> **Know what information you're giving AI, where that information is going and what the AI is allowed to do.**

AI can help produce the work. It doesn't change who is responsible for it.

## Our approach to AI

We don't want Pivots to avoid AI because there is a policy around it. Quite the opposite.

We expect Pivots to understand and make appropriate use of the technology available to them. Experimentation and learning are an important part of keeping our skills current and understanding where AI genuinely helps.

At the same time, using AI doesn't lower our expectations around quality, security, privacy or professional judgement.

When using AI for SixPivot or client work:

* understand the tools and services you're using;
* consider what information you're providing them;
* respect client policies and confidentiality;
* use an appropriate account and environment for the work;
* consider the cost and effectiveness of how you're using AI;
* review and take responsibility for AI-assisted work; and
* ask when you're unsure.

Our [Cybersecurity Policy](../cybersecurity-policy.md) continues to apply when using AI.

For more practical guidance on choosing models, providers and tools, see [AI Tools and Services](ai-tools-and-services.md).

For engineering-specific guidance, see [AI-Assisted Software Development](ai-assisted-software-development.md).

## Think beyond the AI tool

It's easy to think about AI in terms of the application in front of you: ChatGPT, Claude, Cursor, Junie, Copilot or whatever comes next.

The actual path your information takes can be more complicated.

When evaluating AI use, think about three parts:

<figure><img src="../../../.gitbook/assets/image (31).png" alt=""><figcaption><p><strong>Model, Provider &#x26; Tool Example:</strong> Using Opus 5 with Claude Code with different providers may yield different outcomes.</p></figcaption></figure>

### Model

**What is actually processing the request?**

The model might be proprietary, open-weight, hosted remotely or running locally. Consider whether the model is appropriate for the work you're asking it to do.

### Provider

**Who is actually processing the information and where?**

The organisation that created a model isn't necessarily the organisation providing it to you.

The same model can be available through different providers, regions and hosting arrangements with very different privacy, security and data sovereignty implications.

Eg. Opus on Anthropic (US) vs Opus via Azure Foundry (AU)

### Tool

**What sits between you and the model and what can it see or do?**

A tool might send additional context, index a repository, access files, execute commands or connect to other systems.

Don't assume that choosing an appropriate model automatically makes the tool or provider appropriate.

{% hint style="info" %}
An approved _model_ doesn't make every provider appropriate.&#x20;

An approved _provider_ doesn't make every tool or integration appropriate.&#x20;

An approved _tool_ doesn't mean every type of data can be put into it.
{% endhint %}

Our [AI Tools and Services](ai-tools-and-services.md) guidance covers these considerations in more detail.

## Use the right model for the work <a href="#use-the-right-model-for-the-work" id="use-the-right-model-for-the-work"></a>

Bigger or more capable models aren't automatically the right choice for every task.

Consider the capability required, the amount of context being processed, how often the task will run and the cost of using the model.

Routine tasks may be better suited to smaller or faster models, while complex reasoning or particularly difficult engineering work may justify a more capable model.

This becomes especially important when building automated or agentic workflows where a decision made once can result in thousands of model calls.

We don't expect Pivots to optimise every prompt for cost. We do expect people to make sensible choices and avoid unnecessarily expensive use where a cheaper model or approach produces an equivalent outcome.

Eg. Using Fable to change the colour of a border is in-efficient, using Sonnet would work optimally.

## Think about the data

Across the Model, Provider and Tool, consider the information you're working with.

Be particularly careful with:

* client confidential information;
* source code and intellectual property;
* personal or sensitive information;
* production data;
* credentials, secrets and API keys;
* commercially sensitive SixPivot information; and
* information subject to regulatory or data sovereignty requirements.

Only provide AI systems with the information reasonably required for the task.

If you wouldn't be comfortable sharing the information with the provider under the applicable client and SixPivot arrangements, don't put it into the tool. When in doubt, as on our #ai Slack Channel or reach out to the PLT.

## Before using AI

For everyday use, we're created a helpful [AI Checklist](ai-checklist.md) to help.

## Client engagements

Our clients have different approaches to AI.

Some actively encourage its use. Others restrict particular models, providers, tools or types of information. Some may have specific data sovereignty, security, governance, residency or regulatory requirements.

When working with a client, their requirements for their systems and information take precedence.

Don't assume that because something is appropriate for SixPivot work it's automatically appropriate for client work.

It's important to review their AI Guidelines, AI Policies or AI Governance documents, if they don't have one, reach out and find out what they are.

We also have to appreciate and understand [Device Policy](https://handbook.sixpivot.com.au/~/revisions/Srsqj7Icjx72OqJmSZiY/how-we-work/policies/device-security-and-client-devices) and [Client Devices](https://handbook.sixpivot.com.au/~/revisions/Srsqj7Icjx72OqJmSZiY/how-we-work/policies/device-security-and-client-devices#when-a-client-gives-you-a-device) and their operating environments too.

### Before an engagement

Understand the client's expectations around AI before using it with their information.

Know:

* whether the client has an AI or acceptable-use or governance policy;
* which tools and services are permitted;
* whether particular providers or models are restricted;
* understand team or personal budgets, cost constraints or policies;
* what information can be processed by AI; and
* whether there are specific privacy, security or data sovereignty requirements.

Where the client provides their own AI environment, understand when you're expected to use it rather than a SixPivot service.

If the requirements aren't clear, ask or reach out to your PLT.

### During an engagement

Stay within the boundaries established for the engagement.

Use the appropriate accounts, tools and providers for the work.

If the way you're using AI materially changes, such as introducing a new provider, connecting another system or giving an agent additional capabilities, reconsider whether the new arrangement is still appropriate.

### When an engagement ends

Clean up client-specific AI resources that are no longer required.

Depending on how you've worked, this might include projects, uploaded files, persistent context, local data stores, credentials, connectors or client-specific configurations.

There may be legitimate reasons to retain information for ongoing support or other agreed purposes. Follow the arrangements for the engagement where this applies.

## You are responsible for the outcome

AI-assisted work is still our work.

Whether AI helped write code, analyse information, research a problem, create content or make a recommendation, you're responsible for deciding whether the result is appropriate to use.

Apply judgement according to the consequence of getting it wrong.

AI output can be incorrect, incomplete or misleading while appearing convincing. The more important the outcome, the more care we should take validating it.

For software development, see [AI-Assisted Software Development](ai-assisted-software-development.md).

## AI with access and agency

There is a difference between an AI that answers a question and one that can interact with your environment.

Agents, MCP servers, skills, agents, plugins and connectors can give AI access to files, source repositories, shells, databases, browsers, cloud environments and other systems.

As capability increases, agentic workflows increase, so does the importance of understanding what the AI can access and what it can do.

Our **Agents and Connected AI** guidance covers this in more detail.

## If something goes wrong

We're human, mistakes happen.

If you accidentally provide information to an inappropriate AI service, expose credentials, discover that information has been processed somewhere unexpected or believe an AI tool may have caused a security or privacy issue, raise it promptly.

Follow our [Cybersecurity Policy](../cybersecurity-policy.md) and any applicable client incident process.

Early reporting gives SixPivot and the client the best opportunity to understand what happened and manage any risk.

## In short

**Understand the path**

Think about the Model, Provider and Tool, not just the application in front of you.

**Protect the data**

Know what you're sharing and respect SixPivot and client requirements.

**Understand the capability**

Know what the AI can access and what it can do on your behalf.

**Use it effectively**

Choose models and approaches appropriate to the work and be conscious of unnecessary cost.

**Own the outcome**

AI can assist with our work, but responsibility for the result remains with us.

**When in doubt, ask**

If you're unsure whether a particular model, provider, tool or use of information is appropriate, find out before using it.
