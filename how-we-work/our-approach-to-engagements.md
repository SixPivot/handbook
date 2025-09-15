# Our approach to engagements

## Initial Contact

Initial contact with a prospective client can come from anywhere: word of mouth, through developers or customers we've worked with before, and opportunities that we've identified that the sales team have chased up. Whichever the channel, we get the sales team involved and the pre-sales activities kick off.

## Pre-Sales

Pre-sales usually consists of an initial meeting between the sales team and the potential client. Depending on the information at hand there might be a PC involved at that point to help qualify whether the work is our kind of work or not, or that might wait until a second meeting.&#x20;

Next there'll be a requirements gathering workshop led by one of our consultants (an SC or PC) where we'll try to get as much information as we can in order to put together a proposal. That same consultant will then put together the proposal, which will generally include our understanding of the problem, our proposed solution, proposed architecture, team composition, estimated build and running costs, and the usual information about our company, the way we work, T\&C's, etc.

Once a client has signed off on the proposal, sales will work with a PC to schedule the project. We look at technical requirements, experience, PD plans, personalities, etc., to make sure the right people are on it.

## Project Kick-Off

Before day one the PC will be in touch with the client to attempt to get as much of the onboarding done ahead of time as possible. Sometimes this goes well, and we can hit the ground running on day one but sometimes it doesn't. Our goal is to make sure that time is being used as efficiently as possible from the start.

When we reach day one, we have a session with everyone involved to do introductions and set the roles and responsibilities. It's important to have a shared, clear understanding from inception. The first few days will usually be spent setting up user story backlogs, repositories, build and deployment pipelines, etc.

## Running a Project

SixPivot follows an agile software development process for all projects. This is an iterative process that focuses on ongoing communication throughout the entire project to ensure that each piece of functionality is fit for purpose and meets the user’s needs. Despite best efforts the requirements at the start of a project often change as our understanding of the system evolves over time and we receive early feedback from stakeholders and users. The agile software development process allows us to capture this evolving understanding and make any necessary adjustments to future work.

The aim of an agile software development project is to continually deliver incremental pieces of the system to obtain feedback and deliver a return on investment as early as possible. The process starts with the creation of a Product Backlog. From there, we commence continuous feedback cycles called Sprints, which start with a Sprint Planning session, include daily Standups, and concludes with a Sprint Review session and a Sprint Retrospective session.

### Iterative Approach

Agile software development promotes short feedback cycles.

![Circular flow diagram, with Requirements, Plan, Develop, Test, Release, Monitor, and back to Requirements again](<../.gitbook/assets/image (2).png>)

This ensures that any adjustments can be identified and made as early as possible. These adjustments could include:

1. Changes to functionality that was built as per the initial requirements but upon review have been found to be incorrect
2. Changes to functionality that was built as per the initial requirements but upon review a better way to meet the requirements has been discovered
3. Adding functionality that wasn't part of the initial requirements, but have become apparent once a feature has been built and reviewed
4. Removing functionality that was built as per the initial requirements but has since been deemed unnecessary or no longer fit for purpose
5. Fixing functionality that is not performing correctly or fit for purpose

Changes like these are quickest (and therefore cheapest) to make when captured as early as possible, which is why the short iterations of agile software development is important.

### Continuous Improvement

Continuous improvement applies equally to the project and the process. After each iteration, the Delivery Team meets to briefly discuss retrospectively what is working well in the project, what is not, and what they can change to improve things. This continuous improvement endures throughout the entirety of the project.

### Transparency

The nature of agile software development promotes transparency from within the Delivery Team to those outside. By discussing issues each morning at stand-up, reviewing progress at each iteration in a sprint review, and reporting progress after each iteration, the state of the project is always available for anyone to see.

### Our Process

Every project is different. Every project has different people and different challenges, so naturally the process will evolve to suit. Some projects develop more process to address specific needs, while others evolve into a lighter touch process. We do have a fairly standard process that we generally start with. We take a lot of inspiration and terminology from Scrum, but we're not strict Scrum practitioners.&#x20;

> _Rules are made to be broken; Guidelines are made to be followed_\
> _- Quinten, 2022_

As a starting point the ceremonies below generally serve well, but many of the specifics such as attendees, durations, etc., are dependent on the project. The important thing is that we know what value we need out of each session; from there we can find whatever way works to achieve that value.

