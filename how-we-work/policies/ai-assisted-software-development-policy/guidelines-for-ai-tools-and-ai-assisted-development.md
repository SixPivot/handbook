# Guidelines for AI Tools and AI Assisted Development

To make this more fun, try to determine which parts of this document were written by ChatGPT.

## Why have a policy and guidelines?

AI (or, more accurately, large language models and other training-based models) has taken over the world. ChatGPT and GitHub Copilot are the two biggest examples that have affected how we, as developers, are able to design, troubleshoot, and test code.\
Using client IP and sensitive information in these contexts needs to be carefully considered, as does using the output of these models in commercial work. While we can take advantage of the time savings and comprehensiveness when using AI, we need to be careful to keep our high standards, both in terms of the code and content we produce, and our responsibilities when working with client IP.\
Having a policy and guidelines around our use of AI tooling and AI assisted development makes it clear where we need to pay attention to these considerations.

## The Guidelines

**Client IP (intellectual property), commercial secrets, PII (personally identifiable information), and internal information must be protected at all times.**

ChatGPT conversations are not private. At the very least you're sharing information with a third party. In fact, ChatGPT uses the conversation as training material, so you need to make sure you're not sharing sensitive or identifiable client information.

* Treat conversations as if you are having them with a stranger that has a vested interest in sharing all the information you're giving them.
* Talk in the abstract.
* Don't share anything that is considered Client IP - like pasting a section of code belonging to the client.
* Don't share any commercial secrets or internal information, such as employee names, business names, financial details, etc. Put yourself in your client's shoes and ask, "Is this something that would be ok for my competitor to know?"
* When setting up GitHub Copilot you're asked if you want to allow sharing back to GitHub to improve the service. Make sure you opt out of this, otherwise client IP will be shared back to GitHub and might be shared out to other users of the service.

**We must maintain the high quality and high standards that SixPivot is known for.**

It will be tempting to just copy and paste code directly from your bot helper. However, both ChatGPT and GitHub Copilot have a fundamental flaw: they are trained on information found on the internet, and are reinforced on quantity, not necessarily on the quality of their output.

* While the AI tools can generate useful suggestions, the code might not always be high quality or optimised for the task at hand.
* Make sure you read and understand what you're being given, not just on a syntactic level but looking at the bigger picture.
* Test the code that you've been given, ensure that it's doing what it is meant to do.
* Consider the code to be written by a junior, which requires a comprehensive code review.
* You may need to completely rewrite the generated code.
* Treat the suggested code as just that: a suggestion.

**AI is a tool that we should embrace.**

Like any tool, it can provide a considerable increase in the speed and quality of what we produce from day to day. However, also like any tool, it has to be held correctly, otherwise we risk injury or damage.

