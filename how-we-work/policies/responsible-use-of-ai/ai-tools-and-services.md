---
description: The use of AI tools and Services within SixPivot.
---

# AI Tools and Services

**Last Updated:** August, 2026

AI tools and models change quickly. This page provides practical guidance on the tools and services we use at SixPivot and how to decide whether they're appropriate for the work you're doing.

Being able to access a tool doesn't automatically make every use of it appropriate.

Our [Responsible Use of AI](https://chatgpt.com/) policy describes the principles that apply whenever we use AI. This page focuses on choosing and configuring the services we use.

## Think about the whole service

When we talk about an AI tool, there may be several services involved in processing the request.

For example, a coding tool might use one provider for one model and another provider for a different model.

Think about the complete path:

> **Tool → Provider → Model**

The model you select doesn't necessarily tell you who is processing your information or where that processing happens.

Similarly, using an approved tool doesn't mean every provider, model, plugin or integration available through it is automatically appropriate.

## SixPivot and client use are different

A tool that is suitable for SixPivot work isn't automatically suitable for client work.

Before using AI with client information, understand any requirements the client has around:

* approved AI tools and providers;
* data residency or sovereignty;
* source code and intellectual property;
* personal or sensitive information;
* model training and data retention; and
* external integrations or services.

Where a client provides their own AI environment, such as Microsoft 365 Copilot, GitHub Copilot or another managed service, prefer that environment where appropriate.

If a client restricts AI use, their requirements take precedence for their information and systems.

### Use the right account

The account you use can materially change the privacy and security characteristics of an AI service.

Consumer, individual, business and enterprise versions of the same product may have different terms covering data retention, model training, administration, governance and security.

For SixPivot work, use your SixPivot account or an approved SixPivot service where one is available.

For client work, use the account or environment agreed for the engagement.

Avoid using personal AI accounts with SixPivot or client confidential information.

## Privacy and training

Understand what happens to information you provide to an AI service.

In particular, consider whether:

* prompts and responses are retained;
* uploaded files are retained;
* information may be used to train or improve models;
* conversation history or memory is enabled;
* codebases are indexed or uploaded;
* administrators can control retention and access; and
* privacy or zero-data-retention options are available.

Don't assume that selecting a different model inside the same application leaves these characteristics unchanged.

## Data sovereignty

Where information is processed can matter just as much as who processes it.

A model developed in one country might be hosted by a provider in another or run entirely on your own machine.

Conversely, selecting a familiar model through a third-party provider may result in information being processed somewhere you didn't expect.

For work with residency or sovereignty requirements, confirm where processing occurs rather than inferring it from the model or tool.

If you can't establish where client information will be processed, don't send client information to that service until you have clarified whether its use is appropriate.

## Choosing a model

Use a model appropriate for the work rather than automatically choosing the most capable model available.

Smaller and faster models are often suitable for straightforward tasks such as:

* simple transformations;
* summarisation;
* classification;
* routine code changes;
* generating boilerplate; and
* high-volume automated work.

More capable models may be appropriate for complex reasoning, difficult engineering problems, architecture or tasks where getting a high-quality result quickly is more valuable than minimising the cost of an individual request.

The cheapest model isn't always the cheapest way to solve a problem. Repeated retries, poor output or additional engineering time can easily outweigh the difference in model cost.

> **Use the model that gets the job done effectively, not simply the cheapest or most capable model available.**

## Context has a cost

Model selection isn't the only thing that determines cost.

Large prompts, long conversations, repository-wide context, uploaded documents. skills, plugins and agents and agentic workflows can result in significantly more information being processed than expected.

Be conscious of tools that repeatedly send large amounts of context with every request.

This matters particularly when building automated systems. A small inefficiency repeated thousands of times can become expensive.

Where appropriate:

* provide only the context needed for the task;
* avoid repeatedly processing information that hasn't changed;
* use smaller models for simpler stages of a workflow;
* complete smaller tasks in a session, or&#x20;
* use an orchestrator session to create specs and a seperate clean session to do the work;
* cache or reuse results where appropriate; and
* put sensible limits around automated model usage.

Cost optimisation shouldn't come at the expense of producing a reliable result.

## Local models

Running a model locally can be useful where privacy, experimentation, latency, offline operation or cost makes it appropriate.

A genuinely local model can also provide a strong data boundary because prompts and responses don't need to leave the device.

However, don't assume that a tool described as "local" keeps everything local or that Client's automatically approve the use of local models.

The surrounding application may still use external services for things such as:

* authentication;
* telemetry;
* embeddings or indexing;
* web search;
* model routing; or
* other connected features.

Apply the same **Tool → Provider → Model** thinking to local AI as you would to a hosted service.

Local models also remain subject to client requirements. Keeping data on your laptop doesn't automatically make its use permitted.

## Supported tools

SixPivot supports a range of AI tools and we expect this list to change over time.

Rather than treating a product name as blanket approval, consider the account, provider, model and information involved.

Always review the service Terms of Service, Privacy Policy and any data-retention/security policies.

### ChatGPT

**Privacy:** [Training Optout](https://help.openai.com/en/articles/8983130-what-if-i-want-to-keep-my-history-on-but-disable-model-training) (last checked: August, 2026)

> With ChatGPT Business, ChatGPT Enterprise, ChatGPT Edu and our API Platform offerings, by default, we don’t use provided inputs and outputs to train our models. Please see our[ Enterprise Privacy page](https://openai.com/enterprise-privacy) for information on how we handle business data.\
> \
> If you are on a ChatGPT Plus, ChatGPT Pro or ChatGPT Free plan on a personal workspace, data sharing is enabled for you by default, however, you can opt out of using the data for training. To do so, please navigate to _Your Profile > Settings > Data Controls > Improve the model for everyone > Switch off the toggle._ Once you opt out,\* new \*conversations will not be used to train our models. As a separate control, this can also be applied to Voice mode.

Suitable for general AI-assisted work when used through an appropriate SixPivot account and in accordance with the requirements of the engagement.

Be conscious of the information being provided, enabled integrations and any persistent features such as projects or memory.

### Claude

**Privacy:** [Data Usage Policy](https://code.claude.com/docs/en/data-usage) (last checked: August, 2026)

> **Consumer users (Free, Pro, and Max plans)**: We give you the choice to allow your data to be used to improve future Claude models. We will train new models using data from Free, Pro, and Max accounts when this setting is on (including when you use Claude Code from these accounts).
>
> **Commercial users**: (Team and Enterprise plans, API, 3rd-party platforms, and Claude Gov) maintain existing policies: Anthropic does not train generative models using code or prompts sent to Claude Code under commercial terms, unless the customer has chosen to provide their data to us for model improvement (for example, the [Developer Partner Program](https://support.claude.com/en/articles/11174108-about-the-development-partner-program)).

Suitable for general AI-assisted work and more complex reasoning when used through an appropriate account.

[Claude Code](https://code.claude.com/docs/en/overview) is also commonly used for software development. Because it can interact directly with a development environment, the additional guidance in **AI-Assisted Software Development** and **Agents and Connected AI** applies.

### GitHub Copilot

**Privacy:** [Data Usage & Training Policy](https://docs.github.com/en/copilot/how-tos/manage-your-account/manage-policies#model-training-and-improvements) (last checked: August, 2026)

> Starting on April 24, 2026, if you have a **Copilot Free**, **Copilot Pro**, **Copilot Pro+**, or **Copilot Max** plan, GitHub may use your interactions with GitHub features and services—including inputs, outputs, code snippets, and associated context—to train and improve AI models. This change allows us to build more intelligent, context-aware coding assistance based on real-world development patterns. You can opt-out from allowing your data to be used for training in your personal settings for GitHub Copilot. For information about how we use and share data, see our [Privacy Statement](https://docs.github.com/en/site-policy/privacy-policies/github-general-privacy-statement).

Suitable for AI-assisted software development where its use is permitted for the project.

For client repositories, ensure the account and configuration being used are appropriate for that client.

### Cursor

**Privacy:** [Data Use Policy](https://cursor.com/data-use) (last checked: August, 2026)

> * If you enable “[Privacy Mode](https://cursor.com/help/security-and-privacy/privacy#how-do-i-enable-privacy-mode)” in Cursor’s settings: Customer Data will not be used for training by Cursor. Cursor maintains zero data retention (ZDR) agreements with all providers, and AI model providers will not store or train on your data. However, please note that subject to their policies, model providers (including Cursor) may run risk classifiers to detect violations of terms and usage policies, and if your prompts or conversations trigger abuse detectors your data may be stored for investigation and deleted in accordance with their retention policies. Non-ZDR models will be designated as such or require an admin to opt-in to enable the model for your workspace. See documentation from [SpaceXAI](https://x.ai/legal/faq-enterprise), [OpenAI](https://developers.openai.com/api/docs/guides/your-data#default-usage-policies-by-endpoint) and [Anthropic](https://privacy.claude.com/en/articles/7996866-how-long-do-you-store-my-organization-s-data) for more details about their retention policies.
> * If you choose to turn off “Privacy Mode”: we may use and store codebase data, prompts, editor actions, code snippets, and other code data and actions to improve our AI features and train our models. Some of our inference providers may temporarily access and store model inputs and outputs to improve our inference performance; this data is deleted after use.

Suitable for AI-assisted software development where its use is permitted for the project.

Cursor can work with different models and providers and may process repository context as part of providing its features. Selecting an appropriate provider and privacy configuration is therefore as important as selecting the model itself.

### JetBrains Junie

**Privacy:** [Data Collection Policy](https://www.jetbrains.com/help/ai-assistant/settings-reference-data-sharing.html) (last checked: August, 2026)

> When you use AI features, AI Assistant needs to send your requests and pieces of your code to the LLM ([Large Language Model](https://en.wikipedia.org/wiki/Large_language_model)) provider. Besides the prompts you type, it may send additional details, such as file types, frameworks used, and any other information that may be necessary for providing context to the LLM.
>
> ...
>
> The option that controls detailed data collection can be found in the IDE Settings under Settings | Appearance & Behavior | System Settings | Data Sharing | Send detailed code-related data and is disabled by default.

Suitable for AI-assisted software development when its use is permitted for the project.

Junie operates as an agent within JetBrains development environments and can inspect project context, modify files, run commands and execute tests as part of completing a task.

As with other agentic development tools, consider the environment and information Junie has access to, not just the prompt you provide. Ensure the models and providers configured for use are appropriate for SixPivot or the client engagement.

### Microsoft 365 Copilot

**Privacy:** [Data, Privacy & Security Policy](https://learn.microsoft.com/en-us/microsoft-365/copilot/microsoft-365-copilot-privacy) (last checked: August, 2026)

> When you enter prompts using Microsoft 365 Copilot, the information contained within your prompts, the data they retrieve, and the generated responses are processed and stored in alignment with contractual commitments with your organization's other content in Microsoft 365.
>
> ....
>
> Microsoft 365 Copilot is upholding data residency commitments as outlined in the Microsoft Product Terms and Data Protection Addendum. Microsoft 365 Copilot was added as a covered workload in the data residency commitments in Microsoft Product Terms on March 1, 2024.

Suitable for working with information already within an appropriately managed Microsoft 365 environment.

When provided by a client, use it within the boundaries and permissions of their environment.

## Other tools and models

We're technologists. We expect people to experiment with new models, providers and tools rather than limiting themselves to a static list.

Before using a new service with SixPivot or client information, apply the principles in our [Responsible Use of AI](./) policy.

In particular, understand:

1. **what the tool can access;**
2. **who is providing the model;**
3. **where the information is processed;**
4. **what happens to the information afterwards;** and
5. **whether the information you're providing is appropriate for that service.**

Experimenting with public, synthetic or otherwise non-sensitive information is very different from giving a new service access to a client repository.

When you're unsure, ask before introducing sensitive information. The PLT is always  there to help.

## Keep configurations intentional

AI tools increasingly accumulate capabilities over time.

You might start with a coding assistant and later add filesystem access, MCP servers, GitHub integration, browser access or another model provider.

Periodically review what you've enabled and remove integrations, credentials and providers you no longer use.

This is particularly important when moving between client engagements.

## In short

**Don't judge an AI service by its product name alone.**

Understand the tool, provider, model involved & the data/security/residency policies.

**Use the right environment.**

Use SixPivot accounts for SixPivot work and the agreed environment for client work.

**Know where the data goes.**

Privacy, retention and data sovereignty can differ between providers and account types.

**Choose models deliberately.**

Use capability and cost appropriate to the task rather than defaulting to the largest model.

**Experiment safely.**

We're encouraged to explore new AI technology. Start with non-sensitive information and understand the service before trusting it with SixPivot or client data.
