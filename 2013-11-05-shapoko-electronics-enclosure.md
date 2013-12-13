---
layout: post
title: ShapeOko Electronics Enclosure
date: 2013-11-05 16:46
author: mathewowen
comments: true
categories: [design, electronics, Electronics, Enclosure, Laser Cut, Laser Cutting, shapeoko, Shapeoko]
---
<h3 style="text-align: left;"><em>The following post is from guest blogger Matthew Owen. Matthew is a member of the Shapeoko community, a maker, founder of <a href="http://lasercuttinglab.com/shop/">Laser Cutting Lab, LLC</a>, and an all around cool guy. </em></h3>
<hr>
&nbsp;
<h3 style="text-align: left;">ShapeOko Enclosure by <a title="Laser Cutting Lab, LLC" href="http://lasercuttinglab.com" target="_blank">Laser Cutting Lab, LLC</a></h3>
<p style="text-align: left;">I decided to build an electronics enclosure for my ShapeOko and recently acquired ShapeOko 2 (pre-order). The suggested curved acrylic plate was nice but not entirely practical. Besides, I enjoyed designing and building this enclosure so for anyone interested, here it is.</p>

<h3> The List of Components:</h3>
- 1/4" birch plywood - 24" x 12" - 3 pieces ($10 hardware store)
- 24v 5a power supply (eBay $15 incl. shipping)
- 24v 1.4w Papst Fan ($10 eBay)
- Power switch ($3.19 at Radio Shack)
- Power entry component ($0.60 local hardware store)
- e-Stop module ($5 for 2 - eBay)
- 4 x 4-pin connectors ($5 for pack of 4)
- M3 &amp; M5 bolts ($5 local hardware store)
- USB cabe ($3)
- Power Cable ($1.49)
- Extra cables ($6 for 6 feet from Inventables)
- Arduino ($35 Radio Shack)
- GRBL Shield ($69 Synthesos.com)

&nbsp;
<h3 style="text-align: left;">The Design</h3>
<a href="http://www.shapeoko.com/wp-content/uploads/2013/11/shapeoko-enclosure-design.jpg"><img class="alignnone size-full wp-image-1141" alt="Shapeoko_Electronics-Enclosure.3dm" src="http://www.shapeoko.com/wp-content/uploads/2013/11/shapeoko-enclosure-design.jpg" width="600" height="334" /></a>

The design is simple and minimalistic, yet flexible enough to make it easy to incorporate different electronics, not only the grbl-shield. For some components some slight readjustments might be necessary, but for the most part I used standard and readily available components available online or at most local electronics stores. I will add all design files (designed in Rhino 3D, but will export to various different file extensions) for anyone to adjust and redesign to make it their own. In addition I designed a few variations and have files ready to cut in both 1/4" as well as 1/8" thickness. For this page I will however, only discuss the 1/4" option, but the concept remains the same.

&nbsp;
<h3 style="text-align: left;">Fabrication of Parts</h3>
<a href="http://www.shapeoko.com/wp-content/uploads/2013/11/shapeoko-enclosure-laser-cut-parts1.jpg"><img class="alignnone size-full wp-image-1146" alt="Shapeoko_Electronics-Enclosure.3dm" src="http://www.shapeoko.com/wp-content/uploads/2013/11/shapeoko-enclosure-laser-cut-parts1.jpg" width="600" height="334" /></a>

The cutting files are shown above (click on the image for a larger image). <a title="ShapeOko Cut Files" href="http://www.shapeoko.com/wp-content/uploads/2013/11/Shapeoko-Enclodure-option-1.zip">Click here to download the .dxf </a>of the above drawing. I have provided several additional links at the bottom of the page for other formats and variations of this design in 1/4" and 1/8" materials. Just as an overview. The first two parts are the front and back showing the holes for ventilation. The 4 holes around it are to attach a cooling fan (as many variations exist make sure to get one that will fit the size, if you buy a different fan it might not fit). Secondly the Arduino mount is shown, which is simply a small platform on which the Arduino rests. If you are using a different controller and stepper driver, simply adjust it for what you are using. The top and bottom are cut out, notice the circle on the top portion, this is where the emergency stop button will be placed. Next we have Left, Right and R-Inner (Right inner engraving). Do not cut 'R-Inner' out, this is simply meant to engrave on the reverse side of the 'Right' side, right on the other side of where the text X Y Z O is). This is done as the 4-pin connectors have a short threaded part for the material used. By engraving we can make the thickness smaller in that particular area (this is illustrated below).

<img class="alignnone size-full wp-image-1164" alt="shapeoko-enclosure-laser-cut" src="http://www.shapeoko.com/wp-content/uploads/2013/11/shapeoko-enclosure-laser-cut.jpg" width="600" height="322" />

