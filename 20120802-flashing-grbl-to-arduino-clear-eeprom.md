title: Flashing grbl to Arduino, clear EEPROM
link: http://www.shapeoko.com/archives/863
author: smadmin
description: 
post_id: 863
created: 2012/08/02 07:44:11
created_gmt: 2012/08/02 13:44:11
comment_status: open
post_name: flashing-grbl-to-arduino-clear-eeprom
status: publish
post_type: post

# Flashing grbl to Arduino, clear EEPROM

On a few occasions over the last several months I've wanted to flash a *fresh* install of grbl to an Arduino. As you may know, the problem with this is the persistent [EEPROM](http://en.wikipedia.org/wiki/EEPROM) settings that define your Shapeoko's setup. Here's the situation: To save you the hassle of having to re-input your grbl settings each time you do an upgrade, grbl instead stores your settings in eeprom. That's a really great feature, and a real time saver until you don't want those settings anymore! Then it turned into an exercise in frustration as each time I loaded a new version of grbl (v0.8) my setting remained the same, because they were stored in EEPROM. What's the solution? Well, for me it was easiest to just clear the EEPROM with a small script, and *then* flash the new grbl. The script is from the arduino site ([link](http://arduino.cc/en/Tutorial/EEPROMClear)): \-------------------------------- 

> ` /* * EEPROM Clear * * Sets all of the bytes of the EEPROM to 0. * This example code is in the public domain.` `*/ #include void setup() { // write a 0 to all 512 bytes of the EEPROM for (int i = 0; i < 512; i++) EEPROM.write(i, 0); // turn the LED on when we're done digitalWrite(13, HIGH); } ` `void loop() { } `

\--------------------------------  

>

## Comments

**[nick castrovinci](#190 "2013-09-04 04:02:17"):** How do i program the arduino to the GrblShield v4

