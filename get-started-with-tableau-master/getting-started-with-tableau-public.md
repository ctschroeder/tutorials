# Getting started with Tableau Public

## About this Tutorial: Dr. S

This tutorial is a modification of Dr. Miriam Posner's "Getting Started with Tableau" tutorial. Last modified 3/7/2021. It lives live at https://github.com/ctschroeder/tutorials/blob/master/get-started-with-tableau-master/getting-started-with-tableau-public.md.

## About this Tutorial: Dr. Posner

Tableau is a powerful data visualization tool, in heavy use among both laypeople and data professionals.

Tableau Public is the free version of this tool. There are several things to be aware of with regard to Tableau Public. It's free to download and use, but, aside from screenshots, the only way to share Tableau Public visualizations is to publish them to the Tableau Public website. That means they will be freely available on the web, and you will need to create a Tableau account in order to do this.

However, you do not need to create an account in order to use Tableau Public. We will use it today to make two charts, which we'll combine into a dashboard. [Here is a preview of what we'll make.](https://public.tableau.com/profile/miriam.posner#!/vizhome/IowaArtsGrants2015/Dashboard1?publish=yes) At the end of this tutorial, you'll find information on how to publish it to the web. For this exercise, you will need the [Iowa Arts Council Grants data CSV file](https://www.dropbox.com/s/lhanmm3v9ylccgz/Iowa_Arts_Council_Grants.csv?dl=0).

## Tableau Public Application and Tableau Public Workspace Online

You can use Tableau Public by downloading to your computer from https://public.tableau.com. Select Create and then Download. Then you can work offline without worrying about your internet connection.

You also can go to https://public.tableau.com and select Create > Web Authoring to upload your data directly to Tableau online and work in their online environment. This is good for people who a) have a secure internet connection and b) don't have a laptop/desktop or don't have permission to install software on their laptop/desktop.

## 1. Choose your data source

### 1a. Getting your data

After opening Tableau, you're presented with a list of file types you can choose to work with ("connect"). Even though our Iowa Arts Council Grants file *opens* in Excel, it's saved as a CSV. To Tableau, a CSV is a text file. So select **Text file.** Then navigate to the file you downloaded earlier and double-click to open it.

![][1]

[1]: images/getting-started-with-tableau-public/choose-your-data-source.png

### 1b. Understanding your data

Look at your data!  It should look like a spreadsheet.  What is this dataset? What information do you have? 

*Advanced: You can click on some different places in the column headers to format your data inside Tableau, including telling Tableau what kind of data you have. You don't need to do this now, but I'm telling you so you can play around with it later if you want,*

## 2. Create a sheet

In Tableau, you begin visualizing data by creating a **Sheet**. Do that by clicking on the orange **Sheet** button in the lower left-hand corner.

![][2]

[2]: images/getting-started-with-tableau-public/create-a-sheet.png

## 3. Data types in Tableau

Tableau divides your content types (that is, your columns) into **dimensions** and **measures**. Measures consist of numeric information: values that can be added together. Everything else is a dimension. Tableau will often provide recommendations based on these data types.

![][3]

[3]: images/getting-started-with-tableau-public/data-types-in-tableau.png

## 4. Your first visualization

Get started by clicking on **Applicant Arts Discipline** and drag it into the main section of the sheet (the **canvas**). It's not hugely exciting; you just see a list of arts disciplines.

There's a reason for that: Tableau doesn't know what you want it to count.

![][4]

[4]: images/getting-started-with-tableau-public/your-first-visualization.png

## 5. Tell Tableau which measure to use

We want Tableau to create a chart that visualizes the number of grants awarded per arts discipline. We want Tableau to summarize the values.

Luckily, Tableau has done this for us. Scroll to the bottom of the Data column, and look at the measure types that are in italics. You'll see that they contain the word **generated** next to them in parentheses. This means that these are numbers that Tableau has calculated for you.

You'll notice a measure called **Number of Records** or **Iowa_Arts_Council_Grants.csv(count)**. Since each record corresponds to a grant, and we want to count the number of grants, that's the one we want. Click on this measure and drag it to the table on your canvas. Drop it in the second column of the table, where the values are currently represented as "Abc."

![][5]

[5]: images/getting-started-with-tableau-public/tell-tableau-which-measure-to-use.png

## 6. Choose the chart type you want

Once you've dropped the "Number of Records" measure, you'll see that they're nicely summarized for you in the table you created. You'll also notice that highlighted options appear in the palette of chart types on the right-hand side of your window. Now that you have measures, you have some chart options! Click on the bar chart.

![][6]

[6]: images/getting-started-with-tableau-public/choose-the-chart-type-you-want.png

*What does your chart tell you about your data???*

## 7. Compare multiple values

### 7a. You created a visualization! Now, let's see if we can create a stacked bar chart. 

We'll show how **Application Instition Type** correlates with **Application Arts Discipline**.

Luckily, this is easy. Just drag the Application Institution Type measure onto the bar chart you've already created.

![][7]

[7]: images/getting-started-with-tableau-public/compare-multiple-values.png

### 7b. Adjust the chart to differentiate the "Institution Type"'s

Look at the box labeled "Marks" to the left of your chart.  

Click on the little dots to the left of the blue Applicant Insitution Type dimension.

Select "Color".  What happens? 

What happens when you hover over the colors on the bars?

What happens when you click on a bar?

*What does your chart tell you about your data??*

### 7c. The chart's legend

Look in the upper right.  Click on "Show Me" to get rid of all the visualization options. (Don't worry -- if you click on it again, they come back.). You should see the *legend* for your chart.

What happens when you click on an item on that legend?


## 8. Create a different stacked bar chart

Now, let's switch to another stacked bar chart, so we can see the distinctions among institution types more clearly. Go back to "Show Me" and display all the visualization types.  You'll notice that as you hover over each segment, a tooltip gives you more information.

Click on the vertical bar chart option.

![][8]

[8]: images/getting-started-with-tableau-public/create-a-stacked-bar-chart.png

What happens?  How did your chart change?  What are the stacks showing?

## 9. Give your chart a name

Click on your chart's title (it currently reads **Sheet 1**) to give it a more descriptive name.

![][9]

[9]: images/getting-started-with-tableau-public/give-your-chart-a-name.png

## 10. Start a new chart

Now let's make our second chart. Click on the **New worksheet** button (circled below) to begin our new visualization.

![][10]

[10]: images/getting-started-with-tableau-public/start-a-new-chart.png

## 11. Make a map

Tableau has automatically geocoded our geographic dimensions. You can tell because a tiny globe appears next to them. Drag **County** into the main canvas area, and give Tableau a moment to work.

![][11]

[11]: images/getting-started-with-tableau-public/make-a-map.png

## 12. You have a map!

Now that you've done a map, let's add a measure to it. Drag **"Iowa_Arts_Council_Grants.csv (Count)"** into the main canvas area, on top of your map. This field ("Iowa_Arts_Council_Grants.csv (Count)") is the number of records in your spreadsheet or table. In previous versions of Tableau it was called **Number of Records**.

![][12]

[12]: images/getting-started-with-tableau-public/you-have-a-map-.png

## 13. Finish your map

Now the circles on your map grow larger as the number of grants awarded to that county increases. You can fine-tune the look of your map by altering the options in the **Marks window**. Give your new map a title, as you did for your chart.

![][13]

[13]: images/getting-started-with-tableau-public/finish-your-map.png

## 14. Create a dashboard

Now we'll combine our charts to create a **dashboard** -- a snapshot of multiple visualizations. Do that by clicking on the **Dashboard** button, circled below.

![][14]

[14]: images/getting-started-with-tableau-public/create-a-dashboard.png

## 15. Drag your sheets onto your dashboard

From the left-hand side of your dashboard's window, click on each of your sheets in turn and drag them into your main canvas. Very nice!

![][15]

[15]: images/getting-started-with-tableau-public/drag-your-sheets-onto-your-dashboard.png

## 16. Options for exporting

As I've mentioned, in order to make your visualization web-accessible, you will need to create a Tableau account and publish to Tableau's site. From there, you can embed your visualizations in other web pages. To begin this process, select **Save to Tableau Public As...** from the **File** menu. You will be prompted to begin the process of creating an account, logging in, and publishing to the web.

### 16a. Publishing and embedding

Once you've published your charts to the web, you can go to your account on Tableau and get the code to embed. Usually when you **Save to Tableau Public As...** Tableau will trigger your browser to open a window with your account and your chart online. 
 -  On the upper right you will see a very small star icon and a small icon with three circles connected by lines. Click on the three circles
 -  Copy the embed code (not the link)
 -  In Wordpress create your blog post and open an HTML block in your post
 -  Paste the code into the window for your HTML
 -  **LOOK AT YOUR CODE:**
    - It opens with a <div> tag and then has a closing tag and then a lot of other code after. 
    - Delete the code _AFTER_ the closing tag </div>
    - DO NOT delete any of the stuff in the middle of the div tags
    - LOOK AT YOUR CODE: it should begin with an opening div tag and end with a closing div tag. 

There's a *ton* more you can do with Tableau. You can begin learning about its other features [here](https://public.tableau.com/en-us/s/resources).

![][16]

[16]: images/getting-started-with-tableau-public/options-for-exporting.png

### 16b. Screenshot + link

Take a screenshot. Unfortunately, the free Tableau Public doesn't have a good way to export a visualization as a static image like a jpg.  You can take a screenshot.

For the best image for a screenshot, look at the toolbar above the "Columns" field, and you'll see a little screen icon. Click on that for a clean full screen image you can screenshot. (The option below in 16c will give you a higher quality image though.)

Upload the screenshot and link to your Tableau public site.

### 16c. Download image + link

Download the image of your chart/graph from Tableau Public. In your browser at your Tableau Public account page showing your visualization, look in the upper right. 
 - Next to the star icon and three circles icon you will also see an icon that looks like a square with a downward arrow. 
 - Click it and download an image
 - Upload the image to your blog post and link to your Tableau account

## 17. Let's create a map across multiple states.

Download [this dataset about photographs in the Charles Weever Cushman Collection at Indiana University](https://www.dropbox.com/s/38yz4c64b7wb1w7/cushman-collection-lat-long-disagg.csv?dl=0).

Create a new project by going to the menu bar and clicking File > New.  Click "Connect to Data Source" and upload this file just like you did the earlier one above. (It's also a text file.)

Look at your data -- what kind of data do you have?

### 17a. Create our first map of coordinates.

Click on Sheet to create a new sheet.

Look at the "Measures" in the lower left.  Drag "Latitude" up to "Rows".  ("Latitude" not "Latitude (generated)".)

On my Tableau Public, suddenly in Rows "Latitude" now says "AVG(Latitude)".  UH OH! I don't want the average latitude!  Click on the little arrow inside the colored AVG(Latitude) oval. You'll get a drop-down menu.  Select "Dimension" so that Tableau will chart this data as a DIMENSION not as an an AVERAGE of all the entries.

Now drag "Longitude" up to "Columns".

You should see a map with lots of coordinates!

Now drag "Number of Records" up to the "Marks" panel.  **NEWER version may label this field cushman-collection-lat-long-disagg.csv(Count) instead of "Number of Records".** 
- Click on the little dots next to the colored oval there and select "Size".  
- What happens? If the dots are all the same color follow the steps below
  - On the right you'll see a legend that begins with CNT and a color slider: if the dots are all the same color, click on the little down arrow
  - Select Edit Colors
  - Select Advanced
  - Click the End check box
  - Enter 200 as the end number and hit OK
  - Now what does your map look like

Click on Sheet 1 above your map to give your map a good title.

### 17b. Now let's create another map.

DUPLICATE your sheet:  control-click or right-click on the Sheet 1 tab on the bottom. Select "Duplicate."  You should see a new tab that says "Sheet 1 (2)".  

In the "Marks" panel, click on the green oval that says "SUM(Number of Records)". A dropdown menu appears; select "Remove".

Find in the "Dimensions" panel "Topical Subject Headings 1."  Drag it over to the Marks panel.

Click on the little dots next to the blue oval and select "Color."

What happens???

Give your map a cool title!!

### 18. Go back up to Step 14 and create a Dashboard with your maps






