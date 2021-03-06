---
layout: post
title: Things you figure out along the way
date: 2012-02-19 00:42
author: smadmin
comments: true
categories: [design, electronics, Milling, Shapeoko, Software]
---
I just posted up a new video on youtube showing my shapeoko cutting a new set of dremel mounts out of UHMW.

<iframe width="640" height="480" src="http://www.youtube.com/embed/Udd4t5G4mxQ" frameborder="0" allowfullscreen></iframe>

Within an hour of posting, I've had two emails and a youtube comment asking about certain parts of the setup. I figured this was a good opportunity to post about some things I've found out along the way. And why my setup looks the way it does.

We'll take @bxd's youtube comment because he basically summarized the rest of the emails:
<blockquote><em>CNC on a Budget spindle, and mach3?﻿ Do the plexi debris guards help? (or inversely, does the lack of a guard cause the belts and pulleys to get gummed up?)</em></blockquote>
<strong>CNC on a budget Spindle</strong>

That's still on my rig for two reasons: 1.) It's quieter than a standard dremel. I do most of my cutting after 9pm, so noise is a big deal to me. It's not ninja quiet by any means, but it's a little quieter than the dremel. More specifically, it's not as high pitched. I think dB wise, it's only a couple less than the dremel (I"ll do another reading and post those results), but the pitch of the noise is different, and (maybe this is all in my head) I don't think that it travels as far *outside* of my garage as the dremel does. 2.) I mounted the thing up a while back (several months ago) and just haven't really wanted to take it off. Not because it's super awesome, but just because I didn't want to spend the time doing it. Seems like whenever I have time, I spend it cutting parts for the orders, so besides knowing the setup works as is, I don't want to take away from my "production" time.

Ironically, the video I posted on youtube shows the machine cutting a new mount for my dremel. The CNC on a budget spindle has stalled out on me a few times in the last week and nearly stalled a couple other times. All of which resulted in me scrapping my parts. So, I thought I'd give the dremel a shot and see how it does. Plus, the dremel mount brings the bit about 3/4" closer to the z-axis rail. Which should make the setup even more rigid.

<strong>Mach 3?</strong>

It's actually EMC2. But I think maybe @bxd was trying to say "hey, that's *not* grbl! At least that's how I took it :-)

I love grbl. I was one of the first people to start using it after Simen released the initial version. It was my introduction to gcode interpretation and where that fit into the CNC stack. Prior to using grbl I had several failed attempts at both EMC2 and Mach3. But grbl just worked (after I figured out how to compile and flash it to my arduino). And I liked that about it. Hell, I still like that about it actually.

But I don't always use grbl. I mostly use EMC2 when I'm doing batch runs of parts. Because of it's visualization and speed control, I can adjust on the fly for stock sizes that varies from one to the next, and I can adjust the speed on the fly if I've programmed the job too fast. That's pretty handy. There are a lot of handy things about EMC2. There are also lots of handy things about grbl.

I think of grbl like a single speed (not a fixie) bike (if anyone else here is a biker?). With a single speed bike, you don't have to worry about shifting gears, or de-railers breaking, or any of the other stuff, that turns into a distraction, all you have to do is pedal. And that's what it's like with grbl, you don't have to have visualization, or speed control, or anything else. You just pipe it gcode and it diligently interprets it.

<strong>PlexiGlass Sides:</strong>

That's something I learned along the way! It wasn't until I started cutting UHMW that I ran into a problem with material buildup on the rails. The dust from UHMW is really light and it tends to stick to everything that's metal. Spindle, makerslide, bolts, mount plates, screwdriver sitting next to the machine, zipper on your fleece, EVERYTHING!

So, last week I put those shields on. Prior to that I just had a piece of cardboard leaning against both Y axis rails. And prior to that I had nothing.

The makerslide v-wheels have a little lip on the inside of them that acts as a simple "debris clearer" if something gets in there, it'll hit that lip and get pushed out to the side. But, because the UHMW sticks to the rails, it never catches that lip. Instead it just slowly builds up in the middle of the vwheel until eventually your machine will stall.

In everyday life this isn't an issue. You can run a full job and not worry about buildup, in fact you can run several jobs without worrying about it. And I think most of us would clean our machines after each job. Or at least once a night. Nothing fancy, just reverse the hose on your shopvac and blow everything off, then sweep up the floor when you're all finished. But because I want my machine to run for several hours unattended, where all i'm doing is replacing the material after each set, I ended up putting those guards on.

Those are sort of fancy to! I had a friend cut and bend them for me. They're made from regular plexi that was heated up with a torch, then bent over the edge of a workbench. The material cost me about $8 plus the 4 insertion nuts, M5 washers, and M5 x 12mm bolts I used to mount them.

The belt getting gummed up was never an issue though. After I designed it and built the prototype, I wondered if an upside down belt was going to be a problem. So far so good, if material does stay on the belt (which it tends not to for some reason, maybe vibration?) it ends up falling out by the time it makes it over the smooth idler.

I think the main thing to remember is: If you clean your machine after you use it, then you probably won't need the shields. I personally think they look pretty cool though :-) Would be even cooler to edge light them.
