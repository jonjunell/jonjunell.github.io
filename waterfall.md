---
layout: post
title: You can't Iterate a Waterfall
date: 2018-09-10 19:34:00
tags: infrastructure cloud people
author: jon
---

# You can't Iterate a Waterfall

## Overview

It's my general impression that _most_ enterprises have a very close relationship between the project managment team and IT Ops.

Before starting your amazing new project, you really, and I can't emphasize this enough, it is your responsiblilty to communicate how there is not a static system anymore.

In the migration project, the project manager and I had worked out what we called the "green line."  The line represented that there wasn't going to be a final verion of anything, really ever.

The issue was, and this is very clear now, that we didn't break out all those sperate tasks and declare timelines.  I had only developed a rough plan:  

* Build IaaS
  * The Highest Cost, lowest "challenge"
* Move to PaaS
  * Convert those messy full stack TomCat VMs to PaaS instances
* Move to SaaS

Because there were deadlines to hit on a tight schedule we found our selves meeting the deliverables, but not the improvements. This satisfied the project timeline, but not the spirit of improvement and over time we had plenty of things running in Azure, but not leveraging the power of Azure.

We'd meet the time and things would "work".  This introduced latency in the system and circuitus routing.  Additionally it increased the difficulty in troublshooting, configuration,management and accountablity.

### Take Away

Be clear!

Articulate, very clearly, what is required for the technical challenges to be overcome.  Don't settle for a green line, settle for clear, informed timelines, otherwise, you're buying more on-premise hardward, or more than you planned to have.  IaaS vs. a Container eats up a lot more resources.

[back](./)