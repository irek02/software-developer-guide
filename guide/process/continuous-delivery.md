---
layout: page
title: Establish Continuous Delivery
permalink: process/continuous-delivery.html
category: "Process"
---

Successful developers do three things well:

1. They know the technology.
2. They understand the business problem.
3. **They deliver the solution on budget and on time**.

In previous posts, we learned about technology and business. With that, you can figure out what business problem you’re trying to solve and how to solve it. The next step is to build and deliver the product as fast as possible. Continuous delivery plays a crucial role in achieving this goal.

<b color="red">
Edit:
Why CD is important
CD is a long term investment in future value delivery. When established early on, CD will save a lot of time otherwise wasted on bug fixing and slow feature release rate
</b>

## What is continuous delivery (CD)?

continuousdelivery.com defines it as follows:

> Continuous Delivery is the ability to get changes of all types—including new features, configuration changes, bug fixes and experiments—into production, or into the hands of users, safely and quickly in a sustainable way.

In practice, this means decoupling your system and automating your process. This includes steps for testing, building and releasing code to production.

## Advantages of continuous delivery

Because CD streamlines the deployment process, developers are not afraid to push new features as soon as they built them. This results in smaller and more frequent code releases, which brings few advantages:

1. You can quickly learn whether you’re making **the right thing**. For example, you build a simple notification widget for your product and release it using CD.  Later you find that it doesn’t move the needle for any of your business metrics (session length, new subscriptions). As a result, you know that you should stop wasting time on a useless feature and move onto the next thing.
2. You can quickly learn whether you’re building **the thing right**. For example, you add a first version of the chat feature for your product. Users love it and use it extensively. At the same time, you learn that this feature results in sudden bursts of server calls that cripple your site. CD allows you to roll back the feature to restore the site and re-think your approach.
3. CD **improves team morale and trust in the engineering** by allowing to fix production issues faster. This is possible because streamlined releases process results in smaller production issues. And you know that a team can fix problems quicker and with less effort. Therefore, organizations tend to focus on solutions instead of playing a blame game.

## How to setup continuous delivery

On the most basic level it takes three steps to deliver software:

1. Add code.
2. Test.
3. Release to production.

Anything that goes in between is unique to every team. Therefore, it’s really up to the team to figure out what gets in the way of delivering a result. However, there are few primary tools and patterns that every team must utilize to create CD.

### Use version control

Version control provides two features that are essential to CD:

1. Ability to integrate code changes into existing codebase (branching/merging).
2. Ability to create snapshots of the codebase (tags). These tags can then be deployed to production. If a new tag contained a bug, a team can deploy an older tag and quickly restore the system.

### Automate tests

It is impossible to release software frequently without testing it. Obviously, you need to write unit tests in the first place. Ideally, most of the code is covered by unit tests. They usually run faster and are most straightforward to automate.

In addition to unit tests, there can be integration and acceptance tests. However, they are slower. Also, they are harder to automate. Therefore, it is well worth it to optimize and automate the unit tests first.

### Create deployment pipeline

The previous steps ensure that your teams can integrate changes into the codebase and run tests. The next step is to create deployment pipeline which automates the whole process. In the deployment pipeline, code changes go through several stages. Each stage serves some purpose. This includes building the source code (if necessary), running all tests against it, etc. In the end, it verifies that the change does not introduce any regressions.

An example of a simple continuous delivery pipeline can look something like this:
![Continuous delivery pipeline]({{ "/assets/images/continuous-delivery.png" | absolute_url }} "Continuous delivery pipeline")

## Conclusion

In this post, you learned why it is essential to ship code to production as soon as possible. You also saw how continuous delivery enables teams to achieve this goal. Also, you’ve become familiar with how to create continuous delivery and what are its main components.

To further explore the of continuous delivery I highly recommend checking out [https://continuousdelivery.com](https://continuousdelivery.com).
