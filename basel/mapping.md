# Day 3: Mapping
## Overview of today
Today we will 
* spend some time on an overview of mapping tools, projects, and gazeteers for the ancient world
* create basic maps in Google maps and other tools using existing non-ancient spreadsheet data
* community source maps and spreadsheet data using ancient data and tools/projects for antiquity we have examined
* discuss the limitations of geographical mapping for spatial research (e.g., what about places we cannot map onto a site?)



## Mapping Tools, Projects, and Gazeteers
### Sample list
* [Orbis](http://orbis.stanford.edu/) - click on "Using" for instructions/tutorial, or just play around with it
* [Pelagios](http://commons.pelagios.org/) - linked data hub for ancient mapping/geographical study (aggregates data from other sites)
* [Recogito](http://recogito.pelagios.org/) - tool for annotating text and images with geographic data
* [Pleiades](https://pleiades.stoa.org/) - ancient world gazetteer (aggregates data from other sites, mostly through Pelagios)
* [Antiquity a la carte map creator](http://awmc.unc.edu/awmc/applications/alacarte/)
* [Syriaca gazetteer for places mentioned in Syriac literature](http://syriaca.org/geo/index.html)
* [QGIS](https://www.qgis.org/en/site/) - open source mapping software; powerful; not specifically for antiquity, download+install
* [ArcGIS](http://www.arcgis.com/) - commercial software with stripped down public web service; does not do well searching for ancient sites, but you could upload data from another site (Recogito, antiquity-a-la-carte, Pleiades, etc.)
* [Harvard World Maps](http://worldmap.harvard.edu/) - open source mapping software; powerful; not specifically for antiquity
* [Google tables](https://support.google.com/fusiontables/answer/2571232?hl=en) - create maps using spreadsheet data & Google fusion tables
* [Google "my maps"](https://mymaps.google.com) You can create and save maps in Google
* [Carto](https://carto.com/) - commercial mapping tool with free scaled down option; not specifically for antiquity
* [Tableau](https://www.tableau.com/) - commercial mapping and data visualization tool; not specifically for antiquity

One interesting non-ancient project is Palladio and the Republic of Letters
*  http://republicofletters.stanford.edu/publications/voltaire/
*  http://republicofletters.stanford.edu/publications/franklin/
*  Free tool at:  http://hdlab.stanford.edu/palladio/ (they have a sample data set you can use)

### Step 1: [Orbis](http://orbis.stanford.edu/)
Spend some time playing with Orbis to calculate routes in the ancient world.  The About page will tell you more about the data sources.

Map a route from your favorite city to Rome or Alexandria
*  What does the route look like in different seasons?
*  Is the cheapest route the same as the fastest route?  Is the fastest route the same as the shortest route?
*  Pretend you get seasick:  omit the Open Sea from your route.  
*  Pretend you get really really seasick: omit the Open Sea and the Coastal Sea from your route
*  Make sure the bottom pane is open: Look in the bottom pane for information about how much it costs and the methods to get from one place to another (I believe dark blue is open sea, light blue river, green coastal sea, brownish road)
*  Minimize the bottom pane -- play around with the modes of travel

**Pro tip**:  Orbis layers one route on top of the next in your map.  Click reset map on the right to clear it.**

Click on "Network"
*  Choose fastest, cheapest, or shortest
*  Calculate Network -- see how the cities on the map are shaded based on the cost (in terms of distance, time, $)
*  Make sure the bottom pane is open:  Click on Cartogram (not in Distance network but in others) -- what happens?  Click on Zones -- what happens?

To my knowledge, you can download an SVG file (can only be opened in certain programs, doesn't contain map tiles background) or take a screenshot

### Step 2: Visit [Pleiades](https://pleiades.stoa.org/) and [Pelagios](http://commons.pelagios.org/)
Search in Pleiades for your favorite places
*  What's easy or difficult about the search?
*  Look for common and not so common places -- how much information about these places is there?
*  Where is the data coming from for these places?
*  What else interesting do you notice about the data?

What is Pelagios?  Anything you could use it for?
*  Explore data > Roman map  Check out the Roman empire map.  How could this be useful?
*  Linked Data > Search Peripleo:  Search Peripleo for one of the places you searched Pleiades.  What's similar and different about the results?
*  How might you use a linked data hub for a project?

**_If you're interested in a background map tile, you can check out the [Roman Empire map tiles](http://commons.pelagios.org/2012/09/a-digital-map-of-the-roman-empire/)_**

**_If your project has place names or geographic information, you can LINK TO Pelagios & Pleiades with their stable URLs, and you can arrange for them to LINK TO YOUR PROJECT if you have stable URLs_**

### Step 4:  Visit [Syriaca.org Gazetteer](http://syriaca.org/geo/index.html)
What is this?

Search for a site -- what information is there, where is it from?

How did they build the gazetter?

Could this be a model for other projects?

### Step 5:  Make a map using [Antiquity a la carte map creator](http://awmc.unc.edu/awmc/applications/alacarte/)
This map like many map services uses *layers*: you have base terrain or road layers, and then you layer on top more information -- each kind getting its own layer.

First play around:
*  Map layers:  Check and uncheck boxes especially in Cultural data > physical culture and political areas and physical data
*  Search for features
  * Before you click on the button, be sure Features is selected in the Physical Culture layer, otherwise you can't add it to a map
  * Search for a TYPE of place -- I tried "monastery" ... which had an interesting result
  * Search for major named place, such as Antioch -- what do you notice about the results?
    * Add one of your results to the map
    * For Antioch, can you add all the results to the map or not?  Why?

Make the map the way you want it to look, with the layers you want and features you want.

Under File, export it or save the URL to your map so you can use it later

If you download a .kml file you can upload it into Google Maps:  https://support.google.com/mymaps/answer/3024836?co=GENIE.Platform%3DDesktop&hl=en

Access your maps in Google maps at https://mymaps.google.com/

*_Go to mymaps.google.com and make a map by SEARCHING for the same places you searched for in Antiquity-a-la-carte -- what happens?  Which is easier? Which gives you better data? Which gives you more data?_*

### Step 6:  Geotag a text using [Recogito](http://recogito.pelagios.org/)
Pick a text from Perseus in English translation and geotag it!
* Find a text at Perseus -- I picked [Caesar's Gallic War 1.1](http://www.perseus.tufts.edu/hopper/text?doc=Perseus:text:1999.02.0001), since it was right there on the homepage and I knew it contained geo data.  **Copy only the text** and save it as a text file (.txt) on your computer
* Go to http://recogito.pelagios.org/ and create a new account
* Follow the steps to upload your text file -- note you can provide some metadata about the edition you are using, etc.
* Follow the steps to tag your texts for entities and then proofread (this is a pretty userfriendly interface)
* After you've corrected your text, click on icon for the Map View to see the map
* Click on the Download icon to download your data in various forms. 
  * Choose csv form for one of your downloads -- we may try to upload it into Google maps or another tool and see what happens
  * Choose JSON for another download -- we may try to upload to antiquity a la carte 

Are there "spaces" and "places" that don't get mapped in my Gallic War example?

### Step 7:  Let's make a map!

You can use a data source you created in one of the previous steps, or we can community-source a map using data in a Google Spreadsheet.  I'll email you a link via Adam.

If you use a csv file or spreadsheet, you may find that different tools want your geo data in slightly different forms (i.e., one field for lattitude/longitude combined or separate fields for lattitude & longitude)

You can also find your own data, say your favorite papyri in Papyri.info, your geotagged text from Recogito, etc.

If you want a quick dataset good for mapping but has nothing do to with antiquity, here is a set of photographs that are geotagged:
*  [Cushman collection of photos at Indiana](http://bit.ly/cushmancollection)
*  [Cushman collection with latitude/longitude in separate fields](https://github.com/ctschroeder/tutorials/blob/master/basel/files/cushman-collection-lat-long-disagg.csv)

We will try to make maps in:
* [Antiquity a la carte map creator](http://awmc.unc.edu/awmc/applications/alacarte/)
* [ArcGIS](http://www.arcgis.com/) -- requires a registration; free trial period. You can upload your csv files
* [Harvard World Maps](http://worldmap.harvard.edu/)
* [Google tables](https://support.google.com/fusiontables/answer/2571232?hl=en) -- CLICK THIS link to link your Google account to the Fusion Tables app
* [Carto](https://carto.com/) - commercial mapping tool with free scaled down option; not specifically for antiquity -- contact them for info about a free version as an educator, for a class, etc.
* [Tableau](https://www.tableau.com/) - commercial mapping and data visualization tool; not specifically for antiquity.  Scroll down for the free trial.

#### If we have time, play around with Palladio's sample data set http://hdlab.stanford.edu/palladio/

### Some things we learned
Different programs prefer differently formatted data: some required longitude and lattitude in the same field, some placed long/lat in different orders in that field, and others required them in separate fields.
*  Use Excel/Sheets formulas to join data into one field (i.e., =A2&","B2 should merge data from A2 & B2 columns)
*  Use Excel/Sheets to split lat/long data that's joined. Protip: copy it into a new column first, so you have one column with the joined data for some apps, and columns with the split data for other apps.  https://support.google.com/docs/answer/6325535?co=GENIE.Platform%3DDesktop&hl=en

Opening a csv file in Excel can corrupt the data

Clean our data:  use the power of Google Sheets or Excel to get rid of extraneous junk in our long/lat fields

mymaps.google.com is easier than Google Fusion maps, but it doesn't visualize thumbnail images for image URLs



### Discussion

What works and doesn't work with these tools?  

What was your experience with collecting, organizing, and cleaning your data?

What is getting mapped?  At what level of granularity (city, building, exact find spot)?

What isn't getting mapped?  How else might you capture that information?
