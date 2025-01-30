# Topic Modeling with the Online Topic Modeling Tool

## About this tutorial

This tutorial was created by Caroline T. Schroeder, licensed [CC-BY-NC 4.0](https://creativecommons.org/licenses/by-nc/4.0/). Last updated 29 Jan 2025.

This tutorial lives live online at https://github.com/ctschroeder/tutorials/blob/master/topicmodeling.md

This tutorial provides a basic introduction to using the [Online Topic Modeling Tool](https://mimno.infosci.cornell.edu/jsLDA/) (created by David Mimno) and some guidance for critically examining one's use of the tool.

## 1. Introduction to the Tool.

The Online Topic Modeling Tool is a web interface for modelling text documents using Latent Dirichlet Allocation. It was developed by David Mimno, one of the original developers of the topic modeling tool Mallet.

The tool is online at https://mimno.infosci.cornell.edu/jsLDA/. Users can conduct basic topic modeling without having to install an app on their computer.

## 2. Topic Modeling the Default Corpus

### First, use the online Topic Modeling tool's default settings to model the default corpus: State of the Union addresses (by US Presidents)
- Navigate to the [tool in your browser](https://mimno.infosci.cornell.edu/jsLDA/).
- Read the instructions on the main page
- Click on "Run a Model"
- The default is 25 Topics. Start with this number of topics
- Click the button to run 50 iterations. (This means it will sort all the words into topics 50 times.)
- Look at the topics (and most frequent words in each topic) on the left
- Click on a topic -- look at how the documents in the middle of your window change. What is it showing?
- Click on the topic correlations tab: notice which topics go together most, and which go together the least?
- Click on the time series tab: which topics are more popular at which times?
  - take screenshots of the timelines -- be sure to note in your notebook and/or on your computer your dataset, # of topics, and iterations
- Click on Downloads: download the Topic Summaries and open the file on your computer
  - Read each topic and give titles to each topic
- Click the button to run 50 iterations again until you get to 200 iterations
- Look at the topics (and most frequent words in each topic) on the left
- Click on Downloads: download the Topic Summaries and open the file on your computer
  - Read each topic and give titles to each topic
  - Compare to your earlier download: are they the same topics? different? does one look "better" or "more refined"?
  - take notes in your notebook
- Check out the time series tab and topic correlations tab. Take screenshots of what interests you.
- Compare your topics to your neighbors -- are they the same? different? similar?

### Next try changing the settings
- Being sure you've screenshotted and downloaded everything you want, change the slider on the upper right to more or fewer topics
go through some of the steps above for this new experiment
- How are the topics different or similar? Are they "better" or "worse"? Why?
- Download the Topic Summaries and give the topics titles
- Compare to your previous results
- Which topics are the highest percentage of your corpus?
- What do the time series look like -- which topics appear throughout the corpus, and which appear in certain periods?

## 3. Writing Up Your Results

Use the questions above to think about what topic modeling has taught you about your corpus. 

Be sure to document the number of topics and the number of iterations you used.

Are there any problems with your results? Anything that concerns you?

## 4. Using the Online Tool to Model Your Own Corpus

If you decide you want to use this tool for another corpus (say, for your final project), you can. You just need to format your textual data in the correct format.

Go back to the [tool homepage](https://mimno.infosci.cornell.edu/jsLDA/).
- Read the instructions about "Using your own documents"
  - Note what Mimno says about the ideal size of a "document" (a few hundred words); you may need to segment your corpus into smaller units if your documents are larger than that
- Click on the button to "Get the Source"
  - Click on "documents.txt"
  - On the right you'll see an icon with a downward arrow -- click that to download the text file
  - Open it on your computer
  - Notice that the file is basically a series of rows of data that are tab-delimited. Each row has numbers like "1914-1" followed by a tab and then that same year, like "1914", followed by a tab, followed by a string of a couple of hundred words of text.
  - Each State of the Union address has been divided into smaller segments. The first number on the line is the year of the address (such as 1914) followed by the segment of the document (so 1914-1 = the first segment of the 1914 State of the Union).
  - You will need to use the same format for your corpus.
  - I recommend setting it up in a spreadsheet: the first column will be the date stamp, the second column will be the segment sequence, and the third will be the text. You will need to save it as a tab-delimited text file with the ".txt" extension on the filename
 
The homepage provides instructions for setting up your own stop word list. You also can use [Mimno's stop word list](https://github.com/mimno/jsLDA/blob/master/stoplist.txt) if your corpus is in English.


  
