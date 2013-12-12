title: Update: Where were we?
link: http://www.shapeoko.com/archives/76
author: smadmin
description: 
post_id: 76
created: 2010/04/01 15:38:37
created_gmt: 2010/04/01 15:38:37
comment_status: open
post_name: update-where-were-we
status: publish
post_type: post

# Update: Where were we?

.... Oh yes, building a mini CNC machine! **A couple of things happened shortly after the NES success of late February:**

  1. Burnt up another EZ Driver
  2. Burnt up ANOTHER 2 EZ drivers!
  3. Got completely side tracked on trying to design a circuit to hold an Allegro A4983 chip
  4. Was completely side tracked trying to stream gcode from one Arduino to another
  5. Took a break.
**Scope, focus, project goals** As I mentioned in a [previous post](http://www.edslifedaily.com/1/post/2009/11/update-mill.html) there are certain times during a project when you need to step back, regroup, and find your focus. This past month was one of those times for me. After taking a 20,000ft view of the project I decided that in order get past the current hump, I need to straighten out my electronics setup, and just quit messing with it. It seems that because I’m so intrigued by the electronics portion of the project (it’s the newest and most interesting part of the process for me), that I have had a hard time just letting it be, so that’s what I’m going to focus on: Getting the electronics assembled, configured, and hooked up. THEN LEAVING THEM ALONE! **Electronics** For now I have abandoned the [EasyDrivers](http://www.sparkfun.com/commerce/product_info.php?products_id=9402) in search of something that can give my motors a little more oomph. While trying to design a circuit around the Allegro A4983, I ran across [this product](http://www.pololu.com/catalog/product/1201) by Pololu. Which had essentially done what I was trying to do, however thier version is much neater than I could have done. After Ordering 3 boards, and testing them out on the breadboard, I’ve set about making a more permanent solution to mount them in. [PIC] At this point, the goal is to finish implementing/troubleshooting/debugging the electronics by the end of the weekend. This should free me up to move on to more important things….. **Software** If the electronics are setup, and I’m OK leaving my design the way it is (for testing purposes) then I need only focus on implementing the software. Luckily, it looks like [Simen has really kicked ass in the software department](http://labs.bengler.no/-/bulletin/show/556650_micro-w-grbl-first-cuts?ref=mst). All I need to do at this point is get the newest version of GRBL flashed to my Arduino and maybe do some fine tuning on the stepper settings (rapid and default federates). Then: TEST! That’s it for now. Here are some pictures of a couple setups and some new bits...