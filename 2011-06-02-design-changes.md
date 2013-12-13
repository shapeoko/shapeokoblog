---
layout: post
title: Design Changes
date: 2011-06-02 13:46
author: smadmin
comments: true
categories: [design, electronics, Milling, Shapeoko]
---
After running shapeoko for the last two nights, I've noticed a few things that need to be addressed:

<strong>The Y-axis has some issues (Part 1).</strong>
One of the things you'll notice in many of the videos is a certain "wobble" for lack of a better word when the Y axis travels in either direction. At first I thought this was due to a bent acme rod, but the more I looked at the wobble the less likely I thought it to be from that. Mainly because with a bent rod I figured the wobble would increase and descrease as it moved closer/further from the source. My attention turned to the coupler. But, given that it's just a straight steel coupler bought from mcmaster that seemed unlikely. Ends up, it was neither, I'm not sure to what degree, but the turned down end of the rod has a certain (non-trivial) amount of <a href="http://en.wikipedia.org/wiki/Runout">runout</a>. 

<em>*Runout, to my understanding just means that when the rod was turned down in the lathe, it wasn't done concentrically. Or, in other words, the turned down portion isn't lined up with the main body. So think of the turned down portion as being "off-center" from the center of the threaded part of the rod</em>

I was lucky enough to have a special coupler that I bought from <a href="http://dumpstercnc.com/">dumpstercnc</a> where one side of the coupler is acme threaded (1/2" -10tpi) and the other side is just a standard 1/4" straight bore. So, I pulled off the old coupler, unthreaded the rod from the acme nut, and just flipped it around. So the turned down end was now just sitting in the "dummy" end of the setup.

Imagine my delight when the wobble went away! Actually, the wobble went 99% away, so I suspect that is a slight bend in the acme rod. I'll cut a new section when my new rod comes in and see if that solves the problem completely.

<strong>The Y-axis has some issues (Part 2).</strong>
The Entire y-axis is comprised of a single 1/4" piece of MDF. However, the linear rail is mounted directly in the center via 8 x 5mm bolts. When I was designing this section of the machine I figured that the rail would give the MDF enough strength to prevent an sort of flexing. To some degree I was right. What I didn't acount for was "twisting".

<em>*Imagine holding a two foot section of wood in your hands (so both thumbs are up, like you were skiing) . If you try to bend the board (turn your hands in), that's what I'm calling "flexing". If you try to twist the board (twist one hand towards you and one hand away from you) that is what I'm calling "twisting"</em>

So the board twists at certain points of an operation. I think I'll add a few small gussets to each corner of the axis and see if that solves the problem. Otherwise I'll have to design a top "rail" for the back of the axis which would require me to build a new z-axis to fit the new profile. I'm hoping the gussets work!

Also, I'm on to a few new spindles that hopefully weight less than the dremel, are easier to mount, and may provide more tooling options. At nearly 4lbs, the dremel seems to be magnifying the twisting of the Y-axis because of it's cantilevered nature. 

In other (more positive) news: I managed to get my hands on a new product by Brian Schmalz called the "<a href="http://www.schmalzhaus.com/BigEasyDriver/index.htm">Big Easy Drive</a>r". Which is an upgrade to his existing "easy driver" (<a href="http://www.sparkfun.com/products/10267">available at sparkfun</a>). I'm hoping to swap out the Pololu 1201s for these new drivers tonight and give them a test run! 
