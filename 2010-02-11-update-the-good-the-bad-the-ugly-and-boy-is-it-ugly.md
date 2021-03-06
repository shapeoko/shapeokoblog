---
layout: post
title: Update: The good, the bad, the ugly (and boy is it ugly!)
date: 2010-02-11 21:37
author: smadmin
comments: true
categories: [arduino, cnc, diy, easydrivers, electronics, Shapeoko, sparkfun, workshop 88]
---

While doing any long term project you are bound to run across three things: Good things, bad things, and downright ugly things. It's part of the territory. In fact, for a hobbiest, these are the things that make a project a project!

The Good:
A short blip about the project was mentioned in a recent article on Tom's Guide. Grant it, after seeing the posting on Sparkfun, I was actively pursuing being featured in the article, but none the less we made it in! That pretty much made my week.

The Bad:
Last Saturday I drove to a "local" (2 hours away) hackerspace meeting to meet up with fellow geeks and check out what other people have been up to. A couple of bad things happened: Only 2 people showed up (not including the host and hostess). This ended up being OK as the the host and hostess did a fantastic job of making us feel welcome. Even with the limited number, we managed to bottle some beer and have a generally good time BSing with each other. 

Worse: I tried showing off my mill project (yes, I brought it with me!) but for some reason, I couldn't get it to work. I thought that during the trip something on my protoboard became disconnected.

After all, it was the first time I had moved the machine and with extensive use of a breadboard, it wasn't exactly in mobile form to begin with. After troubleshooting for about 15 minutes, I couldn't figure it out and just packed it up. Not a big deal. I figured I'd get it running once I got back home.

The Ugly:
After making the 2 hours trip back to my house, I unpacked the mill and took it back into the Lab, hooked everything back up, put the meter to a few key connections, then tried to give it a test run. Nothing. OK. It had been a long day, I unplugged everything and let it sit.

After a few busy days of domestic duties and work, I had some time Tuesday evening to work on it. After messing around disconnecting the easy drivers from the protoboard (not an easy task!) and simplifying my circuit to only one axis and a simple (known working) sketch. I couldn't get anything to work.

I emailed the creator of the Easy Driver and asked him on a couple of things. Being the generous person he seems to be, he replied with a few tests (procedures) to check if the drivers were fried. Long story short: They were.... All three of them were fried! Here's a couple of pictures of my metering.....




To make matters worse: I fried my Arduino too! It seems that when I tried to demo my machine at the hackerspace meeting I crossed the +24v from my Power Supply and the GND, which essentially meant that I sent 24V into the arduino and then into the Easy Drivers. Both of which were only expecting 5V....

Right now I have a new Arduino on its way from Sparkfun. I will order the easy drivers tonight. In the meantime I'm hoping to learn how one may protect against accidents like this....

But I'll stay positive because, to steal a quote from Dostoyevsky, "A just cause is not ruined by a few mistakes" :)
