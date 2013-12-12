title: Update: An arduino based headless CNC solution
link: http://www.shapeoko.com/archives/84
author: smadmin
description: 
post_id: 84
created: 2010/06/14 23:14:56
created_gmt: 2010/06/14 23:14:56
comment_status: open
post_name: update-an-arduino-based-headless-cnc-solution
status: publish
post_type: post

# Update: An arduino based headless CNC solution

It's completely possible to run an Arduino based headless CNC machine! Here is the current setup I am using: Hardware: 1.) [SD Shield from SeeedStudio](http://www.seeedstudio.com/depot/sd-card-shield-for-arduino-v21-p-492.html) \- as a side note: I hesitate to call this a "Shield" as it doesn't repeat the female headers on the top, so by using this you essentially lose access to your Arduino's V and GND ports. You need access to the GND port so you can tie the two GNDs from each Arduino together. I have circumvented this limitation by using two [mini bread boards](http://www.adafruit.com/index.php?main_page=product_info&cPath=17_22&products_id=65), as shown here: Also, it would be an easy enough fix to replace the current male headers with something like [these](http://www.adafruit.com/index.php?main_page=product_info&cPath=17_21&products_id=85), but I just have not gotten around to doing that. It's not the most elegant solution, but it's working.... (as a side note: the USB cable in "master" is just to power the device, not communicate with it. I have since switched to a wall wart!) Software: Master Arduino: In my setup, I am calling the "master arduino" the one that parses the gcode. For this I am using a program called grbl. IMO, this is the holy grail of arduino based gcode parsing. you can download it [here](http://github.com/simen/grbl), or read a little about it [here](http://grbl.tumblr.com/). I actually found it via the[contraptor project](http://www.contraptor.org/), [here](http://www.contraptor.org/motion-control). You can see grbl in action [here!](http://dank.bengler.no/) Slave Arduino: The arduino that is connected to and reads the SD card. After pouring over a bunch of different fat libraries for arduino I settled on Bill.Greiman's [fat16lib](http://code.google.com/p/fat16lib/). It was very easy to implement and did exactly what I needed it to do. I have had some problems overflowing the Master's buffer, but this is mainly due to the fact that I'm having a hard time setting up flow control. What I need to have happen is for the slave Arduino to Serial.print a line and then WAIT until it receives the "OK" from the master. I can't figure out how to do that reliably, so occasionally i overflow the master's buffer.....

## Comments

**[Ryan](#53 "2011-10-07 17:28:37"):** Thanks for this great artical! Can you please show the schematics or explain what way you connected everything together. thanx!

