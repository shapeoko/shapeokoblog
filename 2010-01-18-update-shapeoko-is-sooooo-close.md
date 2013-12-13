---
layout: post
title: Update: Shapeoko is sooooo close!
date: 2010-01-18 20:00
author: smadmin
comments: true
categories: [arduino, cnc, design, diy, easydrivers, electronics, grbl, Shapeoko, sparkfun]
---
<div>What a long long night...

grbl is definitely installed on my arduino. That is good news! Actually it's the only good news for the night.

After getting home from work and getting the regular chores done, putting the baby to bed, and spending some time with my wife, I headed to the basement to put the final touches on this fantastic project. Honestly, I thought this was going to be "the" night. I couldn't have been any more wrong.

First: my lab is a disaster, which I had forgotten about because it's been at least 3 weeks since I last stepped foot in there. It seems that I was using it for "temporary" storage during the holiday season, and have since neglected to remove the temporary items. OK, spent 10 minutes moving stuff around enough so I could at least sit down and reach all of the components.

Two: The battery in my D630 laptop is totally gone. If I unplug it for a second, I get a critical beep and then BAM. power off. I should note that I'm using a power strip as an "e-stop". So, forgetting about the battery deal, i plug in my laptop, power up, log in, load the desktop (at least a 7 minute affair) and then decide to throw the power on the strip because I realize my soldering iron is plugged in. BAM, laptop powers off. I proceed to do this not once but TWO more times before i finally get smart an plugin to a dedicated strip.

Three: I hadn't exactly completed breaking out the STEP/DIR pins for each axis. Not a huge deal, but i did have to strip some wire and do a quick bit of soldering. Here's a picture of the proto board fully loaded.</div>
<div>
<div><a rel="lightbox" href="http://edslifedaily.weebly.com/uploads/2/5/6/1/2561031/916650_orig.jpg"><img src="http://edslifedaily.weebly.com/uploads/2/5/6/1/2561031/916650.jpg" alt="Picture" /></a></div>
</div>
<div>In retrospect I should have done some color coding for step/dir and especially for the motor harnesses. Chalk that one up under being a rookie I suppose...

OK, so now that everything was setup, I was ready to manually send gcode to the arduino via the serial monitor in the arduino IDE. Laptop is powered up, arduino is connected via USB, XYZ axis' are connected to the arduino. All Set:

I power up the 24v Power supply and everything goes crazy. The X axis is wobbling back and forth, the Y axis is stalling itself out, and the Z axis was making a really creapy humming noise. Power off. Quick.

After trying a few more times, and double checking the pinouts in Simen's config.h file. I couldn't locate the problem. All I know is that if I don't hook up the arduino then everything is fine. The motors will sit there quietly, and everything looks like it's in order. But, the moment I hook up the arduino... bad stuff happens. Here's a video demonstration.


</div>
<div>
<div><object width="400" height="330"><embed type="application/x-shockwave-flash" width="400" height="330" src="http://www.youtube.com/v/lZuz0xWGKIM" allownetworking="internal" wmode="transparent"></embed></object></div>
</div>
<div>So, like I said: That's it for tonight. I'm going to enjoy this delicious Pale Ale from Bell's Brewery and go to bed. Maybe tomorrow will be the day?</div>
