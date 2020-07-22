# Lab 9: Phonebook Application

*Due: Friday, July 24, 2020* 

**The goal** of this lab is to install a pre-built PHP/MySQL application on your localhost, and then extend it to do more than it was originally built to do.

**The purpose** of this lab is to show that you can read and understand code for a basic front-end application well enough to edit it. 

Note: this lab comes in two parts:

- Lab 9 (this part) has you install and then edit a Phonebook application
- Lab 10 will have you move your phonebook application to a class production web server

Both Lab 9 and 10 will be graded after you complete both parts.

## Installation

In this step you need to just install a pre-built application by setting up a new database, editing your files so they work with it, and then testing to make sure everything works.

- Download and extract [this set of starter files, phonelist.zip](lab09-phonelist/phonelist.zip) to a new folder named **lab09** in your web root
- Start your localhost (MAMP or MAMP for Windows), if not already

- In **phpMyAdmin**, create a new database, and an associated user/password
  - Remember: this is a three-part process that you can do in phpMyAdmin all at once
  - Suggestion: set the database and the user to **lab09** and keep the password simple
- In **phpMyAdmin**, click on the **lab09** database and ***Import*** the **phonelist.sql** file
  - Check to see if the SQL script worked...
  - There should be a new table, "*phonelist*" in your database with three fields: **id**, **firstname**, and **lastname**
  - When you *browse* the phonelist table, you should see one record, *1* \| *Placholder* \| *Delete Me!*
- Test to make sure you can connect to your database from a PHP file running in your localhost
  - Enter the user, password, database credentials in your **testmysql.php** file; save and close the file
  - Open **testmysql.php** in a web browser
  - If you get "Connection OK..." then you're okay! if not, figure out what went wrong before proceeding

- In the **lab09** folder, edit the **connect-db.php** file; enter the database variables using the login credentials that you tested in the previous step; then save and close that file

- In a web browser, navigate to your localhost and go into the **lab09** folder
- Test all four database functions (CRUD)
  - If you see the table and record #1, that's the Read function
  - Make sure you can Create, edit (Update), and Delete records

## Extend the Application

This part of Lab 9 involves editing the database and application files to include two new data fields:

- Phone number
- Email address

### Edit the Existing Table

- In phpMyAdmin, in the **lab09** database click on the **phonelist** table
- Looking at the *structure* of the phonelist table, find the area that says Add "1 column(s) [after lastname]"
  - Change the "**1**" to "**2**"
  - Click the **Go** button
- Setup the two new columns:
  - Name: **phone**, Type **VARCHAR**, Length/Values **50**
  - Name: **email**, Type **VARCHAR**, Length/Values **100**
  - Click the **Save** button

You can close or put-aside phpMyAdmin for now

### Edit the Application Files

*Note: for some CSC 174 students (especially those with no prior programming experience) this might be tricky, but not impossible! Carefully look at the lines of code indicated in the instructions below and make the changes as needed to get the application to work with the two new database fields.*

*The instructions are <u>not</u> explicit.  You are expected to understand the code well enough to know what to do. But as always, if you get stuck, reach out for help in the #help channel in Slack.*

- Edit **renderform.php**

  *Note: renderform is used as a PHP Include for both the new.php and edit.php files.  It's the same HTML form in both files so that's why it's placed here in this separate file. Also note that the HTML form in renderform is inside a PHP function so it can be passed arguments when called.*

  - Look at **line 3**; notice that the *renderform()* function has four arguments: `$id, $firstname, $lastname, $error`; add two new arguments to that list: `$phone` and `$email` 
  - Look at **lines 20** and **21**; they put two fields in the HTML form - one for the first name and the other for the last name; add two new fields (new lines 22 and 23) to add fields for the "phone" number and "email" address

- Edit **index.php**
  - Look at **lines 18** and **19**; duplicate those lines (new lines 20 and 21) to create table headings for the phone number and email address columns
  - Look at **lines 29** and **30**; duplicate those lines (new lines 31 and 21) and edit the array keys to match the column names (hint: 'phone' and 'email')

- Edit **new.php**:
  
  - Look at lines **lines 10** and **11**; duplicate those lines (new lines 12 and 13) and edit the names in the super globals to match the names from the renderform name="" attributes (hint: 'phone' and 'email'); also, change the variable names accordingly (hint: `$phone` and `$email`)
  - Look at **line 16**; edit that statement to include: ...*OR `$phone ` is equal to blank OR `$email ` is equal to blank*
  
  - Look at **line 21**; edit the list of arguments on the renderform() function to include: `$phone` and `$email`  
  
  - Look at **line 25**; edit the SQL statement to include the phone and email fields
    - Be very careful with this one - very difficult with all the quotes, commas, and parenthesis)
  - Look at line **32**; add two more empty quotes with commas to accomodate the two new arguments
  
- Edit **edit.php**
  - Look at lines **lines 13** and **14**; duplicate those lines (new lines 15 and 16) and edit the names in the super globals to match the names from the renderform name="" attributes (hint: 'phone' and 'email'); also, change the variable names accordingly (hint: `$phone` and `$email`)
  - Look at **line 19**; edit that statement to include: ...*OR `$phone ` is equal to blank OR `$email ` is equal to blank*
  - Look at **line 24**; edit the list of arguments on the renderform() function to include: `$phone` and `$email`    
  - Look at **line 28**; edit the SQL statement to include the phone and email fields
    - Be very careful with this one - very difficult with all the quotes and commas)
  - Look at **lines 49** and **50**; duplicate those lines (new lines 51 and 52) and edit the array keys to match the column names (hint: 'phone' and 'email'); also, change the variable names accordingly (hint: `$phone` and `$email`)
- Look at **line 55**; edit the list of arguments on the renderform() function to include: `$phone` and `$email`  
  
- Then test all four functions in your web browser
  - If all four database functions continue to work then just leave your files and database as-is until next time when we'll move them to the class web server
  - If any of the four functions don't work you'll need to figure out where you went wrong and fix it before the next class



