---
description: Tools which have been approved for use with SixPivot and Client Data
---

# Approved AI Tools

## Approved Tools

The following AI tools are pre-approved for use by SixPivot employees. Please check with your PC on each project about appropriate use, as some clients may limit usage of such tools for their IP. In addition, you must turn off the ability for the vendor to retrain on your inputs (privacy mode).

* GitHub Copilot
* JetBrains AI (Junie)
* Cursor
* Claude Code
* ChatGPT
* Microsoft 365 Copilot

Available tooling will be continually re-assessed on a case-by-case basis. Raise requests in Slack in #ai-coding-tools

If you wish to test out free or trial version of these on your own, you may do so if the free or trial versions allow you to turn off retraining (privacy mode).

## Licensing

You may request a license for one AI tool of your choosing from SixPivot. If an engagement requires the use of additional tools, these will be provided as needed. Beyond these restrictions, you may use any other approved tools of your choosing at your own expense, provided you follow our AI-Assisted Software Development Policy and  Guidelines for AI Tools and AI Assisted Development.

## Privacy Mode/No-Retraining (as at 14/08/2025)

* **GitHub Copilot:** Training is off by default, manage data-use settings: [https://docs.github.com/en/copilot/managing-copilot/managing-copilot-as-an-individual-subscriber/managing-your-copilot-plan/managing-copilot-policies-as-an-individual-subscriber](https://docs.github.com/en/copilot/managing-copilot/managing-copilot-as-an-individual-subscriber/managing-your-copilot-plan/managing-copilot-policies-as-an-individual-subscriber)
* **JetBrains AI (Junie):** Toggle detailed data collection (off by default): [https://www.jetbrains.com/help/ai-assistant/settings-reference-data-sharing.html](https://www.jetbrains.com/help/ai-assistant/settings-reference-data-sharing.html)
* **Cursor:** Privacy Mode - [https://forum.cursor.com/t/how-do-i-find-privacy-mode/29](https://forum.cursor.com/t/how-do-i-find-privacy-mode/29)
* **Claude Code:** Anthropic’s data-usage policy (no model training on your code by default) - [https://docs.anthropic.com/en/docs/claude-code/data-usage](https://docs.anthropic.com/en/docs/claude-code/data-usage)
* **ChatGPT:** Opt out of training (“Improve the model for everyone” toggle) - [https://help.openai.com/en/articles/8983130-what-if-i-want-to-keep-my-history-on-but-disable-model-training](https://help.openai.com/en/articles/8983130-what-if-i-want-to-keep-my-history-on-but-disable-model-training)
* **Microsoft 365 Copilot:** Commercial tenants: prompts/responses aren’t used to train foundation models - [https://learn.microsoft.com/en-us/copilot/microsoft-365/microsoft-365-copilot-privacy](https://learn.microsoft.com/en-us/copilot/microsoft-365/microsoft-365-copilot-privacy)

## Guidance for Selecting an AI-Assisted Development Tool

The fast-paced world of AI tooling can be overwhelming when you are getting started. If you are unsure of which tool to start with, consider the following.

### Easy On-boarding

#### GitHub Copilot

GitHub Copilot is available in both VS Code and Visual Studio. If those are your primary development tools, GitHub copilot is the simplest transition into AI Code assistants.

#### JetBrains AI (Junie)

Junie is integrated into the JetBrains suite. This is a great option for getting started if you already use that suite of tools. If you have a JetBrains subscription you automatically get a free version of this which does not count as your 'one license' by SixPivot. Higher-level plans do count.

### Best Results

#### **Cursor**

Cursor is a fork of VS Code and as such, can be used in similar ways as VS Code. Anecdotal experience trends towards Cursor being superior to GitHub Copilot for most use-cases, including an improved user experience for code editing due to its deeper integration in the IDE.

If you also use Visual Studio or Rider for dotnet development but wish to use Cursor, consider the following 2 options:

1. Install the relevant VS Code extensions into Cursor to set up for dotnet development directly in Cursor (if available) or leverage \`dotnet\` command line tools.
2. Open the solution in both Cursor and Visual Studio/Rider; use Cursor for edits and Visual Studio/Rider when you require the IDE tooling.

#### **Claude Code**

Claude Code is a command-line-based agent/assistant. While it performs tasks similarly to Cursor, it does so outside the bounds of the IDE. This can be a great option for power-users that also want to stick with their existing IDE setup.

### Summary

Junie and GitHub Copilot are the easiest 'on-boarding' experience as you do not need to change your IDEs. Claude Code is a paradigm-shift away from always editing in an IDE, and Cursor sits as a trade-off medium between these options.
