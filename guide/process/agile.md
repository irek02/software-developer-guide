---
layout: page
title: Use and optimize an agile framework
permalink: process/agile.html
category: "Process"
---

You can hire best engineers. You can show them what business problems you are trying to solve. However, if they cannot deliver result efficiently, none of this will matter.

This post is an introduction to agile software development. You will learn:

* How organizations built software before agile.
* Why agile is better.
* What is Scrum and how it works?
* How your team can use Kanban to build software faster.

## Before agile and why it did not work

It usually takes few steps to create and deliver software:

1. Flesh out requirements
2. Design
3. Build
4. Test
5. Deploy

In the old days, organizations would spend months and even years in each stage before they finally deliver software to users. We call it waterfall.

As time showed, waterfall approach often fails due to one significant flow. It assumes that the organization knows all requirements, constraints, issues and potential scope changes before developers start coding. Turns out, knowing future is nearly impossible.

## Meet Agile

In 2000s engineers formalized a different approach. An approach where an organization does not assume that it has all information upfront. Instead, it plans, designs, builds, tests and deploys a system within weeks rather than months (with limited functionality). They called it an iteration.

After each iteration developers and business evaluate the outcome. Based on this evaluation the team plans next iteration. This allows teams to adjust to any unknowns discovered in the previous iteration. For example, new customer feedback, change in market or an issue in the deployment process.

## Start with Scrum

Scrum is the formalized approach to agile development.

Scrum defines the following **roles**:

* Development team.
* Product owner. He or she takes input from executives, customers, and other teams. This results in a list of requests for the development team.
* Scrum master. He or she helps the development team to overcome blockers.

In Scrum, a development team delivers software in iterations (sprints). Each iteration typically lasts 2-4 weeks. Each iteration consists of the following **steps**:

1. The product owner tells the team *what* the business wants. This takes the form of a product backlog filled with user stories. Product owner sorts the stories by priority.
2. Planning: the team reviews the backlog and plans *how* and *how much value* they are going to deliver in the next sprint. The team estimates the size of each task and fills in the sprint backlog. Tasks in the sprint backlog represent team’s commitment to finish the upcoming sprint.
3. Execution: during the 2-4 week period the team members work to finish all tasks in the sprint. They discuss blockers during daily scrum. Scrum master helps to resolve blockers or any other issues.
4. Review (demo): the team, the product owner, and stakeholders review the delivered value. For example, showing new feature in action to stakeholders or customers.
5. Retrospective: the team, the product owner, and the scrum master decide if the team fulfilled their commitment this sprint. They analyze what went wrong, what went well and what they can improve.

Then the cycle repeats.

![repeats]({{ "/assets/images/scrum.png" | absolute_url }} "Scrum")

## Continue with Kanban

Some of the most significant challenges in software development are scope creep and emerging requirements. Iterative nature of scrum enables organizations to face those challenges and adjust accordingly. For many businesses, this is the main reason for adopting Scrum.

However, there is another advantage in doing 2-4 weeks iterations. It comes in the form of the retrospective. It enables teams to review their process frequently. As a result, they have opportunities to improve the way they deliver value incrementally. Incremental process improvement is the essence of **Kanban**.

The focus of Kanban is to reduce waste which is another big challenge for organizations.

**Kanban principles:**

1. Change management: make incremental improvements to an existing system. In our case, the current system is based on Scrum.
2. Service delivery: focus on delivering value to the customer.

**Kanban practices:**

1. Visualize your workflow.
2. Limit work-in-progress.
3. Manage flow (eliminate bottlenecks, maximize production)
4. Make policies explicit. For example, what is the definition of done for your team?
5. Feedback loops. Scrum already covers via sprint review and retrospective.
6. Improve and evolve.

The above shows that Kanban naturally completes Scrum. It relies on scrum to provide an initial process for agile development. Then it guides an organization to improve that process. In the end, it results in a gradual increase of team velocity while ensuring customer value focus.

## Conclusion

In this post, you learned that before agile, organizations used waterfall approach for building software. You saw that without a feedback loop it did not work. Scrum solved this problem with an iterative approach with tight feedback loops between business, customers, and developers. You also learned how Kanban could complement Scrum by helping to eliminate waste and increasing team velocity.
