---
layout: post
title: Update: SWARF! (of the wood variety)
date: 2011-05-31 22:47
author: smadmin
comments: true
categories: [arduino, DumpsterCNC, grbl, Milling, ponoko, shapeoko, Shapeoko, sparkfun]
---
<iframe width="640" height="390" src="http://www.youtube.com/embed/Gkr86X5UvOM" frameborder="0" allowfullscreen></iframe>

After taking off several months, I've hit the shapeoko project pretty hard over the last few weeks. There was a lot of pre-work involved (unpacking boxes, remembering where I was at) but I finally got the mill setup in my new garage and plugged everything in.

It took a few days for me to get back up to speed on the project but after getting my bearings I decided the first thing to do was load up Simen's <a href="https://github.com/simen/grbl/downloads">newest version</a> of GRBL (v0.6b). The addition of speed acceleration was too good of an upgrade to decline. It was a pleasant surprise to find that the loading process had been improved dramatically! Where as before I was building from scratch and loading with my pocket programmer from sparkfun, now it's a simple hex file download from github then a quick hex file upload to the arduino via <a title="Xloader" href="http://russemotto.com/xloader/" target="_blank">XLoader</a>. It's so easy I feel like a script kiddie using it. But as they say, one must pick their battles, and building from source is a battle I'll gladly stay out of :)

My next hurdle was to figure out how the F*** i was going to mount the dremel. What seemed at the beginning of this project to be the easiest thing to do had ended up being harder than I imagined due to the non-symetrical nature of the dremel. However, after purchasing a 100 series and looking at a few websites I came up with a makeshift arrangement based mainly on an <a title="Dremel Mount" href="http://www.instructables.com/id/Simple-Rotary-Dremel-Mount/" target="_blank">instructable</a> I found. I have plans to make this better, but for now it works just fine. The main issue being clearance, with a standard 1/8" dremel bit chucked all the way up, there's just enough room to slide in a 1" x piece of stock, but then leaves little room for safe z-height clearance. I have a few ideas but would really like to cut out the prototypes myself, so we'll see where that leads us.

As for now, here are two videos. One of the mill in action, the other taken after the job had completed. I wanted badly to run another pass cutting a little deeper into the material but due to the time of day (late!) I didn't think my neighbors would appreciate the continued ruckus coming from my garage. Plus, the stock was really crappy. Tomorrow we'll try UHMW.

Which reminds me: I'll be building a styrofoam enclosure tomorrow as well. The machine isn't loud at all, but the dremel is pretty load and amplified in my garage with the wood walls and cement floor. A quick pink styrofoam enclosure will be a simple fix. I might even put a piece of plexi on the front so I can see what's going on while the mill is running.

<iframe width="640" height="390" src="http://www.youtube.com/embed/DFMW4U8q_1w" frameborder="0" allowfullscreen></iframe>

Apparently "really really well" is the best description my feeble mind could think of while shooting the post-successful milling video. After listening to it back I realized I said everything was working "really well" over and over again. Oh well.

