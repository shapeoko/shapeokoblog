title: Update: Turns out, it's not so bad after all.
link: http://www.shapeoko.com/archives/67
author: smadmin
description: 
post_id: 67
created: 2010/02/19 22:00:20
created_gmt: 2010/02/19 22:00:20
comment_status: open
post_name: update-turns-out-its-not-so-bad-after-all
status: publish
post_type: post

# Update: Turns out, it's not so bad after all.

As mentioned yesterday, driving the mill with an N64 controller seems like an awesome idea. Today, I set to work trying to figure that out. I was almost immediately sidetracked

As luck would have it, my stash of NES controllers (qty: 2) were in the same location as my stash or N64 controllers! I couldn't resist.  Shapeoko needs a "joystick". All CNC machines have one. They are either software controlled (buttons on screen) or hardware.  They are necessary to move the gantry out of the way and to "home" your machine to the material. I have an old [joystick](http://www.happcontrols.com/) from an [arcade](http://www.edslifedaily.com/arcade.html) I build a few years ago that I have been planning to use. However, one of the problems using a traditional joystick is that it takes up one port for each direction you are trying to capture. So in our case we would want: Forward, Back (Xaxis), Left, Right (Yaxis), Up, Down (Zaxis). That's 6 inputs we would need! The NES controller doesn't need one output for each button because it's digital. What's that mean? Good question. Here is how I understand the NES controller to work: The chip inside the controller is polling the status of the buttons at a rapid rate. When the buttons are not being pressed, the result of the poll looks like "11111111" (one bit for each button). After the controller is done polling, it sends that string to the console (in our case the Arduino) which is then interpretted by the program into whatever the button are mapped for. When you press a button on the controller the string changes to reflect it. For instance if you press the select button the string changes to 11011111. The cool part about this is the arduino need only use 3 ports to interface with all 8 buttons! The three ports are for "Clock", "Latch", and of course data. The data wire is where all the action is! Clock and latch are there to keep the timing correct. To be honest I don't completely understand how it works, but I figured it out enough to capture the inputs with the Arduino and light up the corresponding LEDs! I would like to say, as a side note, working with a "digital" also prevents you from having to debounce the button pushes. Because that debounce logic is already in the chip that's doing a2d inside the controller! we're just taking the "clean" data :) Here's a quick video of the setup in action. The code is below if you want it. 

Now that the buttons are mapped and I feel pretty confident about capturing button presses, I am going to get to work on writing the code to control the step/dir functions of the easy drivers.