---
layout: post
title: Attempted Clouds
date: 2018-08-10 19:34:00
tags: infrastructure cloud people
author: jon
---

# All about our Hybrid Cloud Attempt

## Overview

My instituation attempted an ERP migration to the cloud.  It went, in a direction.  Lessons learned, ignored and something happened.

## Current State

Beacuase of _reasons_ We expanded our current private cloud environment to accomodate the current batch of Database servers, and all the associated services that connect to the Banner ERP.

## What _is_ Banner

Banner is a academic ERP.  It manages Finance, Student Services (admission, registration, classes & curriculm), Human Reasources.  In the current EOL version it runs on Oracle WebSphere (Tomcat stuff) for its front ends (for user self service), Oracle Forms for administration and an Orcale DB backend.  There are lots of connected systems.  My instituation has run Banner in various forms for over 20 years.  It's been on Linux hosts for the last 8, and before that it lived on Sun Solaris hardware.

## Why Now

Ellucian, the provider of Banner is upgrading to a newish architechture, where they allow you to drop the Oracle WebSphere & Forms services and replace them with multiple servers running Tomcat.  It feels like general improvement, it makes it much more browser agnostic (Banner 8 was only really viable inside of IE) and modern (you can now resize the window).

## Deeper Dives

* [You Can't Iterate a Waterfall](https://jonjunell.github.io/waterfall.html)
* [Enterprise over IP](https://jonjunell.github.io/vpn.html)
* [Coping with Infinity](https://jonjunell.github.io/cloud.html)

[back](./)