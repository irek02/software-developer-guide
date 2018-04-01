---
layout: page
title: Know Your Tools
permalink: technology/know-your-tools.html
category: "Technology"
---

In my experience, I find that the following three statements define a professional software engineer:

* Know the correct technology to build a software solution (build the thing right).
* Understand the correct business problem (build the right thing).
* Build the solution on budget and time.

In this post, I outline the first and essential part of software engineering: knowing your tools.

## Text editor and IDE

Regardless of a particular text editor or IDE, all developers write code in a repeating cycle of two simple steps. These steps consist of adding/editing a bunch of text and then checking if it worked.

Therefore, to become more efficient at writing code you need to reduce the time of each cycle. You can achieve this by using the following features of all modern editors/IDEs:

1. **Code snippets** are useful when you find yourself typing the same thing over again. Save the boilerplate text into a snippet and paste it with a shortcut when you need it.
2. **Fuzzy search** allows you to find any file within the project by typing just a few characters. Very often this is much faster alternative to using a file browser.
3. Learn **Vim** and add it as a plugin in your favorite text editor or an IDE. Using Vim simply makes editing text faster as it requires fewer keystrokes to accomplish the same result as opposed to using a conventional editor.

## Command line

[Seven essential command line skills for a professional developer](http://irekm.com/7-essential-command-line-skills/).

## Version control system

Learning version control system is the first step in becoming a professional software engineer working in a team.

There are two main reasons why developers and organizations adopt version control.

First, **version control keeps a history of code changes**. Not only that, but it also provides a way to view the history and switch between versions of the code with ease. As a result, it reduces debugging time because developers can track down the issue to the particular change in the history. Additionally, developers can restore an impaired service by deploying the previous version of the code.

Second, **version control allows code branching and merging**. This feature is particularly useful for large projects and organizations. By using version control, developers can work on the same project without overriding each other’s changes. Moreover, small projects also benefit from code branching because other developers can contribute changes easily.

Git is by far the [most popular version control system](https://insights.stackoverflow.com/survey/2017#work-version-control). That makes it a natural choice for your primary version control tool.

## Browser developer tools

If you are developing for the web, you should learn your browser’s developer tools. The tooling allows you to see what’s happening under the hood of the user interface from the client perspective. The following are the benefits of learning browser developer tools:

* You can see (and manipulate) the internal markup of the page. It also includes all JavaScript that runs the page.
* It shows all network activity which allows you to see request/response headers and data. This feature is incredibly useful for learning how web applications work.
* It gathers stats about application performance and memory consumption.
* You can view and manipulate application data such as cookies and local storage.

Both Chrome and Firefox come with standard developer tools, so you do not need to install them separately.

## Runtime environment

Every computer program is meant to be executed in some environment. Regardless of the programming language, you should get familiar with the tooling that allows running your software.

For example, when you write PHP code, you could use something like XAMPP to execute it locally. When you upload your code to a server, however, it will likely run in a LAMP stack. If you write Java code, you should get familiar with JVM and how to set it up locally and on a remote machine.

The point is that without knowing anything about an environment in which your code is supposed to run it is much harder to become a successful software developer.
