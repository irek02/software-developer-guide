---
layout: page
title: Eliminate constraints
permalink: process/constraints.html
category: "Process"
---

In previous posts we learned that a professional software engineer has to know three things:

1. Technology (how to build a solution).
2. Business (the problem you’re trying to solve).
3. Process (how to build and deliver the solution efficiently).

We learned that an efficient process requires continuous delivery and an agile framework. In this post, you will learn the last piece of the puzzle which is about eliminating constraints.

## What are constraints?

A constraint is something that obstructs you from achieving some goal. For example, you want to complete your task within 2 days. However, it takes other developers at least 3 days to review your code. This slow code review process is a constraint.

## Why bother eliminating constraints?

When you remove constraints from your process you get stuff done faster. Let’s look back to our code review example. Let’s say you convince other developers to review your code within 1 day instead of 3 days. As a result, you’ll end up finishing your tasks faster. It’s as simple as that.

## How to eliminate constraints

### 1. Document your workflow

It takes a number of steps to turn an idea into a successful software product. Every team finds their own way to establish this process. Therefore, prior to finding constraints, you need to know your process.
Here is an example. A while ago I worked with one of the teams at Acquia. We noticed that some of our tasks were taking a long time to finish. So we broke down the life cycle of a typical task. It looked like the following:

1. Pick up the task and start working on it.
2. Post the code for review.
3. Receive feedback.
4. Address feedback.
5. Repeat the above until the code is approved.
6. Release to production.

### 2. Measure time in each step

Once you determined all steps in your process you need to know how long each step takes. Tools like Jira provide convenient metric tracking for this kind of thing. For example, you can you can see how long each task spent in different statuses. These statuses might include todo, in progress, in review, ready to release.

### 3. Find waste

The previous step shows where you need to improve things.

My team at Acquia found that tasks spend a lot of time in the review status. So we looked at commits and comments in our GitHub pull requests. What we learned is that when you post code for review it takes a while before anyone visits it. We also learned that after the code receives feedback it takes the developer a while to address it. We concluded that these delays in the feedback-response loop caused overall slow lead time for many tasks.

### 4. Reduce waste

The way you can speed up slow steps depends on the nature of the issue.

In the case of slow review process as a team we agreed on the following:

1. Provide feedback to other code reviews within 24 hours.
2. Address feedback to your code reviews as soon as possible.
3. Don’t have more than two tasks in progress/review.

This reduced wasted time when tasks were just sitting in a queue. In the end, each individual task was completing faster. This resulted in overall increase in velocity. In other words, we got more stuff done in less time.

## It’s all about the journey

This process of continuous improvement is an ongoing battle. Soon after you improve your process in one place you learn that it is struggling in another place. And so on.
Check out my other post where I a model where a team can start with Scrum and continue with Kanban.

To learn more about this topic I suggest to read these two fantastic books:

* [https://www.amazon.com/Phoenix-Project-DevOps-Helping-Business-ebook/dp/B00AZRBLHO](https://www.amazon.com/Phoenix-Project-DevOps-Helping-Business-ebook/dp/B00AZRBLHO)
* [https://www.amazon.com/Goal-Process-Ongoing-Improvement-ebook/dp/B002LHRM2O](https://www.amazon.com/Goal-Process-Ongoing-Improvement-ebook/dp/B002LHRM2O)
