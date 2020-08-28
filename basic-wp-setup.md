## Setting Up Your Basic Website in WordPress

### About this tutorial

This tutorial was created by Caroline T. Schroeder using some content from the staff at OU Create, licensed [CC-BY-NC 4.0](https://creativecommons.org/licenses/by-nc/4.0/). Last updated for Fall 2020 courses.  This page BLATANTLY STEALS text from the [OU Create Wordpress](https://create.ou.edu/docs/web-apps/wordpress/) documentation. Please credit OU Create if you use this tutorial.

This tutorial lives live online at https://github.com/ctschroeder/tutorials/blob/master/basic-wp-setup.md

** OU maintains a robust set of [support documents](https://create.ou.edu/docs/) including a LONG tutorial for [setting up your WordPress site](https://create.ou.edu/docs/web-apps/wordpress/). 

This tutorial focuses on the BARE MINIMUM you need to do to set up a basic WordPress site for **my course**, before adding a lot of content.

### 1. The WordPress Dashboard

The Dashboard is where you give WordPress all of its instructions on how to display your site.  You should be familiar with it, because you probably have already used it in a Private Student Blog or Discussion Site in the course already.

To get to your dashboard, you go to your domain with /wp-admin/ tacked on to the end.  So if your OU Create (sub)domain is imsocool.oucreate.com, you would go to https://imsocool.oucreate.com/wp-admin/

### 2. Title

Go to Settings > General on your dashboard. Once you’re on the General Settings page, you can give your blog any title you want. You can also give your blog a tagline, which can be a short description of the blog.

When you change the Blog title and tag line, they will show up at the top of your site. Depending on what theme you use, the title and tag lines will show up in various places. In the case of some themes, they might not show up at all depending on whether they allow custom configurations. We won’t worry about that for now.

### 3. Themes

The look and layout of your WordPress site is determined by the Theme.  There are a MILLION themes for WordPress. The OU Create documentation page about [setting up your WordPress site](https://create.ou.edu/docs/web-apps/wordpress/) has a section on WordPress Themes with pictures!!!

When you install WordPress, the default (or pre-set) theme is called [Twenty Twenty](https://wordpress.org/support/article/twenty-twenty/) (as of WordPress version 5.3). It is a very customizable theme. You can easily modify the colors of the different fonts and backgrounds used in the theme and even choose between different templates for each page.

To pick a different theme and activate a theme go to Appearance > Themes in your dashboard.  You will see thumbnail images representing each of the themes that you currently have available on your site. Simply mouse over any one of them, and click the Activate link.

**Note: You don't have to install a new theme immediately. If you're new to this it's perfectly ok to stick with the Twenty Twenty Theme!!! If you want to keep Twenty Twenty, skip to Step 4 below.**

If you don't like the themes you see, you can install a new one. (Our course site uses the theme Gutenix.)

- Navigate to Appearance > Themes. 
- Click the Add New Button
- Hover over each theme, and you'll see options to Install, Preview, and Details & Preview. Click Install to add a new theme to your site.
- You can search for themes based on features, and you can also see what themes are popular. Look at the little menu that says Featured Popular Latest Feature Filter on the top.
- Once you've installed a theme you need to ACTIVATE it before it will show on your site.  You should see a link to Activate after Wordpress has downloaded and installed. You an also navigate to Appearance > Themes in your Dashboard and activate it from there.

### 4. Pages and Posts

There are two basic kinds of content for Wordpress: Pages (your basic web page) and Posts (Blog posts that appear on a blog, like the News page of the course website.) The OU Create documentation page about [setting up your WordPress site](https://create.ou.edu/docs/web-apps/wordpress/) has a good section about "Publishing Content" with screenshots, images, and more info on Pages vs. Posts -- go check it out!

You will need to choose if you want your Home page for your site to be your blog roll or a web page. Advantage of a blog -- all your new content appears right away. Advantage of a Page -- information about who you are, what the site is is always there; you can add links to your latest posts in a separate area of a Page called a Widget. We will talk about those later!!!. **You can always change your mind later, so just pick one for now!!!**

If you choose a Page for your Home, then you want to be sure you *have* a page to show. 
- On your Dashboard Navigate to Pages > All Pages on the left menu 
- You will see any sample pages your theme may have for you
- Play around by modifying a sample page or create a new one by either clicking on the Add New Button on the top of the Pages dashboard or clicking on the left menu Pages > Add New
- Creating a Page is a lot like a Post -- you should be familiar with how to do this from the Student Blog/Discussion Page. Adding text, images, etc., to a page is the same as adding it all to a post.

Once you've made a Page, be sure to publish it! 

### 5. Customize your theme

Depending on your Theme, there are different ways to customize. Your Theme has a built-in little tutorial to walk you through Customization. 

Go to Appearance > Customize on the lefthand dashboard menu. *Each theme has different options. Don't freak out if options I discuss here aren't in your theme.* 

- Click on Site Identity and make sure it looks the way you want

- Under Homepage Settings, select either a Static Page or Page of Posts for your home page. (See discussion in #4 about this choice.) If you chose Static Page, you'll be prompted to pick a specific page.

- Pick colors, header image or format (may not be in Twenty Twenty theme), font, etc.  **You can get lost in all these options; if you're new to this, you can stay basic until you're more familiar!**

Be sure to click "Publish" at the top when you're done to publish your site!!!

### 6. Menus

#### About Menus

Menus help your readers navigate your site.  The OU Create documentation page about [setting up your WordPress site](https://create.ou.edu/docs/web-apps/wordpress/) has a GOOD section about "Building Your Custom Menu" with screenshots/images. CHECK IT OUT if you're confused.

There are TWO ways to create/edit your menus

1. In the Dashboard, navigate to Appearance > Menus

2. In the Customization view, click on Menu(s)

#### Create a menu

You need to create a menu to put one on your site. I'm going to describe #1 about -- creating a menu in the dashboard.

- In the Dashboard, navigate to Appearance > Menus

- Enter a menu name in the Menu Name box. (I often use Main Menu as the name for the main menu I want to go across the top of my website. Some people use Primary.)

- Some themes will give you an option about where to put the menu -- click the boxes you want. In Twenty Twenty, I put the Main Menu in my Desktop Horizontal Menu (because that runs across the top) AND the Mobile Menu

- Click "Create Menu"

You can then add Pages, Posts, Custom Links (links to outside websites), and Categories to your menu

#### Add Items to your menu

To add a Page to the menu:

- Click on the little down arrow next to Pages on the list under **Add Menu Items**
- Click View All to see ALL the pages you have on your site
- Select the box next to the page(s) you want to add and click Add to Menu
- They are now in the menu under **Menu Structure**
- You can CHANGE the way the name of the page appears in the menu. Click on the arrow next to the page in the **Menu Structure**
- Type in what you want to see in the menu into the Navigation Label box; for example, I might have a page titled "Digital Humanities Course Schedule" that I want shortened into "Schedule" on the menu. 
- Click Save Menu

You can do the same for links to other web pages and for posts.

You can also add a link to ALL posts or pages with the same Category by clicking on Categories under **Add Menu Items**. You will use this feature for your course website.

Save menu!!

### 7. Publish your site!

Be sure you've published your site.

### Bonus (Stuff you may need to do eventually but can TOTALLY skip now.)
Once you're familiar with all this, you can go to the OU Create documentation page about [setting up your WordPress site](https://create.ou.edu/docs/web-apps/wordpress/) and read and implement the sections on
- Basic Privacy
- Discussion Settings
- Managing Comment Spam with Akismet
- Permalinks
- Widgets
- Plugins
