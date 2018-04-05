---
layout: page
title: Use best coding practices and principles
permalink: technology/practices-and-principles.html
category: "Technology"
---

Following best software engineering practices is only a part of being a highly effective developer. If you want to deliver the best result, you need to do three things:

* Know which change will make the most impact.
* Implement this change by delivering high-quality code.
* Do it on budget and time.

In this post, we will focus on the second point: **delivering high-quality code**.

Use the following practices and principles to produce robust bug-free code; code that doesn’t break in production; code that’s easier to read, change and maintain.

## Coding standards

Coding standards ensure same code format across an entire project. It enables faster reading and comprehension of code. It is much easier to read through code that uses same conventions for main structs such as curly brackets, variable/function naming, indentation, etc. Coding standards is one of the most essential best software engineering practices.

Examples of coding standards include:

* use camelcase instead of the underscore in function/variable names
* use two spaces for indentation, no tabs
* no spaces between name and first parenthesis in function calls

The best way to ensure coding standards is to include it as a part of automated build process. For example, in my team at Acquia, we use eslint automated by gulp which runs on each code change. It validates all code formatting rules and fails in case of a violation.

## Code reviews

In my experience, code reviews proven to be one of best software engineering practices. Code reviews work as follows:

1. Developer submits a patch for a review. For example, in the form of a Github pull request.
2. Other developers review the changes and comment about potential bugs, improvements, and gotchas.
3. The author addresses these comments, makes updates to the code and submits an update patch for another review.
4. Steps two and three repeats until everyone is happy and the patch merges into the codebase.

### Issues with code reviews and how to deal with them

Although code reviews is an essential part of code quality, it can also be one of most challenging parts of the process:

* It might take a while for others to provide feedback for your patch which forces you to switch context and work on something else.
* If you get busy with other tasks, it might get a while until you address feedback received for your patch. As a result, it takes longer to ship the change.
* Sometimes you might disagree with feedback posted for your patch. Then you have to choose: either just apply the requested change or start a potentially lengthy unproductive discussion.

The first two issues are easy to fix. As a team, you can agree to provide feedback within X hours. Preferably, every team member should allocate a couple of slots each day for reviewing patches. For example, 30 minutes in the morning and 45 minutes in the afternoon.

The issue with disagreeing on feedback is trickier. Personally, I always strive to finish my task as quickly as possible and just apply the requested change. But I only do it when I am confident that requested changes don’t introduce long-term adverse effects. Otherwise, I’m willing to get into a discussion and spend precious time to understand why a change is necessary.

## Test-driven development

TDD is by far my most favorite item among best software engineering practices. It guides code development by following the three rules:

1. Do not write any production code unless it is to make a failing unit test pass.
2. Do not write any more of a unit test than is sufficient to fail, and compilation failures are failures.
3. Do not write any more production code than is sufficient to pass the one failing unit test.

You usually start by writing a very first failing assertion. Typically this assertion fails due to a missing class, method or whatever you’re testing against. Then you add a little bit of code just to make that assertion pass. Next, you add another assertion that tests a happy path for your code. Then you make that assertion pass by writing just enough code. Next, add assertion against other paths and make it pass. And so on until the code does what it should do. Then you polish up the code while making sure the tests pass.

### Benefits of TDD

* You always end up with high test coverage.
* You naturally write better tests. It is because you are forced to think about your code regarding expected behavior (interface) opposed to implementation details. If you write tests after the code, you tend to assert against implementation rather than interface which is a recipe for fragile tests that add problems and no benefits.
* You end up with just enough code to satisfy expected behavior. Less code — fewer bugs and maintenance.
* It provides focus because you always have the next step: write a failing test, make a test passes or refactor.

## End-to-end testing

End-to-end tests simulate user interaction against production system engaging all layers of a stack starting from Javascript that runs in a browser down to database servers including everything in between.

However, end-to-end tests are known to be fragile, slow, hard to debug and maintain.

To minimize these issues only write end-to-end tests for most critical parts of your system. Other areas should be covered by unit testing and monitoring. However, I still believe that end-to-end testing is one of the best software engineering practices.

## Design patterns

As engineers, we have been writing code for decades now. There is a set of problems that we have to solve over and over again. These are well-known problems that have a set of well-known solutions. Meet the design patterns: [https://sourcemaking.com/design_patterns](https://sourcemaking.com/design_patterns).

The design patterns can help when:

* Object creation is too complicated for consumers (can be solved by the abstract factory pattern).
* There is a need to use a third party library, but its interface doesn’t fit into an existing architecture (can be solved by the adapter pattern).
* Your data is stored in many different ways, but your algorithms need to be able to traverse it uniformly (can be solved by the iterator pattern).

Use these patterns instead of re-inventing the wheel.

## SOLID

SOLID is an acronym for five principles promoted by Bob Martin. They allow writing code that’s less fragile and easier to change.

The principles:

1. Single responsibility principle: a class should have only one reason to change.
2. Open/Closed principle: a class should be open to extension and closed to modification.
3. Liskov substitution principle: a parent class can be replaced with its child class without breaking any consumers.
4. Interface segregation principle: create more specific interfaces rather than general interfaces.
5. Dependency inversion principle: consumers should depend on abstraction rather than concrete implementation.
