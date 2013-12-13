---
layout: post
title: All-in-one CNC Controller (Azteeg G1)
date: 2012-06-26 09:23
author: smadmin
comments: true
categories: [electronics, Shapeoko]
---
<h2>A quick history:</h2>
A little over 2 years ago, I posted <a href="http://forum.sparkfun.com/viewtopic.php?f=14&amp;t=20170" target="_blank">this</a> to the sprakfun forum. In summary it is a schematic for an 'all-in-one' cnc controller that I wanted to call grblDuino. The core of the design was based off the arduino chip (atmega 168 at the time) and 3 easy drivers (atmel A3977). I tried my hand at eagle but in the end didn't make the appropriate effort or time to learn enough about basic board design to get past a simple (and probably flawed) layout/schematic.

<a href="http://www.shapeoko.com/wp-content/uploads/2012/06/grblDuino.jpg"><img class="alignnone size-medium wp-image-807" title="grblDuino" src="http://www.shapeoko.com/wp-content/uploads/2012/06/grblDuino-300x212.jpg" alt="" width="300" height="212" /></a>

&nbsp;

After several months of not doing anything with the grblDuino, I met and became friends with some people who were capable of making such a board. The problem was they didn't have an interest in it. In fact, nobody that I talked to had an interest in making the board. Their argument was that it wouldn't be cost effective. After all it's tought to compete with Arduino, considering their quantities.

The issue I had was that I wasn't trying to compete with Arduino. I wasn't trying to make anything arduino compatible. The only similarity was the chip (at the time the atmega 168). But, nobody was down with building something that wasn't directly arduino compatible. Oh well, as it were, I was happy with the <a href="http://www.sparkfun.com/products/10267" target="_blank">easy drivers</a>, then I was happy with the <a href="http://www.pololu.com/catalog/product/1182" target="_blank">pololus</a>, then I was happy with the <a href="http://www.buildlog.net/blog/2011/08/stepper-driver-arduino-shield/" target="_blank">stepper shield</a> from buildlog, then I was happy with the <a href="http://www.synthetos.com/wiki/index.php?title=Projects:grblShield" target="_blank">grblshield</a> from sythetos.
<h2>Fast forward to present day:</h2>
Last month I went to Makerfaire in the Bar Area. One of the people that I met was Roy of <a href="http://www.panucatt.com/" target="_blank">Panucatt</a> Fame. You know, the ones who make the Azteeg <a href="http://www.panucatt.com/azteeg_X1_reprap_3d_printer_controller_p/ax13dp.htm" target="_blank">X1</a> 3D printer controller. Roy and I talked about project Shapeoko and he asked if there was anything the project needed, in terms of electornics. My immediate though was back to the grblDuino! Yes, there are lots of solutions currently available to drive your machine, all stated above, and they all work great. But, it's always seemed more complicated than it needs to be. And expensive. Without building your own solution, you'll need:
An Arduino - $30 +
a.) Buildlog shield: $25 for board + $36 for pololu chips = $61 + Arduino = $91
b.) grblshield: $60 for board (build in drivers) + Arduino = $90

For a project that's striving to hit the <strong><span style="text-decoration: underline;">$300</span></strong> mark, every dollar counts! At ~$90, nearly 1/3 of the goal cost for the entire machine is being consumed by the controller. I'm not saying those controllers aren't worth it, they're great, and they've never let me down, but again it seemed like the cost could be shaved considerably by eliminating the unecessary bits and pieces that weren't being used.

<strong>Enter the Azteeg G1 - all in one CNC controller.</strong>

<a href="http://www.shapeoko.com/wp-content/uploads/2012/06/azteeg_g1.jpg"><img class="size-medium wp-image-808" title="azteeg_g1" src="http://www.shapeoko.com/wp-content/uploads/2012/06/azteeg_g1-300x201.jpg" alt="" width="300" height="201" /></a>

Right now panucatt is anticipating a price point between $70-$80USD. As I'm told, general availability could be as early as the end of July!

Some tech specs:

- ATmega 328P
- FT231x USB chip (FT232RL on prototype)
- 2oz PCB RoHS compliant
- 3 DRV8811 Stepper drivers
- 12-30V wide input switching power supply(single supply)
- PTC protected USB line
- Fast Acting 5A Blade Fuse
- RX/TX Leds

&nbsp;
<h2>Here's my review of the unit they sent me for testing.</h2>
<strong>First impressions:</strong> This thing looks awesome! It's the same color blue as the Azteeg X1. The silkscreen is white (and super informative) and the markings are in a very cool silver color. Not sure where the idea came from, but they also put a piece of thick (maybe .22") clear acrylic over the top of the controller. I want to take it off and engrave the Shapeoko logo on it! The acrylic is held in by 3 screws going into standoffs. The standoffs themselves are an added bonus. I can see mounting this thing directly to the back of the machine. (with an additional shroud for protection of flying debris and to prevent possible shorting issues)
<h3>

<a href="http://www.shapeoko.com/wp-content/uploads/2012/06/azteeg_g1_top_left.jpg"><img class="size-medium wp-image-809" title="azteeg_g1_top_left" src="http://www.shapeoko.com/wp-content/uploads/2012/06/azteeg_g1_top_left-300x201.jpg" alt="" width="300" height="201" /></a>

