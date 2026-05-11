---
title: Power Platform vs AI Coding Part 1
date: 2026-05-11
lastmod: 05/11/2026
description: A bit of a rant about AI making low-code solutions obsolete
summary: ""
tags:
  - AI
  - CoPilot
  - Microsoft-Power-Platform-Admin
categories:
  - AI
series: []
draft: false
toc: true
---

## The Problem with the Power Platform
I have had a mixed relationship with Microsoft's Power Platform over the years.   During its initial roll-out I was very excited.  However over time as I became the one who had to manage, maintain, and upgrade the Power Platform objects that citizen developers (often those who had left the company) created,  I began to feel jaded about the whole thing.   

Microsoft has attempted to address this,  with tools like the Power Platform Centre of Excellence and some improved administrative tools.   However these are almost exclusively reactive,  they look at what has been done,  rather than control what can be done.   Combined with the Power Platform's implicit connection mapping it makes enterprise management difficult.    

The other issue with PP Apps / Flow is that they hit a complexity wall.   For example if you want an app that has a complex approval workflow,  the native Power Platform solution will struggle,  for simple approval workflows it is fast and easy,  but add 10+ approval layers,   multiple stage-gates,   long term parking,  and suddenly you are looking at many Power Automate flows chained together,  that are hard to manage,  debug and develop.      

In general I have found that the Power Platform is hard to scale to a true enterprise grade solution, it can be done but requires a team of dedicated Power Platform developers and administrators, and if you need dedicated staff,  what is the point of the low-code solution in the first place?  

## What AI Coding assistants bring to the table

*My experience in this area is mostly with GitHub Copilot,  though other AI Coding assistants should function in a similar fashion*

I will be upfront, I like code first solutions and always have.   They have always seemed more stable,  more sustainable,  and honestly more joyful to work on.   The feeling of finally getting some piece of code to work is a reward unto itself,  when that happens there is usually an 'ah-ha' moment of joy when you realize what you have been doing wrong.   Compared with low-code/no-code solutions the moment of getting it to work is usually a 'huh' moment,  followed by a 'shit' moment when it stops working again for no reason you can see. 

The issue with code first solution is the learning curve.   For my entire career I have worked in end-user organizations which means that the only value coding custom solutions brings is the improvements they can make to the organization's actual value-add activities.   That is a long way of saying that code development(and IT in general) is usually seen as a cost centre,  not a value driver.   

So writing a beautiful code first solution that only a handful(or less) people in the organization can understand is a hard sell.  Instead despite its many flaws low-code solutions like Power Platform can more easily be adopted even if they are harder to manage long-term.  

AI Coding agents change the math on this.   
1. Coding agents are great at reading and writing code
2. The agents dramatically reduce the steep learning curve of approaching a traditional code-first solution
3. GitHub is being integrated rapidly into more control surfaces,  meaning a wider range of workers at an organization can leverage the coding agent.  

## My future vision of citizen developers
First and foremost I believe that as AI coding agents improve they will make traditional UI driven low-code solution obsolete.   In fact organizations that stick with low-code platforms will be held back because those platforms were never designed with enterprise grade SDLC in-mind,  that modern SDLC is exactly what AI Coding agents excel at leveraging.  

In my head here is a future scenario:
1. A group of business subject matter experts have a meeting to discuss shortcomings of a business applications.   For this example let's call the app 'Pricing Builder'.   In the meeting the group discusses several potential improvements to the app.  
2. Copilot transcribes and summarizes the meeting, it recognizes the potential improvements to the app and generates GitHub issues describing the improvements.
3. The application's business owner is notified of the potential improvements ,  they review the GitHub issue and if it looks good assign it to a GitHub coding agent to work on.  
4. The agent completes the requested improvements,  creates a pull request to be approved by the application's technical owner.
5. Once the PR is approved GitHub Actions take over and deploy the improved app to a test environment.
6. Another agent sees the updated issue ticket and notifies the original SMEs that an improved version of the app is ready for testing. 

The scenario is enabled by several things that are achievable for end-user organizations who do not have large IT or development staffs:
- Well built GitHub Repos
	- Documented design patterns
	- Documented existing application designs
	- GitHub actions to automate CI/CD
- AI Context of how the business operates (like Microsoft 365 Copilot's Work IQ)
- AI Coding agents that can follow the Repo instructions and guides
- Applications developed in a platform that lends itself to agents editing the solution


Put this together and there is no need for old-style citizen development platforms.  Instead, non-technical users simply ask for solutions and AI Agents build them based on guidance.  The role of developers inside the organization becomes one of creating the guidance and guardrails the AI coding agents will follow.  
