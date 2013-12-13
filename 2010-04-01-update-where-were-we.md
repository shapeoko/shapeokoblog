---
layout: post
title: Update: Where were we?
date: 2010-04-01 15:38
author: smadmin
comments: true
categories: [arduino, cnc, design, diy, electronics, grbl, project, Shapeoko]
---
.... Oh yes, building a mini CNC machine!

<strong>A couple of things happened shortly after the NES success of late February:</strong>
<ol>
	<li>Burnt up another EZ Driver</li>
	<li>Burnt up ANOTHER 2 EZ drivers!</li>
	<li>Got completely side tracked on trying to design a circuit to hold an Allegro A4983 chip</li>
	<li>Was completely side tracked trying to stream gcode from one Arduino to another</li>
	<li>Took a break.</li>
</ol>
<strong>Scope, focus, project goals</strong>
As I mentioned in a <a href="http://www.edslifedaily.com/1/post/2009/11/update-mill.html" target="_blank">previous post</a> there are certain times during a project when you need to step back, regroup, and find your focus. This past month was one of those times for me. After taking a 20,000ft view of the project I decided that in order get past the current hump, I need to straighten out my electronics setup, and just quit messing with it. It seems that because I’m so intrigued by the electronics portion of the project (it’s the newest and most interesting part of the process for me), that I have had a hard time just letting it be, so that’s what I’m going to focus on: Getting the electronics assembled, configured, and hooked up. THEN LEAVING THEM ALONE!

<strong>Electronics</strong>

For now I have abandoned the <a href="http://www.sparkfun.com/commerce/product_info.php?products_id=9402" target="_blank">EasyDrivers</a> in search of something that can give my motors a little more oomph. While trying to design a circuit around the Allegro A4983, I ran across <a href="http://www.pololu.com/catalog/product/1201" target="_blank">this product</a> by Pololu. Which had essentially done what I was trying to do, however thier version is much neater than I could have done. After Ordering 3 boards, and testing them out on the breadboard, I’ve set about making a more permanent solution to mount them in.

[PIC]

At this point, the goal is to finish implementing/troubleshooting/debugging the electronics by the end of the weekend. This should free me up to move on to more important things…..

<strong>Software</strong>

If the electronics are setup, and I’m OK leaving my design the way it is (for testing purposes) then I need only focus on implementing the software. Luckily, it looks like <a href="http://labs.bengler.no/-/bulletin/show/556650_micro-w-grbl-first-cuts?ref=mst" target="_blank">Simen has really kicked ass in the software department</a>. All I need to do at this point is get the newest version of GRBL flashed to my Arduino and maybe do some fine tuning on the stepper settings (rapid and default federates). Then: TEST!

That’s it for now. Here are some pictures of a couple setups and some new bits...

&nbsp;
