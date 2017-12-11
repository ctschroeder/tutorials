*DRAFT in progress*

# DAY 2: Text Analysis and Natural Language Processing

This tutorial will introduce participants to simple digital text analysis using out-of-the-box tools.  For more complex stylometry methods, see:
* Arnold and Tilton [Humanities Data in R](https://humanitiesdata.org/)
* Jockers, [Text Analysis with R for Students of Literature](https://books.google.de/books?id=K4_IAwAAQBAJ&dq=text+analysis+in+r&source=gbs_navlinks_s)
* The many tutorials online for working in R, such as the ones linked on this [Washington University guide](http://libguides.wustl.edu/R)

## PLEASE DOWNLOAD and INSTALL before the workshop

Voyant [download here](https://github.com/sgsinclair/VoyantServer/releases/tag/2.4.0-M2); [info about how to install here](http://docs.voyant-tools.org/resources/run-your-own/voyant-server/) A web interface available but sometimes it slows if many people tax the server; 

[AntConc](http://www.laurenceanthony.net/software/antconc/) (no web interface, please download and install)

If you have difficulties, we can spend a few minutes in the beginning getting it installed.

## Optional Reading before the Workshop
[Sinclair and Rockwell, "Text Analysis and Visualization" in A New Companion to Digital Humanities](https://github.com/ctschroeder/tutorials/blob/master/basel/files/Sinclair-Rockwell-ch19.pdf) -- note: this file will be removed soon after the workshop

## What is Text Analysis?

Distant Reading
Computationally aided Philological research
Stylistics (including author identification)
Corpus Linguistics
Much more...

Question:  Yesterday we looked at "word frequencies" in Perseus and Coptic Scriptorium corpora. Why would word frequency information be useful?

Extremely accessible online readings in addition to the Sinclair/Rockwell article:
Paige Morgan blog post: ["This Talk Doesn't Have a Name"](http://blog.paigemorgan.net/articles/17/this-talk/): note Harry Potter and Clinton/Trump analysis
Slate article: ["A Textual Analysis of the Hunger Games"](http://www.slate.com/articles/arts/culturebox/2013/11/hunger_games_catching_fire_a_textual_analysis_of_suzanne_collins_novels.html): note comparisons of vocabulary and common sentences across popular young adult book series

Content words vs "function" words ("stop words")
* Sometimes you might want to strip out function words (pronouns, articles, etc.) to see the content of texts
* Sometimes you want to research function words (gender analysis using pronoun study, linguistics, authorship identification)

## Authorship identification
Slate article: ["Can You Identify an Author By How Often They Use the Word “The”?"](http://www.slate.com/blogs/browbeat/2017/08/17/identifying_an_author_s_prose_can_be_as_simple_as_counting_how_much_they.html)
José Nilo G. Binongo, [Who Wrote the 15th Book of Oz?](http://dh.obdurodon.org/Binongo-Chance.pdf)
Patrick Juola, ["How a Computer Program Helped Show J.K. Rowling write A Cuckoo’s Calling"](https://www.scientificamerican.com/article/how-a-computer-program-helped-show-jk-rowling-write-a-cuckoos-calling/)
10 Nov 2017 authorship identification lecture by Patrick Juola at University of Pittsburgh
*  Part 1: https://youtu.be/u_x0Zs6_14M
*  Part 2: https://youtu.be/X6Xvh4SONzA
*  Part 3: https://youtu.be/Sp9YDSXGi6A
*  Slides: https://github.com/ebeshero/DHClass-Hub/blob/master/Assignment-Files/Juola-Files/Pitt-Authorship2016.ppt

[Juola's authorship program is free, downloadable](https://github.com/evllabs/JGAAP)

## Distant reading and text analysis with Voyant Tools

If you did not download and install Voyant, visit http://voyant-tools.org/

*Consider working in PAIRS so we don't load the server too much.*

### First try English

1.  Open an existing corpus
2.  What's the first thing you notice about the word cloud?

*Understanding the page*
In what they call the “default skin”- you will see five panels. Each of these is a tool, Cirrus, Reader, Trends, Summary, and Contexts. These tools interact with one another – if you modify one pane, you may see another update.
The appearance of each of these windows can be modified. Place the cursor on the ? symbol over any given tool, and a menu of options will appear. (Note: hover over the titles of these navigation buttons for descriptions.)
![Voyant Overview](https://github.com/ctschroeder/tutorials/blob/master/images/Voyant-overview-hover.png)

You may need to expand the window of your tool to be able to see the full menu.
![window](https://github.com/ctschroeder/tutorials/blob/master/images/Voyant-overview-moved-window.png)

The first icon below allows you to download data or create a web URL so you can come back to your corpus and this tool.

The second icon allows you to switch to a new tool.

The third icon allows you to define options for the tool. (circled)
![tool menu](https://github.com/ctschroeder/tutorials/blob/master/images/Voyant-extra-tools-menu.png)

*Returning to our English analysis...*

3.  If one of the first things you noticed was the absence of function words
   * Click on the icon to define options for the tool
   * The "stop list" is the list of words you DON'T want analyzed. If you want to include function words, you can unselect the Stop Word list or modify it
4.  Click on "Terms" above the word cloud -- look at the word frequencies
5.  _You almost always want information about *relative* frequencies not *raw* frequencies, so you can compare_
   *  Hover at the right corner of the Terms table, under the question mark: select "Columns" in the drop down menu
   *  Add a "relative frequency" column
6.  Now, click on "Links" (next to terms)
   *  What shows up automatically?
   *  Clear the terms
   *  Try "king" followed by an asterix and "queen" followed by an asterix
   *  What happens?
   *  What happens when you move the context slider?

### Download your analysis
7.  In the "Links" view, click the button to download data or create a web URL
   *  You can download a static image file
   *  You can download code to put into your website for a dynamic visualization
   *  You can open the tool in a new window
   * ...
8.  Click on the "Terms" view
   * Click on the button to download your data (same as above)
   * Download your word frequencies

### Let's try this in Latin!!!!

_STEP 1_ Upload a text from Corpus Corporum in Latin using a LINK:
*  In a new tab or window, go to http://mlat.uzh.ch/MLS/
*  Click on Patrologia Latina
*  Scroll down and click on Augustus Hipponensis
*  Click on a short text (to make it faster) such as Additamentum
*  Click on the TXT download
*  Copy the URL into the Voyant window http://voyant-tools.org/
*  Ok that text is too small to be really interesting by itself, but it gives you the idea

Let's see if we can break the server if we all do this at once:
*  Go to the Voyant homepage http://voyant-tools.org/
*  Enter the URLs for the Confessions, City of God, and De Trinitate
http://mlat.uzh.ch/download_pl/?lang=0&dir=/var/www/Corpus2_PL/&file=031_Augustinus-Hipponensis_Confessiones.xml
http://mlat.uzh.ch/download_pl/?lang=0&dir=/var/www/Corpus2_PL/&file=041_Augustinus-Hipponensis_De-civitate-Dei.xml
http://mlat.uzh.ch/download_pl?lang=0&dir=/var/www/Corpus2_PL/&file=042_Augustinus-Hipponensis_De-Trinitate.xml

_STEP 2_ Explore the visible tools
*  Play with the _Terms_ feature
   * Use the Options to apply the embedded Latin "Stop word" list
   * Check out the terms list -- add RELATIVE frequencies to your list
*  Look at the _TRENDS_ tool in the upper right
   * Find the trends for your OWN words -- try deus and anima for example?
   * Make sure the FREQUENCY option is set to relative not raw frequencies
   * Add a function word like et or in -- what happens to the trend????
*  Look at the _Correlations_ tool (lower right, click on Correlations
   * What correlates with anima? (type "anima" into the box)
   * What happens when you change the "minimum coverage" slider?

_STEP 3_ Check out all the other tools in Voyant.  
The _middle (NOT circled) option_ gives sends you to all the other tools
![tool menu](https://github.com/ctschroeder/tutorials/blob/master/images/Voyant-extra-tools-menu.png)
 
_STEP 4_ Bookmark a corpus or a view within a tool to return to it later
[https://github.com/ctschroeder/tutorials/blob/master/images/voyant-export-tool.png](export function)
* Click Export at the top right of the page
* Select & copy or bookmark the URL for this view to return to your corpus later. (Note, the team at Voyant indicates that the corpus will “accessible as long as it accessed at least once a month.”
* Note, you can also create a URL for JUST that tool (a URL just for the word cloud, for example) by clicking the Export function at the top of the tool; you should see the export icon appear when you hover over the "?" for the tool; it will appear near the options icon for the tool. 

## Distant reading and text analysis with AntConc