Testing:</h3>
Right now there are only about 2 hours of machine time on this controller (time the controller was actually driving the machine). But, from my testing (mostly <a href="http://www.shapeoko.com/wiki/index.php/Tsp_sld" target="_blank">single line drawings</a>) it's been as advertised. It runs exactly the same as an arduino + grblshield. As it should, using the same stepper driver chips (TI DRV8811) and firmware.

<strong>Testing Overview: </strong>The machine I used for testing has a dual drive Gantry. The Azteeg G1 only supports 3 axis. To prevent disassembling the machine, I plugged both my gantry drives into the Y axis control (taking care to reverse the pairs on one of the drives). No problems there. When they sent me the board, it was pre-loaded with the stable version of grbl (v0.7). Instead of loading the edge branch (v0.8d), i ran with the stable version. I'm planning to load v0.8 soon and run some more testing. A couple of features I'd like to test are the limit switches in action and the spindle control. Panucatt placed 2 Mosfets on the board which can be used to drive an external relay (in the same fashion the buildlog <a href="http://www.buildlog.net/blog/2011/10/pololu-compatible-relay-driver/" target="_blank">4th axis relay driver</a> works). Some people might disagree, but I like the fact that they left the relay off the board. This saved some cost, yet still left the option available without too much added work.

[caption id="attachment_810" align="alignnone" width="300" caption="Azteeg G1 - Front/Top View"]<a href="http://www.shapeoko.com/wp-content/uploads/2012/06/azteeg_g1_front_top.jpg"><img class="size-medium wp-image-810" title="Azteeg G1 - Front/Top View" src="http://www.shapeoko.com/wp-content/uploads/2012/06/azteeg_g1_front_top-300x201.jpg" alt="" width="300" height="201" /></a>[/caption]

<strong>Usability Notes:</strong> As with the grblShield, heat dissipation seams to be great. The drivers were set to 1A, and I was running my machine at about 16,000mm / minute. I didn't measure the temp, but there were no overheating issues as seen when using the pololu drivers without heatsinks + active cooling. I'm told with the production version of the Azteeg G1, 2oz copper will be used, adding even more disappation potential to the layout.
- Setting the microsteps individually per axis was a huge plus. They're manipulated the same way the buildlog shield is done (with jumpers).
- Screw down terminals made connecting my machine a breeze. They seem slightly smaller than what's used on the buildlog shields, but didn't seem to effect inserting the wire and screwing it down.
- There's a jumper on the board allowing you to power it from USB only. This can be used for programming the board. Switch the jumper back and it uses the 24v supply. Both are clearly marked on the silkscreen.
- I inadvertantly plugged in the controller to the 24v source *before* attaching my stepper motors. As some of you may have learned the hard way (myself included), with a pololu setup this would have *blown* all the chips, releasing their magic black smoke and becoming $12 paper-weights (<em>for very small pieces of paper</em>). With the Azteeg G1, it didn't matter. After realizing what I did, I simply unplugged the 24v source, then connected my motors, then plugged it back in, and it worked fine. No issues. This is more of a testimate to the TI DRV8811 chips than the board itself, but it's definitly worth noting.

&nbsp;

[caption id="attachment_811" align="alignnone" width="300" caption="Azteeg G1 - bottom view"]<a href="http://www.shapeoko.com/wp-content/uploads/2012/06/azteeg_g1_bottom.jpg"><img class="size-medium wp-image-811" title="azteeg_g1_bottom" src="http://www.shapeoko.com/wp-content/uploads/2012/06/azteeg_g1_bottom-300x201.jpg" alt="" width="300" height="201" /></a>[/caption]

[caption id="attachment_812" align="alignnone" width="300" caption="Azteeg G1 - Top Right View"]<a href="http://www.shapeoko.com/wp-content/uploads/2012/06/azteeg_g1_front_right.jpg"><img class="size-medium wp-image-812" title="azteeg_g1_front_right" src="http://www.shapeoko.com/wp-content/uploads/2012/06/azteeg_g1_front_right-300x201.jpg" alt="" width="300" height="201" /></a>[/caption]

[caption id="attachment_813" align="alignnone" width="300" caption="Azteeg G1 - Front Left View"]<a href="http://www.shapeoko.com/wp-content/uploads/2012/06/azteeg_g1_front_left.jpg"><img class="size-medium wp-image-813" title="azteeg_g1_front_left" src="http://www.shapeoko.com/wp-content/uploads/2012/06/azteeg_g1_front_left-300x201.jpg" alt="" width="300" height="201" /></a>[/caption]
<h2>Conclusion</h2>
I can't really find anything to complain about. There was a minor mistake on the silkscreen, but even with that, this is the best 'prototype' board I've ever seen. Had I not known first hand it was a prototype, I would have guessed it to be a finished product. If Panucatt can really deliver this board for the pricepoint they're estimating, I think it'll be a winner. It's clean, simple, and does what it's supposed to do. I'll post a follow up review after the edge version of grbl is installed and has been tested.