#### Sprints

**Duration**: One or two weeks

The project is broken down into sprints, which are usually one or two-week periods of time (usually two) during which the team commits to the next piece of work, implements the new features, and reviews those features. At the end of each sprint, we aim to deliver the new functionality to the users (or at least an internal test environment) where feedback can be collected, and adjustments can be made if necessary. From the end of the very first sprint, we aim to have working software available for use.

#### Backlog Refinement

**Duration**: 30-60 minutes\
**Attendees**: Product Owner, Delivery Team

Backlog refinement takes place at some point during the sprint to look ahead and plan work for the next 2-3 iterations. For the next sprint's work, the team looks at the stories planned and confirms that they are the right stories, that they have enough information, that they are estimated and the estimations are still valid, and that they are the right size. For work 2-3 iterations out, the team confirms that the work is in the right order and that the analysis work is progressing accordingly. Any stories that can be estimated should be for the sake of projections and shared understanding.

#### Sprint Planning

**Duration**: 30 minutes\
**Attendees**: Delivery Team, Product Owner

Sprint planning will take place at the start of each sprint. Based on the last few sprints worth of work the team will know how much work they should commit to (based on their velocity – an average of the amount of work completed over the last few sprints). The top of the Backlog is reviewed to ensure that the prioritisation is still accurate, and the correct number of stories are committed to. These stories are moved from the Backlog to a Sprint Board, where their status will be visible for the duration of the sprint as they move through To Do, Doing, and Done columns.

#### Daily Standup

**Duration**: 5-15 minutes\
**Attendees**: Delivery Team, Product Owner

A standup is a short meeting at the start of each day where the team gets together to briefly discuss the work in progress. The aim of this meeting is for members of the team to stay aware of what each other is working on, identify opportunities to help complete stories, and identify and resolve any blockers that people might be having. The Product Owner is invited to observe so that they can keep up to date with the project and help the team resolve any impediments that they might be facing. We usually like to "walk the board" to keep the conversation focussed on the right things.

#### Sprint Review

**Duration**: 30 minutes\
**Attendees**: Delivery Team, Product Owner

Sprint Review will take place at the end of each sprint. The team meets to review the User Stories that were committed to at the start. For each story, the team will review the Acceptance Criteria, review the implementation, and ensure that everyone is happy with what has been delivered. If the User Story has a visual component, it is demonstrated by the Delivery Team to the Product Owner. If it is found that the Acceptance Criteria has not been met, the User Story is carried over into the next sprint where it is completed. If it has been completed, the User Story is considered done and is closed.

During a Sprint Review, it is common for new ideas to surface, or for missing requirements to be identified. These will be added as new stories to the Backlog and prioritised accordingly. Any incomplete stories are briefly discussed.

#### Sprint Retrospective

**Duration**: 30 minutes\
**Attendees**: Delivery Team

At the end of a sprint the Delivery Team will have a short meeting to discuss how the project went during that sprint. The aim is to continually review the processes that the team are using and to discuss ideas about how to improve in the future.

#### Weekly Reports

At the end of each week, we like to send out a short email to the key stakeholders from the client and our own PC's and AM's. We want to share what we're working on, how it's progressing, and call out any impediments and/or risks. The latter is key; we want to communicate risks and problems early so that everyone's aware and resolving while they're small, before they get a chance to build up.

### Artefacts

#### Backlog <a href="#toc50379140" id="toc50379140"></a>

At the start of a new project, the requirements (as best understood at that point in time) are gathered and written up as User Stories (defined below). This collection of User Stories is then prioritised with the Product Owner. The aim with prioritisation is to ensure that high value stories are delivered first. Targeting high value stories ensures that we get feedback on these areas as early as possible, whilst targeting high risk stories ensures that we address any technical risk early on that could impact the way that we build parts of the system.

This prioritised list of User Stories forms the Backlog. The Backlog is a living document that is continually reviewed and refined throughout the project.

#### User Stories <a href="#toc50379141" id="toc50379141"></a>

