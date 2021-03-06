---
layout: page
title: Master your stack
permalink: technology/stack.html
category: "Technology"
---

In my view, most successful developers are the ones who know their technologies, business/organizational goals and delivery process optimization. Therefore they know how to build a thing, make sure that it solves a correct problem and do it efficiently.

In this post, I will brush over the technology part of being a successful developer, specifically, knowing your technology stack.

Read on, and you will learn:

* What is a technology stack
* Advantages of knowing your technology stack
* Basic (and advanced) make up of any web service
* Frontend technologies
* Backend technologies

## What is a technology stack?

The technology stack is a set of programs that work together to fulfill a specific function. For instance, LAMP is one of the most popular stacks on the web.

Knowing your stack means that you have at least a rough idea what happens between entering a URL of your website and receiving a response.

## Advantages of knowing your stack

In the long run, it is highly beneficial to know your technology stack:

* It gives you the expertise to implement bigger solutions and solve bigger problems.
* You can debug more complex issues that involve multiple systems.
* You are more competitive in the job market and have a potential to earn a better salary.

As shown above, knowing your stack is beneficial. Next, we will review main components of a full stack. We will think of it as a web service. And on the web, it always starts with a request.

## How a basic web service works

Below is an outline of a conceptual web stack that’s capable of serving basic dynamic content. Think of a WordPress site running on LAMP stack as an example.

![Basic interaction with a web service]({{ "/assets/images/basic-web-service.png" | absolute_url }})

In our example, a user initiates the request by entering http://example.com/index.php?p=123 URL in a browser. The central part of the URL is the domain name `example.com`. However, servers do not have domain names; they have IP addresses. So before the request can reach the web server, the DNS service looks up what IP address is registered for example.com.

Using the IP address, the request reaches the web server (physical or virtual). This web server has a process that listens to all incoming web requests. And that is a software web server (e.g., Apache).

The software web server, determines that the requested resource index.php?p=123 needs to be interpreted by PHP. It passes the contents of index.php to a PHP process. PHP executes contents of index.php, line by line.

During the execution of the PHP code, it might make use of a database, which is the last leg of the journey in our example.

PHP then it returns a response to the web server (Apache), typically HTML of a requested web page, which then makes its way all the way back to the client.

That is all it takes on the most basic level.

## How a horizontally-scalable web service works

Now let’s look at a more advanced version of a stack. Let’s say we want our site to be able to serve more requests, so we add more web servers. A load balancer is used to distribute requests among web servers. A CDN is used to cache responses and prevent unnecessary traffic.

![A web service with CDN caching and load distribution.]({{ "/assets/images/hor-scalable-web-service.png" | absolute_url }})

This is one of the common patterns for increasing system capacity. It scales horizontally until the database becomes the bottleneck in performance.

However, on a fundamental level there are almost always three main parts:

* Client.
* A web server that listens to requests.
* Programming language process. Compiled (e.g. Java) or interpreted (e.g. PHP).

Technologies that power those components are usually grouped into *frontend* and *backend*.

## Frontend

On the frontend, you typically have a browser and everything that makes up a web page. This includes HTML, CSS, and Javascript. Both CSS and JS have a large number of frameworks and libraries.

Below are what I consider major frontend technologies.

CSS:

* [Bootstrap](https://getbootstrap.com/)
* [UIKit](https://getuikit.com/)
* [Foundation](https://foundation.zurb.com/)

JS:

* [jQuery](https://jquery.com/)
* [UnderscoreJS](http://underscorejs.org/)/[Lodash](https://lodash.com/)
* [Angular](https://angular.io/)
* [ReactJS](https://reactjs.org/)
* [EmberJS](https://www.emberjs.com/)

Interesting enough, the only common stack that includes a frontend technology is [MEAN](https://en.wikipedia.org/wiki/MEAN_(software_bundle)), where A stand for Angular.

It’s also useful to know frontend build/packaging tooling: [Gulp](https://gulpjs.com/), [Grunt](https://gruntjs.com/), [Webpack](https://webpack.js.org/) and [NPM’s build capabilities](https://docs.npmjs.com/cli/run-script).

If you are a frontend developer, you should be proficient in at least few of those tools and be familiar with the rest.

## Backend

On the backend, we have everything that’s responsible for handling client requests. This includes CDN caching, load distribution, SSL, web servers, programming language interpreters/compilers, databases.

Load distribution allows horizontal scaling when you just throw more hardware in and let a load balancer do the thinking about where to route next request. Learn more about load balancing here: [https://en.wikipedia.org/wiki/Load_balancing_(computing)](https://en.wikipedia.org/wiki/Load_balancing_(computing)).

Web servers are usually powered by Apache, nginx or IIS. Their main job is to serve requested resources. A resource can be a simple text file or dynamic content generated by a program.

Programming languages are used to generate dynamic content based on request parameters. Most popular languages include: Java, Python, Ruby, C and PHP.

A program written in one of those programming languages might use a database to store and query data. Most common database technologies include Oracle, MySQL, PostgreSQL, MongoDB and many others.

## Conclusion

In this post, we outlined what is a technology stack and how it plays a role in a makeup of any existing web server. We also learned that it is beneficial to know your technology stack because it will make you a more successful developer in the long run. You’ve also seen how a typical stack is broken down into frontend and backend with their own sets of technologies.
