---
layout: post
title: Enterprise over the Internet
date: 2018-09-11 19:34:00
tags: infrastructure cloud people
author: jon
---

# Overview

Banner is actually "simple." It consists of a set of front-end servers, with a backend database.  The challenges start with how those features are implemented and how much customization has occured.

## Banner 9/XE

With Banner 9, you migrate away from Oracle Forms and toward Tomcat-based webservices.  However, the cool thing is you can keep Banner 8 running at the same time you're staging up the new Web fronts.

## Introducing the Internet

Because we had decieded to go with a cloud native deployment of Banner 9, we by design, introduced the Internet into our ERP.

Pro-Tip: _That's a bad idea_

Because the databases had to remain on-premise to guarentee the stability and performance to the Banner 8 system, it couldn't provide consistant connectivity and performance to the Banner 9 system.  

Compounding this, because everything was running over a VPN, not only did the internet have to stay up, but the VPN as well.  For those keeping score:  That's 2 technical requirements, managed by 2 teams.

## On the PM Side

During launch of Test in June, it became apparent that collectivlty we had no ability to force/encourage/cajole any of the Banner 8 users to migrate to Banner 9.  This meant that we'd be running both 8 & 9 for the forseeable future..

..over the internet

..on a vpn

## So?

This was the first real "this isn't going to work moment."  If we were going to commit to Azure, our options and times were closing.

These were our cloud oriented options

* Build Banner 8 completely in the cloud, from scratch
* Force a dump of Banner 8, everyone's using Banner 9

## 3rd Rail?

Punt, buy on-premis hardware to accomodate the database servers.  So, we saved the project.  Our cloud aspirations? GG.

[back](./)