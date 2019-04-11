---
layout: post
title: Where Do You Put Your Fast Lane?
date: 2019-04-11 08:38:00
tags: cloud people networks
author: jon
---

# Random thought on the Datacenter in 2019

## Huh?

I'm going into a meeting about the needs of our datacenter in 2019, and planning what sorts of switches (networking) that we're going to need in the coming years.
Something struck me about this questions.  The majority of our critical services are run in the cloud.  Canvas, our Learning Managment System and O365 make up the proponderance
of our network traffic.  If that's the case, then what's the need in faster-than-10gbit connectivity on premise?

## Two Places

I see two places where that high-speed might be neccessary.  First thing, Storage.  East-West traffic in a SDS system is pretty big.  You've got each node chatting away with its family members and talking to the presentation layers.  When it gets to the end customer, its not really the whole of my stakeholders talking to that storage, its a few groups with
highly specicalized needs (GIS, Archival Storage, Video) where there are a few, but not a lot of simultanous users.  Maybe a 100 at a time, admittedly they are hungry, but faster-than-10gbit
to the desktop isn't really a thing for us.

Second place, the interconnections between our client "zones" the traffic between the totality of our Wireless and Wired clients and the Internet.  Since the majority of the traffic is LMS, O365
and YouTube, the "on-ramps" to the internet need to be the next big pipe.  In that milieu of traffic, the datacenter is just another client.  Backups, syncronizations & stuff are peanuts compaired
to FortNight videos and Spotify.  

## Totally Sure

I'm absoutly positive I've missed something, but it was an interesting thought exercise.

[back](./)