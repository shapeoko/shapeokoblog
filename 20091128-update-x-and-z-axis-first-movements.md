title: Update: X and Z axis first movements
link: http://www.shapeoko.com/archives/25
author: smadmin
description: 
post_id: 25
created: 2009/11/28 23:46:11
created_gmt: 2009/11/28 23:46:11
comment_status: open
post_name: update-x-and-z-axis-first-movements
status: publish
post_type: post

# Update: X and Z axis first movements

Just one short day after figuring out the Y-axis, the X and Z are both moving! I decided to stop by Radio Shack and pickup some DB9 connectors (1 male, 3 females) to make switching between motors easier. Although soldering all those pins on (24 total) wasn't much fun, it was totally worth it. In addition to making it easier switching between X,Y,andZ, the connectors also cleaned up a lot of the wiring. I also soldered headers onto the easy driver so I could actually mount it on the breadboard instead of just setting it there! Worked like a charm. As for the power supply, i switched from the ATX PS which was pushing 12v, to an old Dell Inspiron 20V 90W power supply. I'm not certain on this, but I'm pretty sure the extra power has really added to how smooth the motors run. I'm not even sure if that's possible, but it seems like it to me. Here are some video of the other two axis' running. The Z looks especially smooth, which i'll say is from the fact that the acme rod is short which pretty much eliminates the chance of it being bent (as I suspect is the case on the Y axis). The X axis is coming along but there seems to be some friction somewhere along the path which is causing it to hang up and stall the motor (even with the ramp up / ramp down code) I ordered two more Easy Drivers from Sparkfun yesterday, they should be here early next week. At which time I'll try hacking together something that runs all 3 axis in an indefinite "test" pattern. Pretty exciting stuff here!