The files are ready to use, however, finding the exact thickness of wood is tricky 1/4" wood might be thinner in some stores and thicker in others and even have varying thickness based on wood type). The files are easy to adjust with a little knowledge of CAD software you can make it fit with no problems. In addition the accuracy of your laser cutter will affect how well the parts fit together (less accuracy might cause the cutting line to have a larger thickness than a more accurate machine). I would advise anyone new to laser cutting (or anyone else in fact) to make a small test of the press fit size to see how loose or tight the design is for the wood  as well as the machine you are using.

&nbsp;
<h3 style="text-align: left;">Assembly of Enclosure:</h3>
<img class="alignnone size-full wp-image-1165" alt="Shapeoko-Enclodure-assembly-01" src="http://www.shapeoko.com/wp-content/uploads/2013/11/Shapeoko-Enclodure-assembly-01.jpg" width="600" height="322" />

The image above shown the laser cut components. If you have the correct wood or have adjusted the files slightly, this should be everything you need to put it together. My enclosure fit together so tight it did not need additional hardware or glue, which made assembly extremely easy.

<img class="alignnone size-full wp-image-1166" alt="Shapeoko-Enclodure-assembly-02" src="http://www.shapeoko.com/wp-content/uploads/2013/11/Shapeoko-Enclodure-assembly-02.jpg" width="600" height="322" />

The above image shows the parts press fitting together, making assembly quick and easy.

<img class="alignnone size-full wp-image-1167" alt="Shapeoko-Enclodure-assembly-03" src="http://www.shapeoko.com/wp-content/uploads/2013/11/Shapeoko-Enclodure-assembly-03.jpg" width="600" height="322" />

Once you are sure everything fits together tightly, you can sand it down, paint it or leave it as is. The press fit construction should be tight and solid, taking off the sides and top should be simple allowing you to easily add the electronics. Adding the electronics should take no more than an hour to complete.

&nbsp;
<h3>Adding Electronic Components:</h3>
<p style="text-align: left;"> In the end, the electronics with enclosure came out to be just about $160 (most components bought locally).</p>
<p style="text-align: left;"><a href="http://fablabsf.org/wp-content/uploads/2013/03/enclosure-front.jpg"><img alt="Image" src="http://fablabsf.org/wp-content/uploads/2013/03/enclosure-front.jpg" width="600" height="905" /></a></p>
<p style="text-align: left;">The image above shows an overview of all components and where they are located. These components are:</p>
&nbsp;
<p style="text-align: left;"><strong>1. 24v 5a power supply (eBay $15 incl. shipping)</strong></p>
<p style="text-align: left;"><img class="alignnone size-full wp-image-1172" alt="power-supply" src="http://www.shapeoko.com/wp-content/uploads/2013/11/power-supply.jpg" width="600" height="323" /></p>
<p style="text-align: left;">Available at various stores. Buying a higher amp power supply is perfectly fine too, just do not buy anything lower than 5 amps. Generally the higher the amps the more expensive. I bought this one for $10 on eBay.</p>
&nbsp;
<p style="text-align: left;"><strong> 2. One or two 24v 1.4w Papst Fan ($10 each eBay)</strong></p>
<p style="text-align: left;"><a href="http://www.shapeoko.com/wp-content/uploads/2013/11/papst-fan.jpg"><img class="alignnone size-full wp-image-1173" alt="papst-fan" src="http://www.shapeoko.com/wp-content/uploads/2013/11/papst-fan.jpg" width="600" height="323" /></a></p>
<p style="text-align: left;">Papst fans are one of my favorite and have used them of several projects. Cost is about $8 each. I bought a Papst 8414 M (but similar fan works just as well). I have the option to have one at either end to increase air flow allowing for faster cooling, however, with grbl-shield that is hardly necessary. Start with one and add another if it hears up too much.</p>
&nbsp;
<p style="text-align: left;"><strong> 3. <strong>Power switch</strong>  ($3 at Radio Shack) &amp; <strong>Power entry component  ($0.60)</strong>
</strong></p>
<img alt="Image" src="http://fablabsf.org/wp-content/uploads/2013/03/enclosure-power-connection.jpg" width="600" height="398" />

Using a power switch and 3 prong power connector. Very cheap and easy set up compared to a power entry module. A possible upgrade switch would be one with a light which would only set you back a dollar or two.

&nbsp;
<p style="text-align: left;"><strong> 4. e-Stop module ($5 for 2 - eBay)</strong></p>
<p style="text-align: left;"><strong><img class="alignnone size-full wp-image-1174" alt="e-stop" src="http://www.shapeoko.com/wp-content/uploads/2013/11/e-stop.jpg" width="600" height="323" /></strong></p>
<p style="text-align: left;">The E-stop button is simply connected to the live wire. It allows you to quickly shut the system down before damaging anything. I placed it on the top of the enclosure to easily hit down on it if something went wrong (even though the image below looks like it is on the side, it is in fact on top of the enclosure).</p>
<img alt="Image" src="http://fablabsf.org/wp-content/uploads/2013/03/enclosure-top.jpg" width="600" height="398" />

