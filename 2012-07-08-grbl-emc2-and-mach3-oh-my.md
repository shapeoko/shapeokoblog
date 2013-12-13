---
layout: post
title: GRBL, EMC2, and Mach3...oh my!
date: 2012-07-08 10:17
author: smadmin
comments: true
categories: [Uncategorized]
---
When you start down a road that you haven't traveled before, it's hard to know what you need and what you don't need. What's important and what's not important. So when there are choices, as a newcomer, it's difficult to know what is the *right* choice. With this particular project, we've tried to take away as many of those initial choices as we could yet still leave the project flexible for all types of users.

&nbsp;
One of the choices is to run the machine with an arduino (grbl) or with a PC based implementation such as Mach3 or EMC2. I'll try my best to give a brief rundown on EMC2, as it is what I have been using *almost* exclusively for several months. I have little experience with Mach3, so I'll leave that to another user.
First, we'll cover some basic concepts:

<strong>To run a 'job' on a CNC machine you need to do a couple of things.</strong>

1.) Draw something in a vector format (CAD, inkscape, Sketchup, etc).

2.) CAM what you drew in #1 (cam means to generate the gcode)

3.) Send the Gcode to the machine

4.) Interpret the gcode into step pulses

<strong>The difference with grbl vs EMC2: At the most basic level, EMC2 does both sending/interpreting.</strong>

- With grbl, you would use something like gcodesender to stream the gcode text file to the arduino. grbl then would interpret the gcode commands and convert them into pulses which are sent to the stepper drivers.  And the job is run on your machine.

- With EMC2 - you load the gcode file into the interface (usually called AXIS). The gcode is interpreted into a toolpath and shown to you on the screen. This effectively gives you a preview of what EMC2 thinks your gcode is going to produce. When you're happy with the preview, you click run. After clicking run, the gcode is interpreted into pulses and send over the DB25 cable to your controller (stepper drivers). And the job is run on your machine.

<strong>Got it? OK, good. So what's the difference after this point?</strong>

- There is a slight difference in the way that gcode is interpreted between EMC2 and grbl. (i.e. EMC2 is more robust with a larger set of understood commands).

- I also think that given the same job, EMC2 will run it faster than grbl due to the limitations of the 328p.

&nbsp;
In my opinion both of those differences are minute. EMC2 offers a better interface and better (truer) CNC experience than grbl. But, it's debatable as to whether that matters at all. GRBL was designed to be a no frills CNC controller capable of fitting on an arduino. It's simple by design. Whereas EMC2 is huge and monolithic in it's quest ot be all encompassing to all CNC operations (lathes, 6 axis machines, big machines, small machines, etc. A pretty accurate anology would be: Microsoft Word vs Notepad. Where EMC2 would be Word and GRBL would be notepad. They are both word processors, and both very good at what they do, but one has A LOT more features than the other. Some of those features are handy, some are simply unnecessary for all but the super niche users.

Are you missing anything by not jumping straight into EMC2 or Mach3? It's tough to tell because everyone's situation and expectations are different. My general suggestion to everyone is get your machine running with grbl. Get used to running jobs, get used to the machine in general and the workflow that accompanies it. Once you have that stuff down, if you feel like venturing out, go for it! The most difficult part of using EMC2 is procuring a PC with a parallel port. If you already have that, or have access to that, then in my opinion it's a great choice to use EMC2.

&nbsp;
