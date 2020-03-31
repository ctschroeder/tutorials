# Paint That Page with CSS

## About this tutorial

This tutorial has been modified from [Dr. Miram Posner's "Paint that page with CSS" tutorial](https://github.com/miriamposner/html_css_workshop). Last modified by Caroline T. Schroeder for OU's Intro to DH, 31-March-2020.

**Important Note:** There are a lot of steps to this tutorial.  If you decide to do just a couple, that's fine.  Do what you have time to complete. Just be sure to skip down to sections 10 and 11 fo finish the tutorial!!

## About CSS

You've [used HTML to build your webpage](https://github.com/ctschroeder/tutorials/blob/master/html_css_workshop/HTML_Tutorial.md), but it doesn't have a lot of
style yet. Let's add some with **CSS**.

CSS stands for **cascading style sheet**, a somewhat confusing name for
a language that you use to format your page so that it looks just the
way you want. CSS can get super-complicated, but the basic principles
aren't hard to master.

## 1. Getting Set Up

For this tutorial, we will use your computer's text editor application, just like we did in the [HTML tutorial}(https://github.com/ctschroeder/tutorials/blob/master/html_css_workshop/HTML_Tutorial.md).

1. Open your index.html file from that tutorial.  
2. Also open **two new, blank files** in your text editor.
3. Copy and paste (NOT cut) every thing in your index.html file into one of your new, blank files.
4. Now close the index.html file so you don't change it on accident.
5. Be sure your new file is in **plain text format**. 
6. Save it with a new filename (not index.html); please use the .html ending, though. (So, mine could be ctschroeder.html or ilovebtvs.html or whatever fits with the content of your file.)

## 2.Link your HTML document to a CSS document

You should have two files open in your text editor:

  1. A plain text file with a unique filename ending with .html; the contents look the same as your index file.  We'll call this your HTML document.  If have a very simple HTML document with only text, you may need to add to or change its contents so you have all the elements described below.  If you completed the full earlier tutorial, you already have a header, link, and image in your HTML file, and you're good to go.
  2. A blank plain text file with no contents, no filename.
  
**Dr. S Protip:  Remember from our previous tutorial, that you can save your HTML file and open it in a browser. Put the browser side by side with your text editor. When you make changes to the CSS file or the HTML file the text editor, save the changed file, and refresh your browser. You will see the effects of your changes in the browser!  If you don't see the change, first make sure you've saved BOTH the HTML and CSS. Sometimes I change the CSS, forget to save the CSS file, and then wonder why my changes don't appear in the browser.**

![](css1_images/media/ssimage1.png)

You can add CSS styles to your HTML document in a few different ways,
but I like to keep all of my CSS rules in a separate document. Go to your second
new text document -- the empty one -- (be sure it's **plain text format**) and save it in
the same place as your html document with the name **style.css**.

Now we have to tell the HTML document to look for the CSS document in
order to receive information about styles. Luckily, that's not too hard.
Inside the **&lt;head&gt;** tags on your html document, type

**&lt;link rel="stylesheet" href="style.css"&gt;**

Now you should be linked!

**NOTE: The demo images show changes to the main index file (index.html is the document name). When YOU are doing this tutorial, you will be working on a new HTML file, not index.html. I'm asking you to make a new file so you can see the difference between the two files, you can practice making a link, and practice uploading more files to the server.  Please don't freak out when you see index.html in the images here.**

Now you should be linked!

## 3. How CSS styles work

![](css1_images/media/ssimage2.png)

The basic rule is that you specify the html tag you'd like your rule to
affect and then say what you want to do to the content inside the tag.
Then all of the content inside of that tag will be affected.

In the example above, I've specified that all of the content inside
**&lt;h1&gt;** tags should be made blue and transformed into the
Helvetica font. Notice that the content inside the paragraph tags isn't
affected. That's because the paragraphs are not inside the **h1** tags.

As you can see, your rules go inside angle brackets, which look like
this **{ }** and are separated by semicolons.

## 4. Make everything different colors!

![](css1_images/media/ssimage3.png)

Everybodys know that the more color a webpage has on it, the better it
is.

## 5. Change background colors

![](css1_images/media/ssimage4.png)

To CSS, every element on your webpage forms a box. You can change the
background color of this box by using the background-color style rule.

As you can see above, even the body tag forms a box that contains
everything on the page. Who wants a boring background color? Make that
page stylish!

## 6. Add some borders

![](css1_images/media/ssimage5.png)

Since everything on your page is a box, you can add borders around
everything. Notice that I've also put a border around my dog photo by
using the **img** tag.

## 7. Do some resizing

![](css1_images/media/ssimage6.png)

You can change pretty much anything with CSS, including sizes. I want my
dog picture to be smaller, so I'm going to add some style rules for the
**img** tag.

I've chosen to use percentages, but you can also use pixels (50px).

## 8. Move things around

![](css1_images/media/ssimage7.png)

You can use CSS to move things around on the page. The most direct way
to do this is to change the **margins** (the space between the element
and whatever's next to it). I'm going to scooch my dog picture over to
the right by increasing its left margin. (See what happens when you try
**margin-right**, **margin-top**, and **margin-bottom**).

## 9. Add some padding

![](css1_images/media/ssimage8.png)

Margin is the space between an element and its neighboring elements.
**Padding** is the space between a piece of content and its borders.
Let's give the header some more padding to make it stand out. Looking
good!

## 10. Add a link to your new file in your index file!

Open your index.html file in the text editor. (If you double-click, it will probably open in the browser.  You may need to right-click on the file to "Open in..." the text editor.  If your text editor application is already open, you can go to the text editor's Menu and go to File > Open to open index.html)

Somewhere on the index page, add a link to your new page that reads something like "Check out this page formatted with fancy CSS" (or whatever you want).  Remember, the [HTML tutorial section 4 tells you how to make a link](https://github.com/ctschroeder/tutorials/blob/master/html_css_workshop/HTML_Tutorial.md).  The link will be whatever your subdomain URL is + / + the name of your new file.  So mine might be https://test-pages.carrieschroeder.oucreate.com/ilovebtvs.html . (This link is not live -- it's just an example.)

Now your index page links to your new page, so people can find it!

## 11. Save and Upload Your Files to the Web

No one can see your awesome web design yet.  

Go to the tutorial on [Creating a Subdomain and Uploading Files to Your OU Create Server](https://github.com/ctschroeder/tutorials/blob/master/html_css_workshop/upload-file-OUCreate.md).
  - **If you haven't done the subdomain+upload tutorial before**, do the whole tutorial.  Upload all your files -- the revised index page, the new HTML page, image files, the CSS page -- to your subdomain.
  - **If you have done the subdomain+upload tutorial before**, login to your OU Create account and skip to section 2 on the File Manager and repeat the steps to upload files. Upload the new and newly revised files (since you revised index.html in step 10, don't forget to upload that one). You may get an alert asking you if you're sure you want to replace the old index.html file.  You do!
  
**Now test it out by going to your subdomain -- do you see your index file now with a link to your second HTML page?  Can you click on the link and go to the page gussied up with CSS?**

Congratulations!
