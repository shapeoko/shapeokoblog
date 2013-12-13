---
layout: post
title: Update: Y axis - smooth and awesome!
date: 2009-11-26 13:37
author: smadmin
comments: true
categories: [arduino, cnc, diy, electronics, Shapeoko, sparkfun]
---
The Sparkfun forum guys really helped me out. After getting the Y-axis stepper up and running with the Arduino, there were some issues. Mostly it was loosing steps in a bad way. Plus, the vibration threatened to tear my machine apart! OK, that last bit was an exaggeration, but the vibration was pretty bad.

The guys on the forum pointed out that you can't just start a stepper at full speed, you have to "ramp up". Which after thinking about it, makes perfect sense. At this point in time, i've learned enough to know that in most cases, "it's already been done". Meaning, there was no need for me to write new code to "ramp up" the arduino. I mean, there are tons and tons and tons of stepper based arduino projects on the web, surely someone must have written some good code.....

The short answer: Yes, it's out there . But, the really surprising part is, that link is the only one i found where the steppers were "ramped up". Now, don't get me wrong, it WORKED! Check the video for proof of that. The difference with a smooth start is night and day compared to just the standard method. BTW: the standard method is: Start a loop, Pull step pin HIGH, put step pin back to LOW, delay for a set amount of time, loop. Most people just set the delay to something that won't stall their motor. This varies greatly depending on the specs, but for the most part people are between 200 and 400ms. I guess I'm wondering why more people don't start smooth? maybe it's just easier to set the delay and forget it... who knows. Either way, I'm really happy with the progress so far. Things are starting to come along.

<iframe width="640" height="390" src="http://www.youtube.com/embed/0WSgnEOx7fQ" frameborder="0" allowfullscreen></iframe>
