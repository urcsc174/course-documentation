# Lab 10: Remote Phonebook Application

*Due: Monday, July 27, 2020*

**The goal** of this lab is to take the database application you created on your localhost in Lab 9, and reconfigure it so it uses a remote database (on the class web server); and also create a version of Lab 9 that runs on the class web server.

**The purpose** of this lab is to learn how to decouple a website application from its database so it can be installed and run anywhere.

## Part 1: Localhost Files and Remote Database

### Step 1: Export Your Database Table

- In phpMyAdmin, **export** your table (not the database) from your local phpMyAdmin to an SQL file

*On your localhost, you created a database that had only one table in it: your "phonelist."  When you move your data to the class web server, we'll all be using the same database therefore we all need to have uniquely named tables. So...*

- Open the SQL file for editing and **search and replace** all instances of `phonelist` with a prefix that uses your first initial and last name like this: `rkostin_phonelist`

Save and close the file and put it aside. You'll need it soon.

### Step 2: Login to Bluehost

- Go to [www.bluehost.com](https://www.bluehost.com)

- Login with domain: **csc174.org**<br>And password: **[see the #announcements channel in Slack]**
  - NOTE: please try and get the login right.  If you screw it up multiple times in a row, we will <u>all</u> get locked out!

- Once logged-in, click **cpanel** in the submenu

Then put this web browser tab with your connection to Bluehost aside.  You'll need it later.

### Step 3a: Test Your Connection to the Remote Database

- Open your file: **testmysql.php** file in your localhost and change the login information to these new login settings.  
  - Host: **66.147.242.186**
  - Database user: **urcscon3_lab10**
  - Database password*: `**********`
  - Database name: **urcscon3_lab10**

\* *Replace the `**********` above with the password listed in the #announcements channel in Slack.*

- Save the file and then open it in a web browser (using localhost).
  - Maybe you'll get the "Connection OK" message in the viewport because your IP number is already registered with Bluehost; if so, skip to Step 4
  - Or, if after a long wait you get the "Connect Error (2002)" message, do the following step to setup remote access...

### Step 3b: Setup Remote Access to the Remote Database

You can skip this step if you got the "Connection OK" message in the previous step.  Else do the following.

- Go back to the web browser tab open to Bluehost
- In the cpanel, scroll down to click the **Remote MySQL** chicklet (or you'll probably find a link to it along the left-side, under "frequently used features")
- On the "Remote Mysql Database Access" page, click the [Add] link to add **Your Class C** (<u>not</u> *your IP*)
- When your Class C is showing in the text box, click the green **Add** button
- Go back to your web browser pointed at **testmysql.php** and refresh it;  you should get the "Connection OK" message in the viewport
- In the web browser tab pointed to Bluehost, click **cpanel** in the submenu to go back to the cpanel

### Step 4. Import the Lab 9 Database Table on the Remote Server

1. In the cpanel, scroll down to click the **phpMyAdmin** chicklet (or you'll probably find a link to it along the left-side, under "frequently used features")
2. In the left-side bar, click the name of our Lab 10 database, **urcscon3_lab10**
3. Click the **Import** tab in the top area
4. Click the **Choose File** button and select your edited SQL file from Step 1.
5. Scroll down and click the **Go** button

Hopefully, you'll see a long list of green messages.  If so, proceed to the next step.

### Step 5: Change the Connection Information

Go to your files from Lab 9's Phonebook Application and open the **connect-db.php** file

- Change the database connection variables to the same information used in step 3a, above

### Step 6: Use the Remote Database with your Local Web Application

1. Open the following PHP files from the Four Functions web application in your code editor
   - **index.php**
   - **new.php**
   - **delete.php**
   - **edit.php**
2. Search for every instance of "**phonelist**" in those PHP files and replace them with the new table name based on your first initial and last name, example "**rkostin_phonelist**"
   - In **index.php** there is one instance
   - In **new.php** there is one instance
   - In **delete.php** there is one instance
   - In **edit.php** there are two instances
3. Save and close those files
4. Test the Phonebook Application  in your localhost again
   - Make some additions, edits, deletions ...whatever
   - In the phpMyAdmin that's on the Bluehost web server (*not* your localhost) "browse" your table on the remote server; you should see your additions, edits, and deletions there

## Part 2: Remote Files and Remote Database

For this part you need to FTP your Phonebook Application to the class web server and make sure it continues to work.

- IMPORTANT: edit your **connect-db.php** file again. Change the `$server` information from `66.147.242.186` back to `localhost`

- Open your FTP software and login using the following web server credentials, below.<br>*Note: everyone will use the same FTP account. Be careful not to disturb anyone elses' files.*

```
FTP Server (a.k.a. Hostname): ftp.csc174.org
FTP Port: 21
FTP Username: lab10@csc174.org
FTP Password: [same as before]
```

- When you FTP-in to the account, create a folder using your first inital and last name (e.g. **rkostin** place your application files in there

Test the remote version of your remote application on the class web server: 

`csc174.org/lab10/flastname/`

## Turn It In

- When the remote application and database is working, login to our CSC 174 area in Blackboard and go into the "Labs Assignments Turn-in" area
  - Find the assignment: **Lab 9/10: Phonebook Application**
  - Copy and paste the URL of your application into "Write Submission" 
  - Submit the assignment
