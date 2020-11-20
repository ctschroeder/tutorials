## About this tutorial

In this tutorial, you will learn how to archive Tweets from Twitter on a particular keyword or hashtag using [Martin Hawksey's TAGS tool](https://tags.hawksey.info/).

This tutorial lives online at https://github.com/ctschroeder/tutorials/blob/master/TAGS-tutorial.md

This tutorial is licensed [CC-BY-NC 4.0](https://creativecommons.org/licenses/by-nc/4.0/)

This tutorial was created by Caroline T. Schroeder, PhD, for a course in Cultural Heritage Data Fall 2020 at the University of Oklahoma.

## What you will need

- [Google Drive account](https://drive.google.com/) for Google Sheets, where the Tweets will be archived and where the tool lives

- Good internet connection

- A [Twitter account](https://twitter.com/)

## Preparation

1.  Go to Google Drive and be sure you are logged in to Google Drive on your browser.

2.  Familiarize yourself with TAGS:  Go to https://tags.hawksey.info/ and watch the video

3.  Go to Twitter and login (be sure you know your password)

4.  Set up your TAGS sheet

   - At https://tags.hawksey.info/ click on Get TAGS
   - READ THE PAGE
   - Click on TAGS v6.1

5. You will be asked to copy a document in Google Sheets— click Make a Copy

6. Enter your term(s) in the box that says "Enter Term"

![TAGS](https://github.com/ctschroeder/tutorials/blob/master/images/Tags-screenshot.png)

7. Fill out the rest of the options

   - Period: Select -7 days for your period
   - Follower Count Filter: if your term gets a lot of traffic and you want to weed out spam accounts, you can restrict your archive to only accounts with a certain number of followers. I set mine to 100 but you can do whatever you’d like with it.
Number of Tweets: set the maximum number of tweets you want the tool to archive
   - Type: search/tweets

8. Rename your sheet so it does not say Copy of TAGSv6.1.9.1: click in the box where the title is in the top left and rename

![TAGS document name](https://github.com/ctschroeder/tutorials/blob/master/images/Tags-change-sheet-name.png)

9. In the menu at the top, click on TAGS > Set up Twitter Access
   - Follow the instructions
   - When you get the notice “This app hasn’t been verified” keep going — it’s ok! I’ve used it a million times
   - Click “Advanced”
   - Click on “Go to TAGS v6.1 Client(unsafe)
   - Click “allow” and follow the remaining instructions
   - *Note: When you’re done with the tutorial, you can go back and disconnect TAGS*

![TAGS menu](https://github.com/ctschroeder/tutorials/blob/master/images/Tags-menu.png)

10. Bookmark your spreadsheet for easy reference. (You can also find it in your list of Google docs/sheets in Google Drive later.)

## Run TAGS and collect Tweets

We are going to make a “one off collection” of tweets about a topic from the past week. You can also set it to continuously update every hour. (See the instructions following “Note” in the Instructions block on the TAGS sheet.)
You cannot use TAGS to collect tweets older than a week; Twitter requires you to pay for this! You can continue to collect future tweets using the the Tools menu.
We are going to collect tweets for the past seven days.

11. Under the TAGS menu click “Run now”

## Review and Visualize your Tweet Archive

12. Scroll down the sheet for the Stats section and the Make Interactive section (If you don’t have very many tweets, you can change the follower count filter to 0 and run again or you can add terms and run again)

![TAGS lower-half](https://github.com/ctschroeder/tutorials/blob/master/images/Tags-lower-half.png)

13. To see your tweets, click on the Archive tab at the bottom of the screen

   - **Q: Scroll through your tweets — at a glance, what are they about?**
   - Find the column labeled user_location.
   - Hover your cursor over the letter at the top of the column. You should see a little arrow appear
   
   ![TAGS location](https://github.com/ctschroeder/tutorials/blob/master/images/Tags-tweet-locations-tab.png)
   
   - Click on the arrow
   - Select “Column Stats”
   - **Q: What does that chart say about your tweets? Where are the tweets coming from? Do most of the tweets even have location info? What can you conclude from the location information, if anything?**
   - **Q: Take a screenshot of the chart(s)**
   - **Q: Go back and compare the location info with your quick assessment from scrolling — what else do you learn?**

14. Let’s analyze the content of your tweets
   - Click on the column labeled “text” (in min it’s column C — click on the C and the whole column should be selected)
   
   ![TAGS tweets](https://github.com/ctschroeder/tutorials/blob/master/images/Tags-tweet-archive-tab.png)
   
   - Copy all the text (on my Mac, with the column selected like this, I just click command+c)
   - Go to https://voyant-tools.org/
     - paste the text into the box
     - Click “reveal”
	- The new screen will have a wordcloud of key terms on the left. (The word cloud does not include common words like “is”, “the”, etc.). The most common words are the biggest.

   ![TAGS voyant](https://github.com/ctschroeder/tutorials/blob/master/images/voyant-tags-tweets.png)

   - **Q: what do you learn about the content of the tweets from Voyant?**
   - Note: there’s much more you can do with Voyant - this is just a quick snapshot
   - **Q: Take a screenshot of your word cloud to put in your Lab report**
   - **Q: copy the link in your browser to link to Voyant in your Lab report**
		
15. Let's use TAGS visualizations
  - On your TAGS sheet, click on “Share” in the upper right corner
	- Change the setting to “anyone with link can view”
  - Click on TAGSExplorer to see a network of all the tweeters tweeting on your topic
	
  ![TAGS nodes](https://github.com/ctschroeder/tutorials/blob/master/images/Tags-nodes-only.png)

  - All the dots are nodes; the nodes are the accounts *tweeting* or *mentioned* in tweets
  - Click on “mentions” in the lower right, and you’ll see how people are tweeting with/at each other; the lines between the nodes are edges:  the connections between people tweeting to/with/at each other. The larger the account name, the most connections
  - You can also click on the nodes to see their tweets	
  - You can also click on the menu in the upper left to see top tweeters, top hashtags, etc.
  - **Q: who are the top tweeters on your topic? What can you learn about their interests/location/etc.**
  - **Q: what are the top hashtags in your tweets? Does that tell you anything about what people are interested in regarding your topic?**
  - **Q: copy the link in your browser to put it in your Lab report**. You can see mine at https://hawksey.info/tagsexplorer/?key=1vUsumN9S_xMKyjcyjJeaOe_0OQZ3fOUoyilZlQ0DfbQ&gid=400689247&mentions=true

## Write up your report 

16. Write up your report by responding to the Q’s above, and add anything else of interest to you. Generally: 
	- **Q: what do you learn about how twitter is talking about your topic this week?**
	- **Q: what is *missing* — what don’t you learn? (Consider the language you’re searching in, for example — there may be other things missing)**
	- **Q: is this kind of search useful? Harmful? Both? What else do you think about the implications or consequences of this kind of tweet-harvesting?**
  - Use screenshots and links from the above exercise 
 
17. Post your writeup on your personal website/blog or on the private course blog

18. Put the link to your post in the Canvas assignment.

**When you’re done with the tutorial, you can go back to your spreadsheet and disconnect TAGS from your Twitter account**

Click on the TAGS menu

Select Disconnect Twitter Access




