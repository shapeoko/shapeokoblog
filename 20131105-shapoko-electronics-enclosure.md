title: ShapeOko Electronics Enclosure
link: http://www.shapeoko.com/archives/1102
author: mathewowen
description: 
post_id: 1102
created: 2013/11/05 16:46:24
created_gmt: 2013/11/05 22:46:24
comment_status: open
post_name: shapoko-electronics-enclosure
status: publish
post_type: post

# ShapeOko Electronics Enclosure

### _The following post is from guest blogger Matthew Owen. Matthew is a member of the Shapeoko community, a maker, founder of [Laser Cutting Lab, LLC](http://lasercuttinglab.com/shop/), and an all around cool guy. _

* * *

 

### ShapeOko Enclosure by [Laser Cutting Lab, LLC](http://lasercuttinglab.com)

I decided to build an electronics enclosure for my ShapeOko and recently acquired ShapeOko 2 (pre-order). The suggested curved acrylic plate was nice but not entirely practical. Besides, I enjoyed designing and building this enclosure so for anyone interested, here it is.

###  The List of Components:

\- 1/4" birch plywood - 24" x 12" - 3 pieces ($10 hardware store) \- 24v 5a power supply (eBay $15 incl. shipping) \- 24v 1.4w Papst Fan ($10 eBay) \- Power switch ($3.19 at Radio Shack) \- Power entry component ($0.60 local hardware store) \- e-Stop module ($5 for 2 - eBay) \- 4 x 4-pin connectors ($5 for pack of 4) \- M3 & M5 bolts ($5 local hardware store) \- USB cabe ($3) \- Power Cable ($1.49) \- Extra cables ($6 for 6 feet from Inventables) \- Arduino ($35 Radio Shack) \- GRBL Shield ($69 Synthesos.com)  

### The Design

![Shapeoko_Electronics-Enclosure.3dm](/wp-content/uploads/2013/11/shapeoko-enclosure-design.jpg) The design is simple and minimalistic, yet flexible enough to make it easy to incorporate different electronics, not only the grbl-shield. For some components some slight readjustments might be necessary, but for the most part I used standard and readily available components available online or at most local electronics stores. I will add all design files (designed in Rhino 3D, but will export to various different file extensions) for anyone to adjust and redesign to make it their own. In addition I designed a few variations and have files ready to cut in both 1/4" as well as 1/8" thickness. For this page I will however, only discuss the 1/4" option, but the concept remains the same.  

### Fabrication of Parts

![Shapeoko_Electronics-Enclosure.3dm](/wp-content/uploads/2013/11/shapeoko-enclosure-laser-cut-parts1.jpg) The cutting files are shown above (click on the image for a larger image). [Click here to download the .dxf ](http://www.shapeoko.com/wp-content/uploads/2013/11/Shapeoko-Enclodure-option-1.zip)of the above drawing. I have provided several additional links at the bottom of the page for other formats and variations of this design in 1/4" and 1/8" materials. Just as an overview. The first two parts are the front and back showing the holes for ventilation. The 4 holes around it are to attach a cooling fan (as many variations exist make sure to get one that will fit the size, if you buy a different fan it might not fit). Secondly the Arduino mount is shown, which is simply a small platform on which the Arduino rests. If you are using a different controller and stepper driver, simply adjust it for what you are using. The top and bottom are cut out, notice the circle on the top portion, this is where the emergency stop button will be placed. Next we have Left, Right and R-Inner (Right inner engraving). Do not cut 'R-Inner' out, this is simply meant to engrave on the reverse side of the 'Right' side, right on the other side of where the text X Y Z O is). This is done as the 4-pin connectors have a short threaded part for the material used. By engraving we can make the thickness smaller in that particular area (this is illustrated below). ![shapeoko-enclosure-laser-cut](http://www.shapeoko.com/wp-content/uploads/2013/11/shapeoko-enclosure-laser-cut.jpg) The files are ready to use, however, finding the exact thickness of wood is tricky 1/4" wood might be thinner in some stores and thicker in others and even have varying thickness based on wood type). The files are easy to adjust with a little knowledge of CAD software you can make it fit with no problems. In addition the accuracy of your laser cutter will affect how well the parts fit together (less accuracy might cause the cutting line to have a larger thickness than a more accurate machine). I would advise anyone new to laser cutting (or anyone else in fact) to make a small test of the press fit size to see how loose or tight the design is for the wood  as well as the machine you are using.  

### Assembly of Enclosure:

![Shapeoko-Enclodure-assembly-01](/wp-content/uploads/2013/11/Shapeoko-Enclodure-assembly-01.jpg) The image above shown the laser cut components. If you have the correct wood or have adjusted the files slightly, this should be everything you need to put it together. My enclosure fit together so tight it did not need additional hardware or glue, which made assembly extremely easy. ![Shapeoko-Enclodure-assembly-02](http://www.shapeoko.com/wp-content/uploads/2013/11/Shapeoko-Enclodure-assembly-02.jpg) The above image shows the parts press fitting together, making assembly quick and easy. ![Shapeoko-Enclodure-assembly-03](http://www.shapeoko.com/wp-content/uploads/2013/11/Shapeoko-Enclodure-assembly-03.jpg) Once you are sure everything fits together tightly, you can sand it down, paint it or leave it as is. The press fit construction should be tight and solid, taking off the sides and top should be simple allowing you to easily add the electronics. Adding the electronics should take no more than an hour to complete.  

### Adding Electronic Components:

 In the end, the electronics with enclosure came out to be just about $160 (most components bought locally).

![Image](http://fablabsf.org/wp-content/uploads/2013/03/enclosure-front.jpg)

The image above shows an overview of all components and where they are located. These components are:

 

**1\. 24v 5a power supply (eBay $15 incl. shipping)**

![power-supply](/wp-content/uploads/2013/11/power-supply.jpg)

Available at various stores. Buying a higher amp power supply is perfectly fine too, just do not buy anything lower than 5 amps. Generally the higher the amps the more expensive. I bought this one for $10 on eBay.

 

** 2\. One or two 24v 1.4w Papst Fan ($10 each eBay)**

![papst-fan](/wp-content/uploads/2013/11/papst-fan.jpg)