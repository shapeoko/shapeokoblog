---
layout: post
title: Better DXF exports from Inkscape
date: 2012-08-21 10:50
author: smadmin
comments: true
categories: [Shapeoko, Software]
---
If you're using <a href="http://www.inkscape.org" target="_blank">Inkscape</a> as part of your CNC software stack, you may have found the default Inkscape DXF export utility to be um... lacking. To say the least. Exporting vector images as DXF from Inkscape with the default DXF module will result in a mangled mess of layers, lines, and long evenings trying to piece things back together.

For instance, here is a simple coaster I drew with inkscape:

<a href="http://www.shapeoko.com/wp-content/uploads/2012/08/coast_original.png"><img class="alignnone size-medium wp-image-875" title="coast_original" src="http://www.shapeoko.com/wp-content/uploads/2012/08/coast_original-300x159.png" alt="" width="300" height="159" /></a>

I then saved the file as 'Desktop Cutting Plotter (R13) (*.dxf).

But, when I tried to import the saved dxf into HeeksCNC, I was met with the unpleasant side effect of not all the paths being joined together where they should be. If you cound the number of sketches in the left pain, you'll see a lot of them. There should be one sketch per path, resulting in 9 paths total:

1.) Outside perimeter

2.) Inside decorative edge

3-5.) Letters: C, S, T

6.) Outside of Letter  'O'

7.) Inside of Letter 'O'

8.) Outside of Letter 'A'

9.) Inside of Letter 'A'

It's important that the paths are correctly turned into sketches because that's how we control the toolpaths. Think of the letter 'O': If we machined both the outside and the inside in the same fashion, you'd be left with a shell of a letter. Same with the letter A.

That issue can be resolved in HeeksCNC, but proved to be a PITA and not something I would want to have to do every time I imported a DXF file. Or ever again for that matter.

<a href="http://www.shapeoko.com/wp-content/uploads/2012/08/broken_coaster_import.png"><img class="alignnone size-medium wp-image-874" title="broken_coaster_import" src="http://www.shapeoko.com/wp-content/uploads/2012/08/broken_coaster_import-300x157.png" alt="" width="300" height="157" /></a>

Luckily, the people over at <a href="http://www.bigbluesaw.com/saw/big-blue-saw-blog/general-updates/big-blue-saws-dxf-export-for-inkscape.html">Big Blue Saw</a> have a fix for you (and me!) that will result in perfect DXF exports every time.

Here's the same inkscape file, saved as Big Blue Saw DXF Output (*.DXF) imported into HeeksCNC:

<a href="http://www.shapeoko.com/wp-content/uploads/2012/08/proper_coaster_import.png"><img class="alignnone size-medium wp-image-876" title="proper_coaster_import" src="http://www.shapeoko.com/wp-content/uploads/2012/08/proper_coaster_import-300x160.png" alt="" width="300" height="160" /></a>

&nbsp;

Notice the number of Sketches! Yep, there are 9 there, just as we would expect.