The top of the enclosure showing the e-stop button connected. Thinking about making the top from transparent acrylic.

&nbsp;
<p style="text-align: left;"><strong> 5. 4 x 4-pin connectors ($6.95 for pack of 4 from <a title="4 pin panel connector" href="https://www.inventables.com/technologies/panel-connector-4-pin" target="_blank">Inventables.com</a>)</strong></p>
<p style="text-align: left;"><a href="http://www.shapeoko.com/wp-content/uploads/2013/11/four-pin-panel-connectors.jpg"><img class="alignnone size-full wp-image-1175" alt="four-pin-panel-connectors" src="http://www.shapeoko.com/wp-content/uploads/2013/11/four-pin-panel-connectors.jpg" width="600" height="323" /></a></p>
<p style="text-align: left;">Very cheap way to connect your motors to the driver. I love them because they can easily be disconnected and are secure enough that you do not have to worry about wires becoming disconnected (and damaging your machine).</p>
<img alt="Image" src="http://fablabsf.org/wp-content/uploads/2013/03/enclosre-side.jpg" width="600" height="396" />

I added four 4-pin connectors for use with additional motors in the future (only using 3 at the moment but will install the second Y-axis motor soon as I upgrade to Mach3 or similar). Make sure to get something that will not get disconnected easily as it can destroy your motors! These connectors screw on and stay firmly in place.

<img alt="Image" src="http://fablabsf.org/wp-content/uploads/2013/03/enclosure-raster.jpg" width="600" height="396" />

I used a raster to cut into the wood as it was too thick for the pins. Since this is my first CNC I used a laser cutter instead. I ran a raster engrave and just repeated the raster over again until I had the thickness just right. If you use 4-pin connectors make sure the threaded part is long enough to fit through.

&nbsp;
<p style="text-align: left;"><strong> 6. Cables (various)
</strong></p>
<p style="text-align: left;"><img class="alignnone size-full wp-image-1176" alt="cables" src="http://www.shapeoko.com/wp-content/uploads/2013/11/cables.jpg" width="600" height="323" /></p>
<p style="text-align: left;">Stepper Motor Cable ($6 for 6 feet from <a title="stepper motor cables" href="https://www.inventables.com/technologies/stepper-motor-cable" target="_blank">Inventables.com</a>), USB type B cable ($3) and a 3 prong power cable ($1.49 - regular computer cable to fit the power entry module).</p>
&nbsp;
<p style="text-align: left;"><strong>7. M3 &amp; M5 bolts ($5 local hardware store)</strong></p>
<p style="text-align: left;">M3 and M5 bolts at various lengths and hex nuts to fit them.</p>
&nbsp;
<p style="text-align: left;"><strong> 8. Arduino Uno ($35 Sparkfun / Radio Shack)</strong></p>
<p style="text-align: left;"><img class="alignnone size-full wp-image-1177" alt="arduino" src="http://www.shapeoko.com/wp-content/uploads/2013/11/arduino.jpg" width="600" height="323" /></p>
<p style="text-align: left;">Make sure to get the newer version. For more information read the Wiki on ShapeOko.com.</p>
&nbsp;
<p style="text-align: left;"><strong> 9. GRBL Shield ($69 Synthesos.com)</strong></p>
<p style="text-align: left;"><img class="alignnone size-full wp-image-1178" alt="grbl-shield" src="http://www.shapeoko.com/wp-content/uploads/2013/11/grbl-shield.jpg" width="600" height="323" /></p>
<p style="text-align: left;">Grbl-Shield from Synthesos.com.</p>
&nbsp;
<h3 style="text-align: left;">The Files:</h3>
<a title="ShapeOko Enclosure - Laser Cutting Lab, LLC" href="http://lasercuttinglab.com/wp-content/uploads/2013/11/ShapeOko-Electronics-Enclosure-v2.zip"><img class="alignnone size-full wp-image-1185" alt="shapoko-electronics-enclosure-files" src="http://www.shapeoko.com/wp-content/uploads/2013/11/shapoko-electronics-enclosure-files.jpg" width="600" height="322" /></a>

This is the main file folder with original file drawn in Rhinoceros / Rhino 3D. I exported the files to .dwg, .dxf and .ai (hav not tested .ai yet). If any other file types are wanted or needed please let me know and I will try to add them.
<h3 style="text-align: center;"><a title="ShapeOko Enclosure - Laser Cutting Lab, LLC" href="http://lasercuttinglab.com/wp-content/uploads/2013/11/ShapeOko-Electronics-Enclosure-v2.zip">Download ShapeOko Files, designed by Laser Cutting Lab, LLC (10.6mb)</a></h3>
Thank you for your interest in this project and I hope you will enjoy making one for your new ShapeOko 2 that is about to be released or on your original ShapeOko. ShapeOko is an amazing machine and we thank Edward for the invitation to share our enclosure.
Mathew Owen
Laser Cutting Lab, LLC
www.lasercuttinglab.com
