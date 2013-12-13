---
layout: post
title: Update: Arduino based headless CNC machine. Now featuring hardware flow control!
date: 2010-06-17 23:17
author: smadmin
comments: true
categories: [arduino, cnc, diy, electronics, grbl, headless cnc, Shapeoko]
---
In my last post I mentioned having a problem over flowing the tiny arduino serial buffer while streaming gcode from one unit to another. Since then, I have talked to a few people about the matter, and <a href="http://forums.adafruit.com/viewtopic.php?f=25&amp;t=13715" target="_blank">one suggested</a> implementing some sort of hardware flow-control .

<span style="font-size: x-small;"><span style="font-size: xx-small;">"What it seems to me like you might need is some physical hardware flow control, just a wire running between the master and slave independent of the serial line. So maybe the slave would send some data, and wait for a change on the line, whereas the master would wait to receive data, process it, change the line status, rinse, repeat."</span></span>

How the implementation ended up going down was something like this:

1.) Connect wire between arduinos (Slave: Pin7 to Master: Pin13)
2.) Master: after each byte recieved, check the status of the buffer. By issuing the serialAvailable() command returns the number of bytes available to be read from the buffer. We know the buffer is only 128bytes in size, so we can do a simple if statement:
if(serialAvailable()&gt;= 128) {LEDPORT |= _BV(LEDBIT);}   //turn on LED13

3.) Slave: before sending byte, check the status of pin7
while ((c = file.read()) &gt; 0)
{
while(val = digitalRead(flowpin) == HIGH)
{
delay(100);
}
Serial.print((char)c);
}
Here is a video of the setup in action. Keep in mind that the SD "shield" is not a shield, i.e. the pins are not repeated on the top of the shield. So, in order to get this to work, i had to use the mini-bread-boards and because of that, this looks a lot more complicated than what it is.

Also, on a somewhat related note: <a href="http://blog.makezine.com/archive/2010/06/grbl_an_arduino-based_g-code_interp.html" target="_blank">grbl made it on MAKE!</a>