A User Story is a way of capturing a desired piece of functionality in a specifically formatted sentence: _“As a \<type of user> I want \<piece of functionality> so that \<business value delivered>”_. Writing requirements in this way directs focus to the three most important pieces of information about a software requirement; the type of user performing the action, the functionality itself, and the business value that we’re delivering by implementing this function. A User Story is complemented by Acceptance Criteria, which is a simple bullet point list of things that must work before we can consider the User Story complete. Optionally, a User Story may also contain rough designs of what a screen might look like, and anything else that provides context to the Delivery Team.

### Continuous Integration & Delivery <a href="#toc50379142" id="toc50379142"></a>

#### Continuous Automated Software Builds <a href="#toc50379143" id="toc50379143"></a>

All code written on developers’ machines is continually pushed to a main cloud-based repository where it is automatically compiled. Automated tests are then run against the compiled code to ensure that the changes have not introduced any undesired behaviour.

#### Continuous Automated Software Deployments <a href="#toc50379144" id="toc50379144"></a>

Once code has been automatically compiled, and assuming the automated test suite has passed, the compiled code is automatically deployed to a Development environment in the cloud. This ensures that any changes to the code have not introduced any problems that we might not see on our local machines and provides a very tight feedback loop for the developers to be able to test their changes in the cloud, and if happy, they can then promote this build to a Test environment to make the changes available to explore, test, and provide feedback on.

#### Testing <a href="#toc50379145" id="toc50379145"></a>

Code written as a part of our projects is tested in a variety of ways to ensure it performs correctly, performantly, and to safeguard against accidental changes in behaviour being introduced later. This is done with a combination of unit tests, integration tests, convention tests, performance tests, and manual tests where appropriate.

### Consultant Changes

When we have a project that runs for a while, we like to rotate our people in and out. We do this for a few reasons and genuinely believe that it's win-win. From our side it keeps things interesting for our people, many of whom consult because they like a new challenge on a regular basis. From the client's side they get new eyes and new ideas coming into the project, and a fresh perspective is always a good thing. For both us and the client there's a huge risk mitigation, as there's more than just the team on the ground that know the project, understand the domain, and understand the solution. We've found that these benefits completely outweigh the impact of bringing someone new onto the project and upskilling them.

#### Preparation

Because these rotations are a standard practice for us, we know what needs to be done to make this as seamless as possible. We document the right things, we automate as much of the local environment setup as we can, and we maintain a clean codebase that's easy to bring new people into.&#x20;

Ahead of rolling on to a project the PC will be in touch to give you an overview of what you're walking in to. We'll make some time for PD days to upskill on anything that might be a current gap (maybe this is a Vue gig and you're more Reacty?) so that you can hit the ground running.&#x20;

#### Rolling On

When it's time to roll on to a project we'll organise a day or two (depending on the project) of handover time. During this time, you'll work with one of the existing consultants to get your machine set up, check your access to everything, and get the solution running. You'll probably pair on your first piece of work to help you find your way around the solution. We don't charge the client for the new consultant's time for these days.&#x20;

If we find gaps in the onboarding process, documentation, etc., then we'll update it as we go so that onboarding is that little bit better for the next person.

#### Rolling Off

When we finish up on an engagement we'll spend a bit of time updating any documentation that might need it (ideally we've done this during the gig but this is a good time to double-check it), wrap up any work that we're currently working on, and if there's a new person replacing us, we'll plan for our handover to them. We also make sure that nothing breaks as a result of the change, for example, are there any alert emails that only come to us that need to be updated to someone else?

A week or two after you've finished the PC will be in touch to do an engagement retrospective, where the two of you will look at what went well, what didn't, and what we could improve for the next person.

## Project Shutdown

How we shut down a project is similar to how we roll off. The main thing is to make sure  documentation is up to date; known issues are documented, onboarding guides are up to date, any technical debt is in the backlog and has a plan to be addressed, future stories have as much information as we can give them, etc. We'll also make sure nothing relies on our accounts or presence so that nothing falls over when we're gone.

We know that there's a very good chance that "the next people" could be us in the future, so it's in our best interest to leave things in as good a state as possible.

Although we're not a managed services company and don't offer support contracts to most of our clients, there are one or two where we'll put something in place. These clients are those that came to us with zero IT capabilities and have relied on us end-to-end to deliver a product. We accept ownership of that product going forward and will get a support contract in place so that any future issues can be dealt with.
