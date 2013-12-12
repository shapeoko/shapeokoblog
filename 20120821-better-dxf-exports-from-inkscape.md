title: Better DXF exports from Inkscape
link: http://www.shapeoko.com/archives/872
author: smadmin
description: 
post_id: 872
created: 2012/08/21 10:50:02
created_gmt: 2012/08/21 16:50:02
comment_status: open
post_name: better-dxf-exports-from-inkscape
status: publish
post_type: post

# Better DXF exports from Inkscape

If you're using [Inkscape](http://www.inkscape.org) as part of your CNC software stack, you may have found the default Inkscape DXF export utility to be um... lacking. To say the least. Exporting vector images as DXF from Inkscape with the default DXF module will result in a mangled mess of layers, lines, and long evenings trying to piece things back together. For instance, here is a simple coaster I drew with inkscape: ![](/wp-content/uploads/2012/08/coast_original-300x159.png) I then saved the file as 'Desktop Cutting Plotter (R13) (*.dxf). But, when I tried to import the saved dxf into HeeksCNC, I was met with the unpleasant side effect of not all the paths being joined together where they should be. If you cound the number of sketches in the left pain, you'll see a lot of them. There should be one sketch per path, resulting in 9 paths total: 1.) Outside perimeter 2.) Inside decorative edge 3-5.) Letters: C, S, T 6.) Outside of Letter  'O' 7.) Inside of Letter 'O' 8.) Outside of Letter 'A' 9.) Inside of Letter 'A' It's important that the paths are correctly turned into sketches because that's how we control the toolpaths. Think of the letter 'O': If we machined both the outside and the inside in the same fashion, you'd be left with a shell of a letter. Same with the letter A. That issue can be resolved in HeeksCNC, but proved to be a PITA and not something I would want to have to do every time I imported a DXF file. Or ever again for that matter. ![](http://www.shapeoko.com/wp-content/uploads/2012/08/broken_coaster_import-300x157.png) Luckily, the people over at [Big Blue Saw](http://www.bigbluesaw.com/saw/big-blue-saw-blog/general-updates/big-blue-saws-dxf-export-for-inkscape.html) have a fix for you (and me!) that will result in perfect DXF exports every time. Here's the same inkscape file, saved as Big Blue Saw DXF Output (*.DXF) imported into HeeksCNC: ![](http://www.shapeoko.com/wp-content/uploads/2012/08/proper_coaster_import-300x160.png)   Notice the number of Sketches! Yep, there are 9 there, just as we would expect.

## Comments

**[Simon Arthur](#126 "2012-09-20 17:22:43"):** If you run into further difficulty, another tactic is to export as EPS, then run the command line took pstoedit to convert to DXF.

