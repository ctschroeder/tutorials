# Voyant Tools for Text Analysis: Tutorial

## Description of the tool
Voyant is ["a web-based reading and analysis environment for digital texts."](http://voyant-tools.org/)
You can use Voyant:
1. [online on the website](http://voyant-tools.org/)
2. on your own computer by [downloading and installing the application](http://docs.voyant-tools.org/resources/run-your-own/voyant-server/)

This tutorial assumes you will be using the online version.  Downloading and installing is not difficult.  The advantages: your files stay confidential (not on the web, on someone else's server), and you don't need to have internet access to use the tool. **If you don't have highspeed internet access at home, you may wish to download and install while on campus.**

There is A TON of documentation on the Voyant Page. [GO CHECK OUT THEIR DOCUMENTATION](http://voyant-tools.org/docs/#!/guide) when you are done with this tutorial to see other cool stuff.

## Laptop/desktop vs mobile device
Full functionality requires a laptop or desktop.

You should be able to upload a corpus using methods 1 or 2 described below.  I do not know how well the tols (and especially selecting the options for the tools) work with a tablet. (If you have only a phone, your screen will be too small.)  I do not know if you can save or download image files on a tablet.

## Uploading a Corpus
A "corpus" is a collection of texts. Usually the corpus has been created using some guiding principle (same author, same genre, same time period, etc.)
There are three main ways of selecting a corpus in Voyant Tools:
1. type or paste into the main text area, either normal text or a set URLs, one per line; then hit the "Reveal" button
2. open an existing model corpus the Voyant folks have already included online (such as Austen or Shakespeare) 
3. upload one or more files from your computer

This tutorial uses process #1 & #3.  (So we will use TWO different corpora.)  Try out #2 on your own another time!

### Step 1:
* Download [a test corpus on to your computer](https://minhaskamal.github.io/DownGit/#/home?url=https://github.com/ctschroeder/tutorials/tree/master/teaching-corpora/apocryphal-acts/texts)
* Remember where you put it or the file name so you can find it again.

### Step 2: Upload your corpus to Voyant via one of the following methods
* Navigate to http://voyant-tools.org/
* Do ONE of the following:
  1. EITHER copy and paste the following URL into the window: http://disc.library.emory.edu/lincoln/download/lincoln_sermons.zip
  2. OR Click on "Upload"
      - Navigate to the place in your computer with the test corpus download.
      - Double-click on the file (it should end in a .zip) to upload it to Voyant
* Click Reveal

## Understanding the page

Once opened, in what they call the “default skin”- you will see five panels. Each of these is a tool, Cirrus, Reader, Trends, Summary, and Contexts. These tools interact with one another – if you modify one pane, you’ll see another update.
The appearance of each of these windows can be modified. Place the cursor on the ? symbol over any given tool, and a menu of options will appear. (Note: hover over the titles of these navigation buttons for descriptions.)
![Voyant Overview](https://github.com/ctschroeder/tutorials/blob/master/images/Voyant-overview-hover.png)

You may need to expand the window of your tool to be able to see the full menu.
![window](https://github.com/ctschroeder/tutorials/blob/master/images/Voyant-overview-moved-window.png)

The first icon allows you to create a web URL so you can come back to your corpus and this tool.
The second icon allows you to switch to a new tool.
The third icon allows you to define options for the tool. (circled)
![tool menu](https://github.com/ctschroeder/tutorials/blob/master/images/Voyant-extra-tools-menu.png)

## Tools:
*Cirrus*

A word cloud that visualizes the top frequency words of a corpus or document.
Central location and large size indicate greater frequency.

### Step 3: Play with the Cirrus/Word Cloud tool
* What is the word cloud telling you about your corpus?
* Hover over the words; the number = the number of times the word appears in the corpus
* What happens when you slide the slider next to "Terms"?
* When you click on Scale, you can choose to create a word cloud of your whole corpus or individual documents

### Step 4: Adjust the options on the Cirrus/Word Cloud tool
* Click on Options
[options](https://github.com/ctschroeder/tutorials/blob/master/images/Voyant-extra-tools-menu-2.png)
* What happens to your word cloud if you change "stop words" to "none" and click confirm?
_**Stop words are some of the most common function words and pronouns (the, a, an, she...)**_
* Turn the stop words back on.
* Try adjusting some of the other options listed below. (In class if you have time or at home.)

Here are the other options:

*White List*: you can define a set of allowed words (the opposite of a stopwords list), only terms in this list will be shown in Cirrus (note that the stopwords list is still active, so you may want to choose "None" from the stopwords menu to deactivate it)

*Max Terms*: you can specify the maximum number of terms to be fetched as data from the server (though the Terms slider described above determines how many of these terms are visible at once); note that setting this too high may slow things down considerably

*Font Family*: you can determine which font is used by Cirrus, a set of web safe fonts is provided, as well as Lato; you can also specify a font installed on your computer, but of course it may not be available on other computers (in which case a default font is used)

*Palette*: you can edit the colour palette

### Step 5: Click on "Terms" above the word cloud
This gives you a list of the terms in your corpus (except stop words, if they're turned on).
The count tells you the number of times each term appears in the corpus.
* Hover over "Count"
* Click on the little down chevron next to Count to get a drop down menu
* Hover on Columns
* Select "Relative" and unselect "Count"
* Now your chart of Terms shows the relative frequency of each term.  The number isn't the raw count; it's now the number of times per million words each term appears.  It is more accurate to compare relative frequency than raw frequency.
* Click on Links. Now you'll see a network of terms that appear near each other.  [More information here](http://voyant-tools.org/docs/#!/guide/collocatesgraph)

### Step 6: Check the time.
* If we are almost out of time, skip down to Step 8 to bookmark your corpus and do Steps 8-11.  You can finish Steps 7 & 12 at home on your own.

### Step 7: Play around with the other tools (listed below)
* Search for terms in "Trends".  What terms trend together? 
*Reader*

Text Reader- displays text for reading.

*Terms Berry* within the Reader

Visualizes the frequent words: the more frequent, the larger the berry.  Hover on the berries -- what happens? What does it mean?

*Summary*

Provides information about the corpus.

*Contexts*

shows each occurrence of a keyword with surrounding text.

*Correlations* within the Contexts Tool

Correlations tool shows the extent to which two terms are freqent together or not together. Correlation of 1 means they are always appearing together.  Correlation of -1 means they don't appear together.
[Check out the documentation for more details](http://voyant-tools.org/docs/#!/guide/correlations)

*Trends*

A line graph that depicts the distribution of a word or words (occurrence across a corpus or document).

Additional tools can be added using the Choose Another Tool button described above.


### Step 8: Bookmark a corpus or a view within a tool to return to it later
[https://github.com/ctschroeder/tutorials/blob/master/images/voyant-export-tool.png](export function)

* Click Export at the top right of the page
* Select & copy or bookmark the URL for this view to return to your corpus later. (Note, the team at Voyant indicates that the corpus will “accessible as long as it accessed at least once a month.”
* Note, you can also create a URL for JUST that tool (a URL just for the word cloud, for example) by clicking the Export function at the top of the tool; you should see the export icon appear when you hover over the "?" for the tool; it will appear near the options icon for the tool. 

### Step 9:  Download an file of your visualization from a tool

* Hover over the "?" for the tool/visualization you want to download.
* Click on the export button (the square with an arrow)
* Click on "Export visualization"
* Select a PNG file. (SVG is higher quality but sometimes our blog software won't allow you to use SVG files.)
* Follow instructions on screen to save (right-click or ctrl-click, save image as..., navigate to place on your computer where you want to save)
* Be sure to give your file a **meaningful filename** before you save.
* Be sure to make note of what this visualization visualizes (what is the corpus, using stop words or not
, etc.)

### Step 10: Embed a corpus or tool visualization in a blog post or website
Sometimes you might want a LIVE version of your visualization, so people can click around or hover over the visualization to reveal more information. 

* Click Export at the top of the page. 
* Select “an HTML snippet”
* Click export for the snippet to appear
* Select and copy the snippet. (command-a to select all, command-c to copy)
* For HTML pages: cut and paste into your HTML page. (If you don't know what this is, don't worry -- you don't need to)
* For a blog post: start a new blog post on your Wordpress blog
* Click on the Text tab (**This is very important**. The code won't work if you are in the Visual tab.)
* Paste the snippet into your post. (command-v to paste)
* Adjust the height or width if you'd like by changing the 800px (=800 pixels) height to another number or the 100% width to another percentage of your screen

### Step 11: Document your visualization and corpus

* In your blog post, website, or separate text/wordprocessor file where you are keeping your notes: document what your corpus is and where you got it from
* You should also document the tool if you are including visualizations/information based on the tool.  
* First we will document Voyant Tools. Click on the Export button for the tool.
  * Click on Export View
  * Select Bibliographic reference and click Export
  * Copy the reference in whichever format you prefer.
  * Paste it into your blog post/webpage/notes page.  For blog posts/webpages, check the formatting
* Best practices are also to link to your corpus/tool online if it is online.  (You can't do this if you downloaded the Voyant app and are using it offline.)
  * Click on the Export button at the very top right of your screen (in the blue bar)
  * Click Export
  * A new window will appear.  Copy everything in the web URL up to and including the "&" symbol.
    * So, for http://voyant-tools.org/?corpus=c36aca9ef64535300b59062b8832c87f&panels=cirrus,reader,trends,summary,contexts you would copy http://voyant-tools.org/?corpus=c36aca9ef64535300b59062b8832c87f&
    * You can also copy the whole URL. It's not a big deal either way; copy the whole thing if you are confused.
  * Put this link in your webpage/blog post/notes as documentation
  
### Step 12: Try it with another corpus
* Go back up to Step 2.  If you used the Lincoln sermons for this tutorial, then do the tutorial again using our test corpus. If you used the test corpus, try it with the Lincoln sermons.
* Is there a corpus of literature you are interested in? 
  * How could you use Voyant to study your corpus?
  * What would you need to do to make it ready to import into Voyant?
  

## Credits
This tutorial has been adapted from prior work by me, the Voyant Tools documentation, ["Doing Digital History"](http://history2016.doingdh.org/voyant-tutorial/), and [Kate Farley](http://katefarley.org/voyant/)
