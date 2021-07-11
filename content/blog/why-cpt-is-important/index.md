---
title: WHY IS CONTINUOUS PERFORMANCE TESTING (CPT) IMPORTANT?
date: "2021-06-23"
description: "Nowadays, users don't stay longer than a second on your site and that's why checking your site's performance has become a game changer. Learn how to implement continuous performance testing to obtain outstanding results and decrease your website's bounce rate."
---

![Kolleen Gladden - Unsplash](./kolleen-gladden-unsplash.jpg)

According to WebsiteSetup, a site specialized in growing web apps, when load time decreases by 0.1s, retail customer engagement increased by 5.2%.  Also, “regardless of the industry that you’re in, it’s critical that all businesses develop fast web experiences. If your main competitor has a better site and page speed than you, that competitive gap will grow wider”. Meaning, the performance of your web app, mobile app, or any type of platform is an essential factor for a successful business strategy.

## But what is performance anyway?

Performance is a set of metrics that measure how your platform is using its resources, meaning, how the code is taking advantage or disadvantage of the computing power.  

The problem is that many teams do not give performance the importance that it deserves. Some only execute a couple of performance tests before releasing the product. When the client runs tests, they find a slow product with infinite load screens and are not impressed with the result.  

Bad performance applications can lead to several outcomes, and most of them are negative ones. For example, if you provide software solutions or own an app with an e-commerce component, you may lose clients due to poor performance. Best-case scenario, which isn’t a great one, you will potentially waste money in the process of having to refactor your application. While it may not be all about money; it will also cost you time since you will need to execute more testing to find the problems you're having with your product; and believe me, finding performance problems is a nightmare! Especially when your product is in the production stage. There are specialized tools called profilers that help find bottlenecks and inefficient code but using these tools can be challenging.

> So, performance is important, right? The next question should be, how can I measure the performance of my application?  

Here is a list of some key metrics that you should measure from the very beginning of the development:

1. Average response time: It is kind of obvious, isn’t it? The main metric is how much time it takes your app to show results to the user. In almost all apps, it’s a combination of the time that your backend services take to respond, plus the time that it takes for the frontend to render the data. Usually, most of the time is spent in  backend services since they take care of processing data and returning it in a presentable state.
2. CPU Usage: This is a more specialized factor, and it’s usually taken into account only for high-performance applications or applications with a huge amount of data to process because it can take a lot of time to complete the task. In these cases, CPU efficiency becomes a key factor that can save you a lot of money if you do it correctly.
3. Request rate: this is how much traffic your application receives and how the traffic behaves.
4. Throughput: is the effective rate of the request processed by the system, this is an important metric, one that tells  if your system is degrading.
5. Error rates: there are 3 different ways to track application errors:
6. Application instances count: Scaling is a huge topic, and it is tightly related to performance. Currently, this metric is measured by having a statistic of how many instances  applications are running in different periods.
‍
## Let’s focus on the average response time.  

I have seen many projects do load and stress testing at the very end of the development lifecycle, as a final step, like another item on a checklist that must be approved before releasing the product.  

‍The wait until the end approach can be problematic. What if the results are not good? Are you going to tell your client that you need another month to fix some issues? This becomes a challenging situation since you probably have a short amount of time before release. For instance, if you checked your product at the end of the process and noticed that a transversal library within the application is causing performance problems, you won't be able to fix the problem within your deadline. Many things can go wrong, and one of the best solutions is Continuous Performance Testing (CPT).

## WHAT IS CONTINUOUS PERFORMANCE TESTING (CPT)?

Are you familiar with Continuous Integration? If you are not familiar with the concept, then it’ll require for you to test your code continuously and automatically for defined periods and gather the results of those tests to analyze them and make conclusions about the state of your product regarding performance.

Sounds easy, right? Continuous performance testing is an important task that can save you time and money, but performance is a variable that must be considered in every stage of the development lifecycle.

## PERFORMANCE IN THE DEVELOPMENT PROCESSES

### PLANNING STAGE
‍
You have a new business proposal, an app that will change the life of a thousand people, a million people, a billion people. How many people? There are several questions to ask in this stage. This is the stage where you and your client define the performance targets. Performance targets are subjective, and they depend on the necessity of the project and the business logic. Some things take time, and you cannot pay for a quantum computer to deploy your app yet. But in general, most of the apps sell things and they require competitive load times.

Good questions you should be asking in this stage:

- How many transactions per second are we going to reach?
- How many concurrent users are we going to have?
- What is the amount of data that should be processed at any given time?
- Is there a scaling plan?

### DEVELOPMENT STAGE

‍Apply CPT. The developers need to be pushed to squeeze the best performance of the tools they use. How? CPT must be about testing your app as a whole, starting from its parts. You must measure the impact of every new development in the fluxes of your business logic. If a list in a screen takes 20 seconds to load and the other parts take only 1 second, then your screen loads in 20 seconds.

Everything must meet the performance targets and let’s be honest, developers, most of the time, do not check that. They have a lot of tasks per sprint, they must attend meetings, they must run other tests, and at the end, they only care that everything works well. Performance tasks should be generated as another task of the sprint or whatever agile methodology you are using. CPT must give you constant feedback on the performance of the app, and if something is compromising the targets it must be fixed during the development stage.

### PRODUCTION STAGE
‍
There are several things to talk about here, but let’s focus on one thing: Monitoring. Things can go wrong even if you applied CPT during the development stage that can be attributed to infrastructure reasons, last minute changes, third-party issues; there is just too much that can go wrong. But do not worry, everything has a solution, and the first step is to detect the problem.

There are a lot of tools for monitoring every type of product, mobile, web, desktop, and others. Find the one that fits your necessities and use it wisely. Sometimes the reports are not clear, so you must define a strategy to capture your application’s meaning traces and logs to easily detect what is failing.

CPT is a transversal operation, and it involves a lot of profiles. The managers of the projects must be aware of the performance metrics and push for the best results. The people in charge of applying the agile techniques must create the tasks (it should be automatic in the best scenario) regarding performance issues.  

The Devops should create the infrastructure to apply CPT. The developers should improve their skills and learn the best ways to apply the implementations to get the best performance results from their code. And last but not least, there should be someone related to data science and analytics, who can get the best insights from the information that is being gathered in the CPT process.  

Trust me, if you apply it well, there will be a lot of information to process.  

## HOW TO START WITH CONTINUOUS PERFORMANCE TESTING?

1. Have a CI process: Yes, you need a CI process already in place, you need a pipeline that execute tasks over your project automatically. Do the testing: I’m currently using Taurus; it is a tool that helps including load testing on CI processes. You must define load tests that measures the performance of your app and find a way to process that information. This is just a tip on how to handle the situation. Every company must find a way to handle the data to get the best results possible.
2. This step requires a person related to data science and analytics. Extract conclusions from those tests. What is going well, and what is not?
3. Finally, you must provide feedback to the developers. They need to know that there are problems, and they need to know as soon as possible. There are companies that have this performance culture so deep in their roots, that developers know that their code is affecting the performance the next day after they’ve run their code.

> Performance is essential and must be considered from the beginning stages of each project. A very good way to prevent releasing your product with performance issues is to apply CPT during development stage! There are many other ways you can tackle this issue, but this will depend on your specific needs and it’s important for every company to find its way.

Originally published [here](https://www.leangroup.com/blog/why-is-continuous-performance-testing-cpt-important)