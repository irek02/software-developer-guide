---
layout: page
title: Learn about software architecture
permalink: technology/architecture.html
category: "Technology"
---

Understanding software architecture is a an essential skill. It allows creating solutions that evolve the system. Otherwise, it’s too easy to drive it into a swamp from which it never recovers.

Read on and you will learn:

* why it is important to understand software architecture
* how to improve understanding of a software architecture
* how to design and sustain a good software architecture

## Signs of poor software architecture

Poor architecture can show in many ways. Code is hard to test, change and debug. The system is fragile. It’s also prone to security and performance issues. And no one fully understands it.

## Know your architecture

### 1. Ask someone for initial walkthrough

Codebase is first the place to look but it’s best to start with asking someone familiar with the system to draw few boxes and arrows to visualize main components of the system. Then you can find those components in the codebase and go from there.

### 2. Use debugger to generate stack traces for main endpoints

One of the best way to figure out how a system works is to use a debugger.
Find a line in the codebase. Then place a break point and execute the code. A debugger will generate a stack trace.
Stack trace can show all major components that were involved in producing a response for the request. When studying those components focus on their purpose and not implementation details.

### 3. Document what you learned

It’s a good idea to write things down as you learn. Otherwise it’s too easy to forget important details. Once you documented your knowledge you can present it to a group for feedback.

## What is a good software architecture?

Before trying to create a good architecture let’s define what it means:

* it expresses its purpose and responsibilities
* it’s relatively easy to make additions and adjustments
* it’s technology/framework agnostic

## How to create good architecture

Use the following to help you create good architecture.

### 1. Follow principles of clean architecture

Uncle Bob is a software development veteran. His advice comes from decades of experience.

### 2. Have a vision

Architecture of a system should be dictated by its purpose (requirements). Therefore it is highly beneficial to figure out why and what you are trying to build. This leads to the next point.

### 3. Do some design upfront

Scaffold main classes/services and their interfaces before diving into code. You can even stub methods/endpoints with mocked data and build a first proof of concept.

### 4. Use Domain Driven Design

Domain Driven Design is a methodology that bridges business domain and system implementation. It helps to ensure that the core of the system architecture is fully dedicated to its business purpose.

### 5. Use Test Driven Development

TDD helps you create better interfaces. Classes end up having better defined roles and are easier to reuse. And this is just one of many benefits of TDD.

### 6. Follow SOLID principles

SOLID is a set of principles promoted by Uncle Bob. Learn more at butunclebob.com/ArticleS.UncleBob.PrinciplesOfOod.

### 7. Design for change

Lastly, the only constant in software is change. So design your architecture to be flexible.
