# QA Process - Software Development and Testing <!-- omit in toc -->

- [Feature development: where do I start?](#feature-development-where-do-i-start)
- [Epics and User Stories](#epics-and-user-stories)
  - [Epics](#epics)
  - [User Stories](#user-stories)
- [Software Requirements Specification Document](#software-requirements-specification-document)
- [Testing and Development](#testing-and-development)
  - [Making a Test Plan](#making-a-test-plan)
  - [Test Strategy](#test-strategy)
  - [Testing Tools](#testing-tools)
- [Test Driven Development](#test-driven-development)
  - [Determining appropriate tests](#determining-appropriate-tests)
  - [Writing a failing test case](#writing-a-failing-test-case)
  - [Writing code to pass your test](#writing-code-to-pass-your-test)
  - [Refactoring Code](#refactoring-code)
- [Testing Templates](#testing-templates)

You might be wondering, before jumping into coding and planning tests for a new feature, _where do
you begin_?

## Feature development: where do I start?

- Clearly articulate the problem and why the changes need to be made.
- Create [epics](#epics) for each feature for planned development.
- Identify [user stories](#user-stories) of the feature.
- Consider how best to mitigate risk or look for alternate solutions.
- Determine functional and non-functional requirements.
- Determine acceptance criteria.

  - What are the metrics for success?
  - What's in/out of scope?

- Your extracted purpose and requirements will be documented within your
  [Software Requirements Specification](#software-requirements-specification-document) document.
- Plan your testing by defining your Test Strategy and Test Plan:
  - Using your specifications, fleshout the expected behaviour for different use case scenarios;
    these will provide scenarios to be tested in your [Test Plan](#making-a-test-plan).
  - Determine _how_ you are going to test your scenarios and describe this in your
    [Test Strategy](#test-strategy).

## Epics and User Stories

### Epics

Epics describe a large body of work that will be broken down into smaller tasks (called user
stories). Epics are a higher-level view of user request or needs that help with considering larger
aims, what value the work described will bring to the business, organizing work and creating a
hierarchy. Epics will be broken down into smaller, more manageable tasks ("user stories") to be
completed by team members. A Markdown [Epic Template](../../leadership/epic-template.md) is also
available.

### User Stories

User Stories are user-centric statements often put in the form of:

**"As a [persona], I [want to], [so that]"**

This describes a _persona + need + purpose_.

A **[persona]** – describes the person we are building this for. The persona is not just a role or
job title; we want to have an understanding of who the person is, how they work, think and feel.

**[wants to]** – describes the user's _intent_ (what they want to achieve) and not the feature they
use. If you are describing implementation specifics here, you are taking the wrong approach.

**[so that]** – explains the motivation behind the user's desire and the overall benefit to them
from what they are trying to achieve.

User stories use non-technical language to provide context and an understanding of what is to be
built and why. They provide a framework for approaching development which is user-focused, discrete
and small enough to be manageably tackled by team members in an Agile environment.

Benefits include:

- Keeps focus on the user: keeps the team focused on solving real-world problems in user-centric
  ways.
- Enables collaboration: by defining the end goal, the team can work together on deciding on how
  best to meet it
- Drives creative solutions: the focus on the end-user solution required, rather than the how,
  encourages creative problem-solving (where to-do lists do not).

In Agile methodology, during a sprint or iteration, the team decides which user stories to tackle
that story and discuss requirements; once agreed, requirements are added to the stories; Story tasks
and subtasks can be tracked and assigned using the team's relevant Trello board; user stories for
future sprints can remain in the backlog.

When defining user stories, consider:

- Definition of "done": how will we know when a task/story is complete?
- Tasks or subtasks: what steps need to be completed and by whom?
- User personas: who is the user being considered; are there multiple users (consider making user
  stories for each of them)
- Ordered steps: In a larger process, write a story for _each step_
- Time: consider how long a story may take; if it's more than one sprint, or seems very complex, the
  story may need to be broken down into smaller stories (or, you may be looking at an epic)

Further background on user stories can be found at
https://www.atlassian.com/agile/project-management/user-stories

## Software Requirements Specification Document

A Software Requirements Specification (SRS) document describes the expectations for your product,
how it should perform, and the functionality required to meet stakeholder needs. An
[SRS template](templates/srs-template.md) has been provided which sets out an example format of an
SRS, including the following components.

- **Introduction**:

  - **Product Purpose**

    Define the purpose of the SRS

  - **Intended audience**

    Who are the expected readers (testers, developers, leadership team?) of the SRS document?

  - **Intended use**

    How are these readers expected to use the SRS document?

  - **Scope**

    What are the goals and objectives for this product? What should the product do (And what should
    it _not_ do?)

  - **Definition and acronyms**

    Describe relevant terms, definitions and acronyms required to understand the document.

- **Overall Description**

  Describes your product and what you are going to build; describe here whether it is a new product,
  or an enhancement/add-on to an existing product, who it is for and why it has value. This explains
  the general background and factors affecting requirements (rather than the specific requirements
  themselves)

  - **User Needs**

    Who will use your product feature and how? What needs do your end users have that you need to be
    aware of?

  - **Assumptions and dependencies**

    Provide any assumptions made (what are we assuming to be true) or dependencies for your
    product/feature

- **System Features and Requirements**

  - **Functional Requirements**

    Fundamental requirements are essential requirements that, as the name suggests, provide
    functionality and are often described by "The system shall..." statements.

  - **External Interface Requirements**

    Specific requirements detailing hor your product interfaces with other components. They may
    include user, hardware, software and communications interfaces.

  - **System Features**

    _System features are types of functional requirements. These are features that are required in
    order for a system to function_

  - **Nonfunctional requirements**

    Nonfunctional requirements are those relating to non-functional measures and relate to aspects
    such as performance, safety, security and quality.

Further references include Perforce's
[How to Write an SRS Document](https://www.perforce.com/blog/alm/how-write-software-requirements-specification-srs-document)
and, for a higher level of detail on recommended guidelines for the SRS elements,
[IEEE’s Recommended Practice for Software Requirements Specifications](https://drive.google.com/file/d/1G1vQq-RjnbEmTTzItIUarWuMnbqZchlx/view).

_After completing the SRS, you’ll need to get it approved by key stakeholders. This will require
everyone to review the latest version of the document_

## Testing and Development

Testing should be built into the software development process. Thoth-Tech advocates for a
[Test Driven Development](#test-driven-development) (TDD) approach. In any event, all coding
projects should consider and record their [Test Plan](#making-a-test-plan) and
[Test Strategy](#test-strategy) and produce these as project deliverables.

### Making a Test Plan

For each product/feature, using the required specifications, flesh out the expected behaviour for
different use case scenarios. A collaborative approach helps to make sure you are defining the right
problem and solution; be sure to seek feedback from the team during this process. These scenarios
will be detailed in a Test Plan, which will record each scenario to be tested, the expected outcome,
and the actual outcome of tests. A simple Markdown
[Test Plan Template](templates/test-plan-template.md) has been provided.

### Test Strategy

You need to consider _how_ you are going to test your scenarios as part of this process –
considering matters such as what [testing tools](#testing-tools) you will use, what platforms tests
will be performed on, any release processes, and what deliverables will you need to produce. This
should be considered as part of your Test Strategy – a deliverable which should be produced as part
of the QA process. Other documents that may be produced as part of the QA process include a Test
Plan and Bug Reports.

Templates have been provided for sample [Test Strategy](templates/test-strategy-template.md),
[Test Plan](templates/test-plan-template.md) and [Bug Report](templates/bug-report-template.md)
documents.

While manual testing may be conducted initially, moving towards automated tests allows for better
efficiency, ease of code checks and is the preferred method to allow automatic test incorporation
into the deployment pipeline. Testing and processes, like many other in the Agile model, are not
static, and can (and should) be improved on successive iterations. This may include iterating
existing processes for testing releases as well as automating more functionality.

Thoth-Tech encourages a [test driven development](#test-driven-development) approach, in which
testing is intertwined with softward development. If your software coding has begun in advance of
testing considerations, then you should still formulate a Testing Strategy, including a Test Plan,
to verify that your code successfully meets requirements.

### Testing Tools

Using testing tools makes tests easier to write and easier for future developers to understand. They
add consistency and repeatability to the testing process, and make test design and documentation
simpler.

Testing tools include:

- [Jasmine](https://jasmine.github.io) (for javascript unit testing)
- [Cypress](https://www.cypress.io/) (javascript end-to-end testing)
- Minitest (for Rails)
- [Catch2](https://github.com/catchorg/Catch2/tree/v2.x) (for C/C++)
- Junit (for Java)
- Nunit (for .Net languages, such as C#, F#, Visual Basic)
- [Karma](https://karma-runner.github.io/latest/index.html) (a testing tool for automation that
  utilises other testing frameworks)

But there are many more. Look for what is currently available and popular in your language.
Currently, proposals have been put forward for utilising [Jasmine](https://jasmine.github.io) and
[Karma](https://karma-runner.github.io/latest/index.html) for relevant unit testing and automation
and [Cypress](https://www.cypress.io/) for end-to-end testing in the OnTrack space.

## How do I prove my code does what it's supposed to do? <!-- omit in toc -->

## Test Driven Development

By utilising _test driven development (TDD)_, software requirements are embedded into the testing
and coding process, so that functionality is validated as it is coded. This assists to confirm code
is actually fulfilling the requirements while improving the robustness of testing and paving the way
for automation in deployment pipelines.

How does it work?

1. [Determine appropriate tests](#determining-appropriate-tests)
2. [Write a failing test case](#writing-a-failing-test-case)
3. [Write code to pass the test](#writing-code-to-pass-your-test)
4. [Refactor code](#refactoring-code)

### Determining appropriate tests

Tests should come from your _requirements_ and _acceptance criteria_; they are designed to test
requirements not methods.

From these, project teams solidify scenarios that relate to project requirements – make sure you
collaborate and obtain feedback on these scenarios to check that you have understood the
requirements correctly. This can be done through group brainstorming sessions (especially valuable
in initial stages) and through returning to the team for feedback.

Remember, test-driven development does lend itself to an iterative software development process,
such as Agile, so it is quite suited to a development process where coders start with basic
functionality that may be added to or improved in subsequent iterations. This is okay – you will
progress and build, and using the TDD approach allows for evolving such code in a robust manner. A
useful approach is to begin with base functionality and increase complexity.

### Writing a failing test case

_Why are we writing a test to fail?_

Having determined our test case from our acceptance criteria, we begin by writing some code that
will fail our test. Why? Because we want to make sure that our test works; we don't want later
checks to be useless because we wrote our test incorrectly and are having false positives returned.

### Writing code to pass your test

Once you've confirmed your test "works" by failing for code that doesn't pass your test, you can now
write code to pass your test. This can also be an iterative process – first, starting with arbitrary
values that you know will give the "expected" result (faking it to pass), before refining to be more
broadly applicable to how your code needs to work in the live system.

When you are satisfied that your code is complete, it is wise to challenge your test again with
known failing code to reaffirm your testing is still functioning as expected.

**What next?**

Once your code is passing your test, it's time to examine _code quality_. Is your code:

- reusable:
  - are there components that are (or will be) repeated elsewhere?
- efficient:
  - is your code cost-effective and easily modifiable?
- readable:
  - could a third-party looking at your code easily understand what is going on?

These are concerns which may be addressed through _code refactoring_.

### Refactoring Code

Refactoring involves changing the _internal_ structure to make it more easily understood, effective
and/or cheaper to modify without changing the _external behaviour_ of the code.

While writing a failing test case and then coding it to pass focuses on **requirements** (and adding
**new functionality** ), refactoring focuses on **improving design**.

**My code is complete and passing tests; is it time to refactor?**

You don't need to assess your code for refactoring on every test, but if your find your code is:

- repeating itself (or repeating functionality),
- confusing to follow, or
- you are getting stuck,

these are good signs that it might be time to refactor.

**How do I refactor?**

Extract function refactoring is one common and intuitive approach to refactoring code: this involves
comparing the code intention with the implementation. If the code is doing more than the intention,
particularly if it is doing things that may be repeated elsewhere, it probably contains functions
that should be split off.

[Refactoring.com](http://refactoring.com/) provides useful reading that covers a number of
refactoring techniques.

**Further information about Test Driven Development**

Deakin students have free access to LinkedIn Learning courses.

A useful course on these general concepts is
[Programming Foundations Test Driven Development](https://www.linkedin.com/learning/programming-foundations-test-driven-development-3)

Developers working with C++ may also find
[Test Driven Development in C++](https://www.linkedin.com/learning/test-driven-development-in-c-plus-plus)
useful

## Testing Templates

Several Markdown testing templates are available:

- [Sample Test Strategy](templates/test-strategy-template.md)
- [Test Plan Template](templates/test-plan-template.md)
- [Bug Report Template](templates/bug-report-template.md)
