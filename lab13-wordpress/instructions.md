# Lab 13: WordPress (localhost only)

*Due: Wednesday, August 5, 2020*

**The goal** of this lab is to install and use the popular Content Management System: WordPress. 

**The purpose** of this lab is to practice the procedure for installation (and see how easy it is) and then get some hands-on experience using the CMS 

## Install WordPress

- On your localhost, **create a new database and associated user**.
  - You can call it whatever you want, e.g. **lab13wordpress**
  - Make sure you have a associated database user and password with that new database
- Download WordPress from [www.wordpress.org](https://wordpress.org/) then extract and and move the **wordpress** folder to your web root
- Open your localhost in a web browser and navigate into the wordpress folder to initialize the WordPress installation
  - Note: your WordPress login you will create will be totally separate from the database credentials and all other username/password on your system; use (and remember) whatever username and password you want
- Carefully complete the installation and then login to WordPress

After you successfully install your WordPress website on your local host take some time to

- Look at the "frontend" of the website: go to: [http://localhost/wordpress/](http://localhost/wordpress/)
- Look at the "backend" of the website: go to: [http://localhost/wordpress/wp-admin/](http://localhost/wordpress/wp-admin/)
- Open up your file system and browse around; open some of the files and see how it's constructed; noticed that it's not very intuitive - certainly not as straightforward as a static website. As you'll see there are lots of PHP includes and SQL Select statements in PHP loops ...instead of actual content.
- Also, open phpMyAdmin and look at your Lab 13 database.  That's where all the dynamic content is stored and retrieved for both the front- and back-ends of the website

## Install a Theme

- Starting from the WordPress "Dashboard" navigate to the "Themes" utilities (under Appearance/Themes) use the "Add New Theme" widget to select, install, and activate a new theme.
  - Do NOT use one of the pre-installed Themes; click the **Add New** button and find a new, interesting (and fairly simple) Theme to install and activate

## Customize the Site

- Using the Settings area, go into "General" and change the **Site Title**, **Tagline**, and some of the other settings
- Explore - and play with - the other areas under Settings; make some changes

## Load Content

Try adding creating new "Pages" and "Posts" with some dummy content and see how they appear on the front-end 

- Copy & paste content from anywhere, upload images
  - Add some **Media**
  - Create some **Posts**
  - Create some **Pages**

## Get Credit

For lab credit: **take the following screen shots** of your WordPress website and submit the image files in Blackboard to get credit for Lab 13

- Your Dashboard, with your localhost web address clearly shown
- Your Themes page (in Appearance \| Themes) with your new, installed/active Theme clearly shown
- Your website front-end with your localhost web address clearly shown 