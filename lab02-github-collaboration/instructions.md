# Lab 2: GitHub Collaboration

*Due: due: Wednesday, July 1, 2020 …today*

**The goal** of this lab is to get up-and-running with GitHub quickly and experiment with collaborating on a simple website to see how it works.

**The purpose** of this lab is to demonstrate how working with a team of web developers is better than working alone using these common industry tools:

- **Localhost** - to work independently
- **GitHub** - to sync your independent work with the rest of the team
- **Slack** - to communicate with each other remotely and asynchronously

## Step 1: Join a Team

- Go to [this shared Google Sheet](https://docs.google.com/spreadsheets/d/1z0z8gNCR0_-zW18ft0YDoiLPn6z4OTuAM5P8jVIa7cg/edit#gid=0) and **move** (cut & paste, or drag) your name/email from the "Pick list" to any "City-team"
  - It doesn't matter if you're #1, 2, or 3

- When you get other members in your City-team, DM each other in Slack and then one of you, create a *private* channel in Slack, and then invite the other members.  
  - This will be a temporary channel that you can delete after this lab is complete
  - You will use your private channel to coordinate with the other team members
- Amongst your team, decide on the name of a city somewhere in the world, and back in the Google Sheet, change your city-team name (column header) from **City-Team #n** to your city's name

## Step 2: Set-up a GitHub repository

- Everyone in your team needs to [have or create an account in GitHub](https://github.com)
  - Note: you can setup an "academic account" or something like that, that gives you some extra features; if you have any questions about that, leave a message in the #help channel in Slack
- In your team's private channel in Slack, share your GitHub user names with each other
- In your team, decide amongst yourselves which one of you will create a new GitHub repository for Lab 2
  - IMPORTANT: make it "Public"
- Whoever created the repository, go into **Settings** and then **Manage access**
- Click the **Invite teams or people** button, and then invite the other members of your team

## Step 3: Setup GitHub Desktop

- If you haven't already, go to the [GitHub Desktop](https://desktop.github.com/) website, and download and install the desktop software on your computer
- Use the desktop software to **Clone a repository** 
  - In the **Clone a Repository** dialog box, select the new repository from GitHub.com
  - BE CAREFUL HERE: don't click the Clone button too quickly!  Read the next step...
- In the **Clone a Repository** dialog box, *change* the **Local Path** to a new folder named **lab02** in the  document root (a.k.a. web root) of your localhost

## Step 4: Build a Website together

The intent here is for your team to take everyone's **Lab 5** files from CSC 170, and stitch them together into a quick website.  

- The website just needs to have a new, working **navigation element** to switch between the three pages

- There does *not* need to be an **index page** (home) in this website
- If there are any mistakes (incorrect things), your team needs to fix them

Once everyone is up-and-running with a shared repository in your own localhost, communicate with each other in your private channel in Slack and divide-up the following roles:

- Who will manage the file system - fixing file names and folders, and making sure the files and folders are correct (even if something was incorrect, it has to be fixed)
  - This person will start everything off and prepare the files for the others to work
- Who will build a simple navigation system and insert it into the web pages
  - This person will focus mostly on the HTML
- Who will make sure everything looks good (enough) to be usable and functional
  - This person will focus mostly on the CSS

### Hints and Tips

- When someone is in the repository arranging files and folders (moving and renaming things), that person needs to:
  - Tell everyone to and **push** their latest changes to GitHub and then STOP working
  - When everyone confirms that they've stopped, make the changes in the repository
  - When done, alert everyone and have them do a **pull**, and then carry on
- Suggestion: at some point in the process, do a "conflict" on purpose to see what that's like
  - Have two people edit the same line of one file
  - Have them both commit and then push the changes to GitHub
  - The second person doing the pushing will get an error message; that person needs to open their files in their localhost, look at them and make everything right (and then clean-up/delete) the markers that GitHub left in your files
  - Then do another push to GitHub

## Step 5: Installation

When everyone has the finished website in their own local repo:

- Decide amongst your team who will publish the website to the class web server, and then do it

Note: each team will use the same FTP account. Be careful *not* to disturb other teams' files.

```
FTP Server (a.k.a. Hostname): ftp.csc174.org
FTP Port: 21
FTP Username: lab02@csc174.org
FTP Password: [same password as lab01 - see Slack]
```

- When you FTP-in to the account, create a folder using the name of your **city-team** and place your website in there

## Submit the Lab

To get credit for your work:

- ONE of you must submit a link to your website in Blackboard, in: **GitHub Collaboration**
- Along with your link write in the **Write Submission** area (*not* the comments box):
  - **Your city-team name**
  - A list of **everyone's name** in your team (including your own)
  - A **link to your team's website** on the class web server
  - A **link to your team's repository** (which should be set to public)
