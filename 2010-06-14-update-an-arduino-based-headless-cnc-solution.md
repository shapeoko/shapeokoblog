---
layout: post
title: Update: An arduino based headless CNC solution
date: 2010-06-14 23:14
author: smadmin
comments: true
categories: [arduino, cnc, diy, electronics, grbl, headless cnc, seeedstudio, Shapeoko, sparkfun]
---
It's completely possible to run an Arduino based headless CNC machine! Here is the current setup I am using:

Hardware:
1.) <a href="http://www.seeedstudio.com/depot/sd-card-shield-for-arduino-v21-p-492.html">SD Shield from SeeedStudio</a> - as a side note: I hesitate to call this a "Shield" as it doesn't repeat the female headers on the top, so by using this you essentially lose access to your Arduino's V and GND ports. You need access to the GND port so you can tie the two GNDs from each Arduino together. I have circumvented this limitation by using two <a href="http://www.adafruit.com/index.php?main_page=product_info&amp;cPath=17_22&amp;products_id=65">mini bread boards</a>, as shown here: Also, it would be an easy enough fix to replace the current male headers with something like <a href="http://www.adafruit.com/index.php?main_page=product_info&amp;cPath=17_21&amp;products_id=85">these</a>, but I just have not gotten around to doing that.

It's not the most elegant solution, but it's working.... (as a side note: the USB cable in "master" is just to power the device, not communicate with it. I have since switched to a wall wart!)

Software:
Master Arduino: In my setup, I am calling the "master arduino" the one that parses the gcode. For this I am using a program called grbl. IMO, this is the holy grail of arduino based gcode parsing. you can download it <a href="http://github.com/simen/grbl">here</a>, or read a little about it <a href="http://grbl.tumblr.com/">here</a>. I actually found it via the<a href="http://www.contraptor.org/">contraptor project</a>, <a href="http://www.contraptor.org/motion-control">here</a>. You can see grbl in action <a href="http://dank.bengler.no/">here!</a>

Slave Arduino: The arduino that is connected to and reads the SD card. After pouring over a bunch of different fat libraries for arduino I settled on Bill.Greiman's <a href="http://code.google.com/p/fat16lib/">fat16lib</a>. It was very easy to implement and did exactly what I needed it to do.

I have had some problems overflowing the Master's buffer, but this is mainly due to the fact that I'm having a hard time setting up flow control. What I need to have happen is for the slave Arduino to Serial.print a line and then WAIT until it receives the "OK" from the master. I can't figure out how to do that reliably, so occasionally i overflow the master's buffer.....
