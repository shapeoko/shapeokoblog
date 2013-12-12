title: Update: From zero to hero. And back again.
link: http://www.shapeoko.com/archives/60
author: smadmin
description: 
post_id: 60
created: 2010/02/18 20:00:39
created_gmt: 2010/02/18 20:00:39
comment_status: open
post_name: update-from-zero-to-hero-and-back-again
status: publish
post_type: post

# Update: From zero to hero. And back again.

After frying my old Arduino Duemilanove I knew that I'd need to get a new one, and fast. Sparkfun to the rescue. I sat down, ordered a new one (the standard chip is now an atmega328!), ordered some jumper wires and a new breadboard while I was at it. The three tiny breadboards were ordered before I fried my easyDrivers. FYI: they are the perfect size to hold and tie in to a single EasyDriver (v4.2) with headers soldered on! I also took the liberty of ordering an atmega328 chip with Arduino bootloader. Because of the semi low cost (~$5), i figured it was worth trying to revive my old arduino. First thing I did when the new gear came was pop the old chip out of the fried arduino and popped in the chip in. Yahtzee! My old Arduino is not only alive, it's also upgraded to a better chip. Needless to say, that was good news. While I decide what path to take for the rest of this project I also ordered more easy drivers. Although there's a good chance I will be using a different solution by the time I complete this project, but I feel comfortable with the easy drivers and know they will work for the time being. Also, I have been thinking very much about cutting the PC out of the loop entirely. As is, the PC (currently my Dell Mini 9) is simply streaming a gcode file to the arduino. From there, grbl does the rest. Seems like overkill to use a PC for such a simple task.....Enter a second arduino. The second Arduino will have some FAT library loaded as firmware (have yet to decide which one) and be connected to an SD card shield! The arduino will then read one line of gcode at a time, send it to the primary arduino and wait for the "OK" before sending the next line. Also, I ran across this instructable, which gave me a pretty rad idea: Why not use one of my old N64 controllers to control the mill? I'm thinking about going to a two Arduino setup as is, with one Arduino not doing much work there should be plenty of ports and programming space available to implement a program which will allow me to jog the machine around, along with possibly homing the Z axis. In fact, although the feature has a certain amount of "coolness", its quite practical. After all, one does need a way to gracefully move the machine to a "home" position. Right?