---
title: "Unified Developer Experience: An Introduction"
date: 2026-03-30T19:58:43-04:00
lastmod: 2026-03-30T19:58:43-04:00
description: ""
summary: ""
tags: []
categories: []
series:
  - '["Unified Developer Experience"]'
cover:
  image: images/cover.png
  alt: ""
  caption: ""
draft: true
toc: true
---

# Introduction of an Introduction

First off a word on terminology.  I will be calling Microsoft Dynamics 365 Finance and Microsoft Dynamics 365 Supply Chain Management,  D365 F&O from here on out.  If and when Microsoft changes the name to add AI or Co-Pilot to it,  I will still call the product D365 F&O,  which is progress because I am not going to calling it DAX.

As a long-time user of D365 F&O the thought of moving away from LCS and cloud-hosted development VMs is both exciting and terrifying.   It has taken years but I am finally just getting used to developing in this cloud based world, and Microsoft is changing the rules again.   Well change is nothing if not constant. 

# OK Now What
As the D365 F&O ecosystem moves away from LCS to PPAC(Power Platform Admin Centre) D365 F&O professionals need to adapt and embrace this new tooling.    Of particular concern to this series is the Unified Developer Experience.  

The UDE is the next generation of development tools and processes for developing in the D365 F&O software stack.     The biggest change it makes is to move the D365 database and application layer from the LCS Cloud-Hosted VM to a Power Platform environment.  This means that UDE environments are as capable as a full production environment,  including all connections to Power Platform.   This makes developing Dynamics cross-application solutions much easier.  

# The UDE Series
This blog series will cover the end-to-end implementation of UDE at a mature D365 F&O customer.  Many topics will be covered as part of the migration from LCS to UDE.  

## PPAC Environment Management
How to provision UDE environments, including copy options.   This is one of the biggest changes compared to LCS Cloud-Hosted environments

## Dataverse Storage costs
This is a big one,  when deploy a UDE environment,  it lives in dataverse, and dataverse is expensive.  So expensive that depending on your D365 F&O db size it could make the Azure VMs that LCS is based on look downright reasonable.   

The good news is that Microsoft is aware of the concern and changes are coming. 

## Local Development VM
Just because it is possible to set-up your personal PC to be a development client for UDE doesn't mean it is a good idea.   I will be covering how to set-up a fresh VM to connect to and develop against a UDE Environment


## Unified Sandbox Environments
What are they?  How do their compare to Tier 2+ LCS environments? Why are they called USE but Unified Developer Experience Environments are called UDE Environments?  At least some of these questions will be answered. 


# Closing Thoughts
I will be documenting the process of migrating from LCS Cloud-Hosted Developer environment to Unified Developer Experience Environments in real-time as I do it.   You should expect that mistakes will be made, and incorrect statements said with confidence.   I will do my best to update posts as I find out the right answer.

Also it is important to note that I represent only myself in the opinions and guidance I provide.  As always it is worth what you paid for it. 

If you my reader should decide to follow my advice and guidance,  remember don't fuck it up. 