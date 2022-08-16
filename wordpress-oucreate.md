## Installing WordPress on your Domain at OU Create ##

### About this tutorial ###

This tutorial will teach you how to install WordPress on your domain at OU Create
- **If you already have your own (sub)domain on OU Create or on another hosting service you may use that. Check in with Dr. S before moving ahead**
- **If you know programming or other web applications and you DON'T want to use WordPress, check with Dr. S**

This tutorial lives online (with live links) at https://github.com/ctschroeder/tutorials/blob/master/wordpress-oucreate.md.

Last edited for Dr. Schroeder's Fall 2022 courses.

### Setting up your website AT your domain ###

1. Go to https://create.ou.edu

2. Click “Login” and login using your regular OU credentials

If you know web programming, you can use whatever system you like.  If you don’t, I recommend you use WordPress, which is the dominant content management system on the web.  (If you want you can [read more about web applications](https://create.ou.edu/docs/web-apps/what-exactly-is-a-web-application/)). 

#### Installing Wordpress ####

1.	Click on CPanel once you’ve logged into create.ou.edu if you're not already there. (CPanel is a window with a lot of applications icons on it.)

2.	You should see a panel with a lot of applications.  When you get to that panel, click on WordPress, and then click on “Install this application” 

3.	You should get to a window with the Installatron install wizard:
If you are using WordPress for your main website:  **make sure the DOMAIN is your website using https not http, and DIRECTORY is BLANK. You may need to delete “blog” from DIRECTORY.**
 
![Installatron](https://github.com/ctschroeder/tutorials/blob/master/images/installatron.png)
 
On the same page, scroll down to SETTINGS.   

![Installatron Settings](https://github.com/ctschroeder/tutorials/blob/master/images/installatron-settings.png)

4. In SETTINGS tell Wordpress:
  - The login username you want for your website.  
      - (This is different from your OU Create login which uses your 4x4).  OU Create is your webhosting service provider.  create.ou.edu is where you manage your account.  When you install software on your website, you will login to that software to update your website, just like you do to post to the class blog. (See https://create.ou.edu/docs/web-security/accounts-passwords/ for more details):
  - The login password
  - Check the email address is correct
  - Your website’s title (you can change this later)
  - Your website’s slogan or tagline  (not required/you can change this later)
  - YES limit login attempts (this ensures bots can’t attack your site)
  - NO do not enable multisite (unless you already have plans to set up multiple websites using WordPress!)

5. Make sure everything on this page is as you like it and click INSTALL.

6. You will get to a page that tells you the web address of your website and the web address to administer it.  
This should look like https://whateveryoupickedforyourdomainname and https://whateveryoupickedforyourdomainname/wp-admin 

7. BOOKMARK these pages. 

8. Click on the admin address (with wp-admin) and Customize your site!!  

### What If I Forget My Domain Name or Password??? ###

You can also **find your (sub)domain again** by going to create.ou.edu

   - Go to https://create.ou.edu and click login in the upper right
   - Login using your OU credentials
   - On the new screen, you should see your domain on the right under "Primary Domain"
   - If you need to change your WordPress password
     - click on the WordPress logo
     - click on "My Applications" in the upper right
     - click on the little wrench icon next to your website title
     - enter a new password in the password field
     - click "save all" button at the bottom right


This work is licensed by Caroline T. Schroeder under a [Creative Commons Attribution-NonCommercial 4.0 International License](https://creativecommons.org/licenses/by-nc/4.0/)
