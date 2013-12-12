title: Update: Mill - overall progress
link: http://www.shapeoko.com/archives/40
author: smadmin
description: 
post_id: 40
created: 2009/12/01 13:47:21
created_gmt: 2009/12/01 13:47:21
comment_status: open
post_name: update-mill-overall-progress
status: publish
post_type: post

# Update: Mill - overall progress

There's something wrong with the X axis. Unlike the Y, it's very difficult to move. Well, not very difficult but more difficult than the Y. I think there may be a bit of a design flaw... stupid designer. From what I can tell, there is some friction between the X-axis-rail-mount-plates (the ones slotted end to end) and the X-axis-cross-plate (the one that the X-axis acme nut mounts to). I'll try taking some sandpaper to it and if that doesn't work, perhaps the dremel? Someone also suggested I use wax.. i don't even know where I'd find wax though. Also, I should have boxed in the X-axis cross plates because there is flex when the nut is being driven. I'm going to move forward and continue with the current iteration. After the new power supply is delivered and the EasyDrivers are installed, I'll see where we're at. But, I'm afraid I'll have to make some changes to the design and re-order all of the parts from ponoko. It's not the end of the world but I hate the fact that I didn't get it perfect the first time... Though, I should be used to that by now. On a different note: When I started this project I was certain that a computer would be running the machine. However, I've been using the arduino to test the motors and when I get the 2 additional EasyDrivers I'm planning to run them through their paces with the arduino as well. I keep thinking how awesome it would be to use the arduino permanently as the controller. Yes, replace a full PC with a tiny arduino! My machine has a very small footprint to begin with, and I keep thinking how cool it would be house *all* of the controls in a tiny matching box! I don't even know if that's possible, but wouldn't it be sweet! I'm imagining something like this: Obviously, do the CAD/CAM on a workstation but save the G-code to an SD card. Then, insert the SD card into the arduino, turn the arduino on, it would then look for a specific text file. Parse the file and run the machine! I know it's a lot harder than that and I'm doubting there would be enough room on the arduino to store the code to both control the reading of the SD card and parse the file and run the machine.  Either way, a guy can dream right?