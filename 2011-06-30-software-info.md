---
layout: post
title: Software info
date: 2011-06-30 12:13
author: smadmin
comments: true
categories: [arduino, grbl, phlatboyz, Shapeoko, sketchup, Software]
---
I've received quite a few questions since the <a href="http://www.kickstarter.com/projects/edwardrford/project-shapeoko-a-300-complete-cnc-machine">kickstarter launch</a> relating to software.

For anyone who is starting something new, it's often difficult to wrap your head around the process and adding "options" to the process makes it seem more complicated. At least that's how I work. For anyone who is new to this whole thing, it might seem overwhelming at first (it was for me). But trust me, it's not! Most of confusion comes from all of the options. But, when you boil it down to it's simplest form it's actually quite easy.

<em>Side note: There are <del>100</del> 1,000+ different ways to do this. If you're comfortable with the process, feel free to insert your own solution into any of these steps.</em>

<strong>The process goes like this:</strong>
1.) <strong>CAD:</strong> Draw something in a CAD program (or any vector program such as Inkscape).
2.) <strong>CAM: </strong>Convert your CAD drawing into gcode. Gcode is the format that the cnc controller uses to tell the machine where to go. Think of it like X,Y coordinates with some extra stuff included.
3.) <strong>Stream: </strong>The process of sending your the newly created gcode from your computer over to your mill.
4.) <strong>Controller:</strong> On the other end of the stream is your CNC controller. The controller is what recieves the gcode from your computer and changes (interprets) that gcode into pulses. Those pulses are what tell your stepper motors to turn. The truth of the matter is that once you get your controller setup (in our case we're using GRBL loaded on an Arduino) you will probably never have to worry about it again.

<strong>Here's my current stack:</strong>

<strong>CAD</strong>: <a href="http://sketchup.google.com/intl/en/download/index.html">Google Sketchup</a>
<strong>CAM</strong>: <a href="http://sketchuppluginreviews.com/2010/04/30/phlatscript-google-sketchup-plugin-review/">Phlatboyz Sketchup Plugin</a>
<strong>Streamer</strong>: stream.rb (a bare bones ruby script included with every version of <a href="http://dank.bengler.no/-/page/show/5470_grbl?ref=mst">GRBL</a>)
<strong>Controller</strong>: <a href="http://dank.bengler.no/-/page/show/5470_grbl?ref=mst">GRBL</a>

We're always open to suggestions so if someone else has a sure-fire dead simple stack, we'd love to hear about it!
