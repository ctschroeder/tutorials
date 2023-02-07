# Corpus Analysis with AntConc

Last modified 7 February 2023

This tutorial lives online at https://github.com/ctschroeder/tutorials/edit/master/antconc-programming-historian.md.

This is a modification of the original [Programming Historian Corpus Analysis with AntConc Tutorial](https://programminghistorian.org/lessons/corpus-analysis-with-antconc).  The images from the original PH tutorial have been deleted or replaced by screenshots of a more recent AntConc version; it provides a more detailed explainer of Target and Reference Corpora, with tips for using them in the Keyword Tool.

---
title: Corpus Analysis with Antconc
layout: lesson
date: 2015-06-19
authors:
- Heather Froehlich

reviewers:

- Nabeel Siddiqui

- Rob Sieczkiewicz

editors:
- Fred Gibbs

difficulty: 1

activity: analyzing

topics: distant-reading

abstract: "Corpus analysis is a form of text analysis which allows you to make comparisons between textual objects at a large scale (so-called 'distant reading')."

---

## Introduction
Corpus analysis is a form of text analysis which allows you to make comparisons between textual objects at a large scale (so-called 'distant reading'). It allows us to see things that we don't necessarily see when reading as humans.  If you’ve got a collection of documents, you may want to find patterns of grammatical use, or frequently recurring phrases in your corpus. You also may want to find statistically likely and/or unlikely phrases for a particular author or kind of text, particular kinds of grammatical structures or a lot of examples of a particular concept across a large number of documents in context. Corpus analysis is especially useful for testing intuitions about texts and/or triangulating results from other digital methods.

By the end of this tutorial, you will be able to: 

* create/download a corpus of texts
* conduct a keyword-in-context search
* identify patterns surrounding a particular word
* use more specific search queries
* look at statistically significant differences between corpora
* make multi-modal comparisons using corpus lingiustic methods

You have done this sort of thing before, if you have ever...

* searched in a PDF or a word doc for all examples a specific term
* Used [Voyant Tools][48] for looking at patterns in one text
* Followed [Programming Historian][51]’s Introduction to Python tutorials

In many ways [Voyant](http://voyant-tools.org/) is a gateway into conducting more sophisticated, replicable analysis, as the DIY aesthetic of Python or R scripting may not appeal to everyone. [AntConc](http://www.laurenceanthony.net/software/antconc/) fills this void by being a standalone software package for linguistic analysis of texts, freely available for Windows, Mac OS, and Linux and is highly maintained by its creator, [Laurence Anthony](http://www.laurenceanthony.net/). There are other concordance software packages available, but it is freely available across platforms and very well maintained. See the [concordance bibliography][56] for other resources.

This tutorial explores several different ways to approach a corpus of texts. It's important to note that corpus linguistic approaches are rarely, if ever, a one-size-fits all affair. So, as you go through each step, it's worth thinking about what you're doing and how it can help you answer a specific question with your data. Although I present this tutorial in a building-block approach of 'do this then that to achieve x', it's not always necessary to follow the exact order outlined here. This lessons provides an outline of some of the methods available, rather than a recipe for success.

### Tutorial downloads
1. Software:[AntConc](http://www.laurenceanthony.net/software/antconc/).    
Unzip the download if necessary, and launch the application. Screen shots below may vary slightly from the version you have (and by operationg system, of course), but the procedures are more or less the same across platforms and recent versions of AntConc. 

2. Sample Corpus: Download the [zip file of movie reviews](https://programminghistorian.org/assets/corpus-analysis-with-antconc/antconc_corpus_files.zip).

### A broad outline of this tutorial:
1. Working with plain text files
2. The AntConc user interface, loading corpora
3. Keyword-in-context searching
4. Advanced keyword-in-context searching
5. Collocates and word lists
6. Comparing corpora
7. Discussion: Making meaningful comparisons
8. Further resources


## 1. Working with Plain Text Files
* Antconc works only with plain-text files with the file appendix .txt (eg Hamlet.txt).  
* Antconc **will not** read .doc, .docx, .pdf, files. You will need to convert these into .txt files.  
* It will read XML files that are saved as .txt files (it's OK if you don't know what an XML file is).  

Visit your favorite website for news, and navigate to a news article (doesn't matter which one, as long as it is primarily text). Highlight all text in the article (header, byline, etc), and right-click "copy". 

Open a text editor such as Notepad (on Windows) or TextEdit (on Mac) and paste in your text.

Other free options for text editors include [Notepad++][53] (Windows) or [TextWrangler][54] (Mac), which offer more advanced features, and are especially good for doing a lot of text clean-up. By text clean-up, I mean removing extratextual information such as "boilerplate", which appears regularly throughout. If you keep this information, it's going to throw your data off; text analysis software will address these words in word counts, statistical analyses, and lexical relationships. For example, you might want to remove standard headers and footers which will appear on every page. Please see [“Cleaning Data with OpenRefine"](/lessons/cleaning-data-with-openrefine) for more on how to automate this task. On smaller corpora it may be more feasible to do this yourself, plus you'll get a much better sense of your corpus this way.

Save the article as a .txt file to the desktop. You may want to do some follow-up text cleanup on other information, such as author by-line or title (remove them, then save the file again.) Remember that anything you leave in the text file can and will be addressed by text analysis software.

Go to your desktop and check to see you can find your text file. 

Repeating this a lot is how you would build a corpus of plain text files; this process is called _corpus construction_, which very often involves addressing questions of sampling, representativeness and organization. Remember, *each file you want to use in your corpus _must_ be a plain text file for Antconc to use it.* It is customary to name files with the .txt suffix so that you know what kind of file it is. 

As you might imagine, it can be rather tedious to build up a substantial corpus one file at a time, especially if you intend to process a large set of documents. It is very common, therefore, to use webscraping (using a small program to automatically grab files from the web for you) to construct your corpus. To learn more about the concepts and techniques for webscraping, see the _Programming Historian_ tutorials [scraping with Beautiful Soup][50] and [automatic downloading with wget][51]. 
Rather than build a corpus one document at a time, we're going to use a prepared corpus of positive and negative movie reviews, borrowed from the [Natural Language Processing Toolkit](http://www.nltk.org/). The NLTK movie review corpus has 2000 reviews, organized by positive and negative outcomes; today we will be addressing a small subset of them (200 positive, 200 negative).

Corpus construction is a subfield in its own right. Please see [Representativeness in Corpus Design](http://llc.oxfordjournals.org/content/8/4/243.abstract)," _Literary and Linguistic Computing_, 8 (4): 243-257
and [_Developing Linguistic Corpora: a Guide to Good Practice_](http://www.amazon.com/Developing-Linguistic-Corpora-Practice-Guides/dp/1842172050/ref=sr_1_1) for more information. 


## 2. Getting Started with AntConc: The AntConc user interface, loading corpora

When AntConc launches, you will see a **window** with a few sections and a **menu bar** at the top of the screen.

On the left-hand side, there is a window to see all corpus files loaded (which we'll use momentarily).

There are 9 tabs across the top:

**KWIC:** This will show you what's known as a Keyword in Context view (abbreviated KWIC, more on this in a minute), using the search bar below it; this is the classic Concordance feature.  

**Plot:** This will show you a very simple visualization of your KWIC search, where each instance will be represented as a little black line from beginning to end of each file containing the search term.  

**File View:** This will show you a full file view for larger context of a result.  

**Cluster:** This view shows you words which very frequently appear together. 

**N-Gram:** This shows frequency of words that appear right next to each other. N-gram size 3 shows all the combinations of three words in a row and how frequently those three words appear in a row in the corpus. N-gram size 4 shows four word combinations, etc.

**Collocate:** Clusters show us words which _definitely_ appear near each other in a corpus; collocates show words which are statistically likely to appear together.  

**Word:** A list of all the words in your corpus.  

**Keyword:** This will show comparisons between two corpora.

**Wordcloud:** This is a new feature only in the recent versions.

As an introduction, this tutortial barely scratches the surface of what you can do with AntConc. We will focus on the KWIC, Collocate, Keywords, and Word List functions. 

### Loading Corpora
AntConc's recent version has pre-built corpora embedded in it. You can experiment with those later. Today we will use our own corpus of film reviews.

Start with the menu bar's File&nbsp; &gt; > Corpus Manager. (For this activity, you can also select the Quick Corpus option in the File menu, but I want you to see the full Corpus Manager screen.) Be sure you're in the "Target Corpus" Tab. (Tabs are on the right side pane of the Corpus Manager.)

AntConc allows you to open entire directories, so:

- Under Corpus Source on the left select "Raw files"
- On the right select Add Directory to add a directory or folder of files. (You don't want to add 100 files one by one.)
- In the dropdown menu a**navigate to our folder "Corpus Files for AntConc Workshop":**
- Keep opening the folders until you get to the **Positive Reviews** folder -- load that directory
- You should see a list of files appear in the window in the upper right and the number of files should read 200
- Do the same thing to add the **Negative Reviews** folder
- You should see the nuber of files jump to 400
- Give your corpus a descriptive name (mine is ph-movie-reviews)
- Keep the other options the same. 
- Don't worry about the metadata table -- that is an advanced option we're not using right now
- **Click Create at the bottom of the screen**
- In the right pane, you should see a bunch of info about your corpus appear
- Click **Return to Main Window**
- You should see all the files from your corpus on the left pane

## 3. Searching Keywords in Context 

Note: for any query below or change to order or Sort be sure to click **Start** after you make a change in the other settings or query.

### Start with a basic search
One of the things corpus tools like Antconc are very good at are finding patterns in language which we have a hard time identifying as readers. Small boring words like *the, I, he, she, a, an, is, have, will* are especially difficult to keep track of as readers, because they're so common, but computers happen to be very good at them. These words are called function words, though they commonly known as 'stopwords' in digital humanities; they are often very distinct measures of authorial and generic style. As a result, they can be quite powerful search terms on their own or when combined with more content-driven terms, helping the researcher identify patterns they may not have been aware of previously. 

**In the search box at the bottom, type the word the and click "start".** The KWIC view (CONCORDANCE in the images) will show you every time the word the appears in our corpus of movie reviews, and some context for it. This is called a "Key Words in Context" viewer. 

(14618 times, according to the Hits box on the top right.)

![KWIC or Concordance Tool](https://github.com/ctschroeder/tutorials/blob/master/images/01-concordance.png)

As above, the KWIC list is a good way to start looking for patterns. Even though it's still a lot of information, what kinds of words appear near "the"? 

Try a similar search for "a". Both "a" and "the" are articles, but one is a definite article and one an indefinite article - and the results you get will be illustrative of that.

Now that you're comfortable with looking at a KWIC line, try doing it again with "shot": this will produce examples of both shot the noun ('line up the **shot**') and the verb 'this scene was **shot** carefully')

What do you see? I understand this can be a difficult to read way of identifiying patterns. 

Try changing the option in the lower right from Order by freq to Order by value and click the Start box -- what happens?

You can adjust the way AntConc sorts information by changing the parameters at the bottom of the panel labeled "Sort 1", "Sort 2", "Sort 3" (see image below): 
- L corresponds with 'left' and R corresponds with 'right'; you can extend these up to ±5 in either direction. 
- The default is 1 right, 2 right, 3 right, but you can change that to search 3 left, 2 left, 1 right (to get phrases and/or trigrams that end in the search term in question, for example). 
- If you don't want to include a sorting option you can select C. 
- Less linear sorting practices are available, such as 4 left, 3 right, 5 right, which includes a lot of other contextual information. 
These parameters can be slow to respond, but be patient. 

![Sorting in Concordance tool](https://github.com/ctschroeder/tutorials/blob/master/images/02-sort.png)

## 4. Advanced KWIC: Search Operators

### The * operator (wildcard) 
The * operator (which finds zero or more characters) can help, for instance, find both the singular and the plural forms of nouns.

**Search for qualit*, then sort this search.** What tends to precede and follow quality &amp; qualities? (Hint: they're different words, and have different contexts. Again- look for patterns in usage using the KWIC!)

For a full list of available wildcard operators and what they mean, go to Global Settings &gt; Search.  

To find out the difference between d* and ?, search for th*n and th?n. These two search queries look very similiar, but show very different results. 

The ? operator is more specific than the * operator:  
wom?n – both women and woman  
m?n – man and men, but also min  
contrast to m*n: not helpful, because you'll get mean, melon, etc.

**Compare these two searches: wom?n and m?n**
1. sort each search in a meaningful way (eg. by search term then 1L then 2L)  
2. File &gt; Save Current Tab Results to a text file (&amp; append with .txt )

>HINT: During the course of exploring in your research, you may generate many such files for reference; it's helpful to use descriptive filenames that describe what's in them (such as "wom?n-KWIC-results.text", not "antconc_results.txt").

![Saving results](https://github.com/ctschroeder/tutorials/blob/master/images/05-saveresults.png)

And now you can open the plain text file in your text editor; you might have to widen the application window to make it readable.

Do this for each of the two searches and then look at the two text files side by side. What do you notice?

### The || operator ("or")

The operator || (two vertical lines) is the equivalent of "or" and lets you search for multiple terms.

**Search on she||he.**. 

**Now search for she and he separately:** how many instances of she vs he?  There are many fewer instances of she – why? That's a research question! A good follow-up questions might be to sort the she|he search for patterns, and look to see if particular verbs follow each. 

**Practice searching a word of your choice, sorting in different ways, using wildcard(s), and finally exporting.** Guiding focus question here: what kinds of patterns do you see? Can you explain them?

## 5. Collocates and word lists
Having looked at the KWIC lines for patterns, don't you wish there was a way for the computer to give you a list of words which appear most frequently in company with your keyword?

Good news - there is a way to get this information, and it's available from the Collocates tab. Click that. Sometimes (if Collocates are the first thing you do in AntConc) AntConc will tell you it needs to create a word list. Hit OK; it will do it automatically.  

Try generating collocates for she.

The Default settings in AntConc only show the most statistically significant collocates. If you want to see _all collocates_ you need to adjust the settings:
- In the upper left menu click on Settings then Tool Settings then Collocate
- Under the Likelihood Measure option you will see Threshold
- Set to "All Values"
- Click Apply
- Close the window
- In your Collocates Pane click Start to rerun your query.
- Notice the differences in the two lists

The two images below show the Collocates list with the two different settings. What do you notice about the lists?

![Collocates for "wom?n": Threshold of All Values](https://github.com/ctschroeder/tutorials/blob/master/images/06-collocate.png)

![Collocates for "wom?n": Default settings](https://github.com/ctschroeder/tutorials/blob/master/images/06b-collocate.png)

**Dr. S note:** depending on the version or whether you're using Mac or PC, the results may or may not be sorted.  Read through the next four paragraphs in full before playing around with the "sort" feature. The "sort" menu is on the bottom of the panel; you will see a menu you can toggle to "sort by freq", "sort by stat", etc.

The unsorted results will seem to start with function words (words that build phrases) then go down to content words (words that build meaning)– these small boring words are [the most frequent words in English][55], which are largely phrase builders. Some versions of AntConc often include the search term as the first hit, presumably because the search term you are looking for shows up in the text and we are looking for words which are likely to appear with this word. 

Some people might want to remove these small words by using a stopword list; this is a common step in topic modelling.  Personally I don't encourage this practice because addressing highly-frequent words is where computers shine! As readers we tend not to notice them very much. Computers, especially software like Antconc, can show us where these words do and do not appear and that can be quite interesting, especially in very large collections of text - as explored earlier in the tutorial, with *the*, *a*, *she* and *he*.

Additionally you may have a single letter 's' appear, quite high as well - that represents the possessive *'s* (the apostrophe won't be counted), but AntConc considers that s indicative of another word. Another example of this is *'t* appearing with *do*, as they contract as *don't*. Because these so commonly appear together, this makes them highly likely collocates. 

**Dr. S note:** "Likelihood" is the likelihood these words appear together:  the higher the number, the more connected those two words are.  The formula takes into account how often they appear together.  The words with the highest "Likelihood" number always or almost always appear with your search term, and less frequently appear anywhere else in the corpus.

What happens if you change the "Minimum Freq" to a higher number?  Try changing it to "3" and click "Start."  Now your list of collocations only includes words that appear at least 3 times in the corpus.*

**Task:** 
Generate collocates for m?n and wom?n. Now sort them by frequency to 1L.  
This tells us about what makes a man or woman 'movie-worthy':  
– what words are associated with women?  
– what words are associated with men? 
– can you draw any conclusions?

This is not necessarily telling us about the movies but about the way those movies are written about in reviews, and can lead us to ask more nuanced questions, like "How are women in romantic comedies described in reviews written by men compared to those written by women?"

**Dr. S note:** the results will vary depending on the parameters of your query:  sort, minimum collocation frequency, 1L/1R vs 2L/2R vs 3L/3R etc. and whether you changed the default Settings as described above.

## 6. Comparing corpora
One of the most powerful types of analysis is comparing your corpus to a larger reference corpus.

I've pulled out reviews of movies with which Steven Spielberg is associated (as director or producer). We can compare them to a reference corpus of movies by a range of directors.

Be sure to think carefully about what a reference corpus for your own research might look like (eg. a study of Agatha Christie's language in her later years would work nicely as an analysis corpus for comparison to a reference corpus of all her novels). Remember, again, that corpus construction is a subfield in its own right.

**Dr. S Note:**

- The TARGET corpus is the corpus you are analyzing 

- You want the REFERENCE corpus to be the corpus for comparison

- So for this activity -- analyzing the Spielberg reviews -- you want Spielberg to be TARGET and the larger 400-review corpus to be REFERENCE. 

**PRO TIP from Dr. S:** if you get confused with your corpora and need to restart, clear everything in AntConc out with File > Clear All Tools and Files.  Then Load your TARGET corpus first ; load the REFERENCE corpus using the corpus manager.
* In fact, let's do this:  Clear All Tools and Files.  (You should see no files in that left pane.)
* Now using the File > Corpus Manager command in the menu bar, open the corpus manager
* clear your corpus here again
* load Spielberg reviews in the main Antconc window.  You should see 24 files. **Give it a new name!!** and click CREATE
* Click the REFERENCE corpus tab on the RIGHT pane
* On the LEFT pane click the Corpus Database button (you're going to choose a corpus you used before and that AntConc saved.)
  * You should see your larger movie reviews corpus if you haven't restarted AntConc-- **select it by clicking on it.** Then **click Choose** 
  * If you don't see it in the list of databases you load the files again. Click on Raw File(s). Be sure you're in the REFERENCE tab, clear the corpus, load your reference corpus directory, give it a name, hit Create)
* Click on both Reference and Target tabs to be sure you have the right corpus in each one.
* Click Return to the Main Window 

Note: You can also opt to swap reference corpus &amp; main files in the Files menu (File > Swap Target/Reference Corpora). 

In Keyword TAB, just hit Start (with nothing typed in the search box).   

We see a list of Keywords that have words that are much more frequent in the Target corpus than in the Reference corpus.  These words are *characteristic* words for the Target corpus compared to the Reference corpus. 

&gt; Keyness: this is the frequency of a word in the text when compared with its frequency in a reference corpus,  For those interested in the statistical details, see the section on keyness on Laurence Anthony's [readme file](http://www.laurenceanthony.net/software/antconc/releases/AntConc335/help.pdf). 

What are our keywords?

(This section heavily modified by Dr. S)

## 7. Discussion: Making meaningful comparisons
Keep in mind that the way your organize your text files makes a difference to the kinds of questions you can ask and the kinds of results you will get.  You could, for instance, make other comparisons with different subsets of reviews, which yield very different kinds of questions. 

Of course, the files you put in your corpus will shape your results. Again, the question of representativeness and sampling are highly relevant here – it's not always necessary or even ideal to use *all* of a dataset at once, even if you do have it. At this juncture, it's really worth interrogating how these methods help produce research questions. 

When thinking about how movie reviews work as a genre, you could consider, for example... 

* Movie reviews vs music reviews
* Movie reviews vs book reviews
* Movie reviews vs news articles about sport
* Movie reviews vs news articles in general

Each of these comparisons will tell you something different, and can produce different research questions, such as:

* How are movie reviews different than other kinds of media reviews?
* How are movie reviews different than other kinds of published writing?
* How do movie reviews compare to other specific kinds of writing, such as sport writing?
* How do movie reviews have in common with music reviews?

And of course you could flip those questions to make further research questions:

* How are book reviews different to movie reviews?
* How are music reviews different than movie reviews?
* What do published newspaper articles have in common?
* How are movie reviews similar to other kinds of published writing?

In summary: it's worth thinking about:

* Why you might want to compare two corpora
* What kinds of queries make meaningful research questions
* Principles of corpora construction: sampling &amp; ensuring you can get something representative

## 8. Check out the N-Gram tool (it's pretty self-explanatory)

## 9. Try a different corpus!!

-----

## 9. Further resources for this tutorial
[A short bibliography on corpus linguistics][43].    
[A more step-by-step version of this tutorial, assuming no computer knowledge](http://hfroehli.ch/workshops/getting-started-with-antconc/)


[41]: http://www.lexically.net/downloads/version6/HTML/index.html?keyness_definition.htm
[43]: http://hfroehlich.wordpress.com/2014/05/11/intro-bibliography-corpus-linguistics/
[47]: http://hfroehli.ch/workshops/getting-started-with-antconc/
[48]: http://voyant-tools.org/
[50]: http://programminghistorian.org/lessons/intro-to-beautiful-soup
[51]: http://programminghistorian.org/lessons/automated-downloading-with-wget
[52]: http://www.antlab.sci.waseda.ac.jp/
[53]: http://notepad-plus-plus.org/
[54]: http://www.barebones.com/products/textwrangler/
[55]: http://www.wordfrequency.info/free.asp
[56]: http://hfroehli.ch/2014/05/11/intro-bibliography-corpus-linguistics/

## Dr. S in class instructions streamlined ##
1-2. Load the movie review corpus (All Reviews)

3-4. Search for a term

- use the KWIC tool to find more information about the use of the term

- sort

- change the parameters of "KWIC sort" at the bottom & sort

- Use wild card characters such as * and ? in your search

- Save output as text file(s) with meaningful title

- discuss what you learned from your searches with your neighbor

5. Use the Collocate tool to search for words most associated with your search term.

- Adjust the Window Span and Minimum Collocate Frequency options; how does that change the results?  What do those changes mean? (REREAD what Dr. Froehlich says about MEANING at the end of the [Collocates and Word Lists](https://programminghistorian.org/lessons/corpus-analysis-with-antconc#collocates-and-word-lists).)

- Use wild cards like m?n and wom?n to find collocations

- Find collocations for your own terms

- Save output as text file(s) with meaningful title

6. Use the Keywords tool to compare corpora

- Read the instructions to find words that are more associated with Spielberg reviews than other reviews

- Remember:  TARGET is the corpus you're analyzing; REFERENCE is the comparison corpus

7. Make meaningful analyses and comparisons from your results

8. Play around with the N-Gram tool

9. Try a different corpus! (for Keywords: what's your Target, what's your Reference? why?)

**PRO TIPS from Dr. S**

**1. If you get confused, or you load your files incorrectly:  You can always reset by going to the File menu and selecting "Clear Tool", "Clear All Tools" or "Clear All Tools and Files."  "Clear All Tools and Files" will wipe your tool clean.**

**2. Click File > Save Current Tab results to save your results before doing another query.**

