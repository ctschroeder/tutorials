# Google My Maps Basics Tutorial

This tutorial will show you how to upload a spreadsheet (or other structured data file like a csv file) of georeferenced data to create a custom map in Google Maps.

It works best in the CHROME browser.

Created for the University of Oklahoma's Introduction to Digital Humanities course. It lives online at https://github.com/ctschroeder/tutorials/blob/master/google-my-maps-basics.md. Licensed [CC-BY-NC 4.0](https://creativecommons.org/licenses/by-nc/4.0/).  Last updated 3/7/2021.

## 1. Upload Your Data

For this tutorial, use will use the same [Cushman Collection dataset about photographs at Indiana University](https://www.dropbox.com/s/38yz4c64b7wb1w7/cushman-collection-lat-long-disagg.csv?dl=0) we used for Tableau.  Download the file as a csv.

Navigate to Google's My Maps feature at https://www.google.com/maps/d/u/0/ .  

Click "+Create a New Map".  A base map will appear.

In the white info box on the left, click "Import".  Navigate to your file on your computer and upload it.

Google Maps will ask you to tell it the fields with the georeferenced data.  Click BOTH "Latitude" and "Longitude".

Google Maps will ask you to tell it the field to use as the title for your locations. You can pick what you want -- I will choose "IU_archives_number".  (You can pick something else if you want.)

A pretty map with markers on all the locations of the photographs should appear.

## 2. Select Labels for Your Markers

Notice your markers all have the same color and are unlabeled.  

In the white info box on the left, click "Uniform Style".  You will see two sets of options.

On the "Set labels" option, pick a field for the label for each marker.  I will pick "description_from_slide_mount".  (You could pick a different one, but make it informative for your map viewer.)

Close that little window and look at your map.  How has your map changed?

## 3. Customize your markers

### 3a. Change the color or style for all of them

Click the little paint bucket next to "All items".

Change the color or icon.  I am choosing the camera icon for photographs.

What happens to your map?

### 3b. Change the color or style for different groups of entries

Directly underneath your filename in the upper left box we are working in, you should see something that says something-something "Style"; mine says "Uniform Style". Hover over it with your cursor and you'll see a pop-up that says you can "Customize the appearance" of features on your map.  Click on it.

This time use the "Group Places By" option. Click on that and set it to "genre_1". What happens?

If you want to change the icon or color for each group, click on the paint bucket for each group.

## 4. Add images to your pop-up windows

Click on one of your markers. What pops up?

Right-click or control-click on the link in the image_url field and "Copy link address".

In the same window with the information on your marker, click on the little camera at the bottom of the window.  
 - Click on "Image URL" in the new window that appears.  
 - Paste the link address you just copied there.  
 - Save

What's in your popup window now?

Unfortunately, there doesn't seem to be a good way to get Google My Maps to automatically preview the image from your spreadsheet data.  (If you figure it out, let me know.  We used to be able to do this.) So if you want an image preview you need to do it for every entry manually.

## 5. Publish your map if you want to share it

First, be sure to provide a good description and title for your map -- including a description of and link to your dataset!!!  Click on "Untitled Map" at the top of the white box and give your map a title and description. 

Click "Share" to publish your map.  

 - If you only want people with a direct link to view it, choose that option.  You can send the public link to your friends.

 - If you want to embed your map into a website, you must make it public for everyone to view.

Select your option. 


Then click "Preview" to see the version your friends or the public will see.

## 6. Embed the map

You can always take a screenshot of the map and then link to the live version on Google.

You also can embed the map.  Click on "Share" in the public map for options to tweet it, facebook it, or embed it.


