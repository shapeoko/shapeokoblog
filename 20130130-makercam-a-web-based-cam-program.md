title: MakerCAM - a web based CAM program
link: http://www.shapeoko.com/archives/969
author: smadmin
description: 
post_id: 969
created: 2013/01/30 22:52:02
created_gmt: 2013/01/31 04:52:02
comment_status: open
post_name: makercam-a-web-based-cam-program
status: publish
post_type: post

# MakerCAM - a web based CAM program

I have a little story to tell you. Years ago, maybe 7-8 at this point, I finished building my very first CNC machine. It was not named Shapeoko, you could not build it for anywhere near $300, and it was not assemble-able by nearly everyone. It was in fact, the exact opposite of Shapeoko. But, neadless to say, I finished assembling the machine, and wired all of the electronics. After that I installed EMC2 (now [linuxCNC](http://linuxcnc.org/)). I tuned the motors and ran the test job. Success! I was in business. Right away, I wanted to cut my own part. I had already drawn it to scale in CAD and saved the file. Problem was... I kept trying to open it with EMC2 and for the life of me, I couldn't get it to open. Ends up, there's a step between the CAD part and the cutting part. It's called CAM.  I didn't know that. So off to the internet I went, scouring any sort of information I could on this so called "CAM". I'll give you a run-down on the jist of CAM:  CAM is the process where you (or the software) define your toolpaths. The toolpaths are what turn into g-code. And the g-code is the language your machine understands. The overall workflow goes like this: **Draw Something -> CAM Something -> Stream Something -> Cut Something** Pretty easy right? It actually is surprisingly easy once you find a program for each of those steps that you are comfortable with. The problem for most beginners is they don't really know what software to use for steps 1 and 2. **Here are my suggestions:** _DRAW SOMETHING_: Start with [inkscape](http://inkscape.org/) for your CAD program. it's free, there are plenty of tutorials, and it's pretty easy to use once you get the hang of it. Yes, you are not going to design the space shuttle with inkskape, but it's a no-risk way of getting started drawing. _CAM SOMETHING_: I've looked high and low for a nice open source, entry level CAM program. As luck would have it, after YEARS of searching, I found one mentioned in another forum, and tracked it down to find out it had been abandoned but the source was released before said abandonment. It was created by a guy named Jack, and I'm planning to do an entire other blog post explaining how this came to be. For now, just know that Jack's creation (which he called PartKam), is now available on my [github page](https://github.com/shapeoko/makercam), and is being hosted at one of my other domains. You can find it here: [www.makercam.com](http://www.makercam.com). You will find a basic 'help' and 'tutorial' link at the top of the page. However, they say that a picture is worth a thousand words, so we'll assume that a video is worth a million. So, instead of rambling on more about this, here are two videos representing steps 1 and 2 of the process.     Please feel free to join in on the [forum discussion](http://shapeoko.com/forum/viewtopic.php?f=6&t=1200) regarding makercam, and if you're interested in helping improve the code base, drop me a line. There you have it. Enjoy!

## Comments

**[Craig Hollabaugh](#145 "2013-02-08 03:01:35"):** Edward, I just opened my first shapeoko box this evening. Its now 2AM and I'm so excited. I just watched these 2 videos and am ready for the third. I hope you use linuxcnc for the controller. I plan on using this shapeoko for making stuff with my 5 year-old granddaughter. We spend Saturdays together and always have a project. These two videos are a perfect introduction for that. My second shapeoko will be a SMT pick and place machine for work. Your kit is awesome. Part machining quality is high and beefy. Build documentation is excellent. If I could stay awake, I'd had this put together before sunrise. Thanks sooo much. Will keep you posted on our projects over here. Craig

**[selektha](#171 "2013-07-02 09:02:00"):** Hi, Any news when the third part will arive? =) I think these videos is great for the first timers and would love to see more of them.

