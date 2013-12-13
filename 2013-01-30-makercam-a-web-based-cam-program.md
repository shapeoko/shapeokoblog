---
layout: post
title: MakerCAM - a web based CAM program
date: 2013-01-30 22:52
author: smadmin
comments: true
categories: [design, Shapeoko, Software]
---
I have a little story to tell you.

Years ago, maybe 7-8 at this point, I finished building my very first CNC machine. It was not named Shapeoko, you could not build it for anywhere near $300, and it was not assemble-able by nearly everyone. It was in fact, the exact opposite of Shapeoko. But, neadless to say, I finished assembling the machine, and wired all of the electronics. After that I installed EMC2 (now <a href="http://linuxcnc.org/" target="_blank">linuxCNC</a>). I tuned the motors and ran the test job. Success! I was in business.
Right away, I wanted to cut my own part. I had already drawn it to scale in CAD and saved the file. Problem was... I kept trying to open it with EMC2 and for the life of me, I couldn't get it to open. Ends up, there's a step between the CAD part and the cutting part. It's called CAM.  I didn't know that. So off to the internet I went, scouring any sort of information I could on this so called "CAM".

I'll give you a run-down on the jist of CAM:  CAM is the process where you (or the software) define your toolpaths. The toolpaths are what turn into g-code. And the g-code is the language your machine understands. The overall workflow goes like this:

<strong>Draw Something -&gt; CAM Something -&gt; Stream Something -&gt; Cut Something</strong>

Pretty easy right? It actually is surprisingly easy once you find a program for each of those steps that you are comfortable with. The problem for most beginners is they don't really know what software to use for steps 1 and 2.

<strong>Here are my suggestions:</strong>

<em>DRAW SOMETHING</em>: Start with <a href="http://inkscape.org/" target="_blank">inkscape</a> for your CAD program. it's free, there are plenty of tutorials, and it's pretty easy to use once you get the hang of it. Yes, you are not going to design the space shuttle with inkskape, but it's a no-risk way of getting started drawing.

<em>CAM SOMETHING</em>: I've looked high and low for a nice open source, entry level CAM program. As luck would have it, after YEARS of searching, I found one mentioned in another forum, and tracked it down to find out it had been abandoned but the source was released before said abandonment. It was created by a guy named Jack, and I'm planning to do an entire other blog post explaining how this came to be. For now, just know that Jack's creation (which he called PartKam), is now available on my <a href="https://github.com/shapeoko/makercam" target="_blank">github page</a>, and is being hosted at one of my other domains. You can find it here: <a href="http://www.makercam.com" target="_blank">www.makercam.com</a>. You will find a basic 'help' and 'tutorial' link at the top of the page.

However, they say that a picture is worth a thousand words, so we'll assume that a video is worth a million. So, instead of rambling on more about this, here are two videos representing steps 1 and 2 of the process.

&nbsp;
<iframe width="640" height="480" src="http://www.youtube.com/embed/Ow4L6SozIK8" frameborder="0" allowfullscreen></iframe>
&nbsp;
<iframe width="640" height="480" src="http://www.youtube.com/embed/tVFMIFQviPw" frameborder="0" allowfullscreen></iframe>

Please feel free to join in on the <a href="http://shapeoko.com/forum/viewtopic.php?f=6&t=1200">forum discussion</a> regarding makercam, and if you're interested in helping improve the code base, drop me a line.
There you have it.  Enjoy!
