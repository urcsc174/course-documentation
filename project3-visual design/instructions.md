# Project 3: Visual Design

*Due: Wednesday, July 22, 2020 ...extra time!*

**The goal** of this project is to apply the full-set of page design principles to a forked version of another team's Project 2 website; the new website will have:

- A new home page that uses a Z-pattern design (replaces the original index)
- A new secondary page that uses an F-pattern design (acts like an index, but isn't an index.html file per se); it'll act as a gateway to the rest of the website
- A set of student webpages from Project 2

**The purpose** of this project is to demonstrate your understanding of:

- CRAP Principles (from Part 1)
- Z-patterns and F-patterns (from Part 2)
- Principles of Legibility, Readability, and Typography (from Part 3)

...as it applies to websites, while working in a team of Visual Designers

## Establish a New City-Team

For this project, everyone will be a Visual Designer in a new city-team, working on a "forked" copy of one of the **Project 2** websites.

*Note: just like with IAs, it is common in very large organizations working on very large websites to have a team of Visual Designers (or whatever they call them); there is usually one designer with the most experience who acts as the team lead; the rest are junior designers - but in our case, your team just needs to try to work well together; none of you are "in charge" per se.*

- Go to [our shared Google Sheet](https://docs.google.com/spreadsheets/d/1z0z8gNCR0_-zW18ft0YDoiLPn6z4OTuAM5P8jVIa7cg/edit#gid=0)  and **copy** (do *not* move) your name/email from the **Project 2** city-teams to a *new* (different) city-team for **Project 3**
  - Note: *do not decide too fast*!  There is criteria below (Choosing a New City-Team) that you should know about before deciding where to move

- Then, establish contact with your new City-Team
  - When you have a team, follow the same steps as before to create a *new* private channel in Slack and invite the other members

### Choosing a New City-Team

The requirements for this project will have you and your new teammates come-up with a new visual design, **based on its existing design***.  So, things to consider...

- Your Project 3 city must be different than your Project 2 city
- When you move to a new city, you will use that team's repository that they created for their Project 2
- When you choose a new city-team keep in mind: its Project 2 website has to have a design that you think you can *improve* by applying the *principles of page design* (parts 1, 2, and 3)
- Hint: a website that looks like you can make a lot of improvements will be a better choice!  

** Side note: my original intent for Project 3 was to have you throw-out the CSS from Project 2 and use the comps from Lab 7 to guide the creation of a new design.  However, since just about everyone created "wireframes" instead of comps for Lab 7, I am re-writing this Project to have you use the existing CSS from Project 2 as a basis for it's new design.  So consider the submitted drawings from Lab 7: wireframes after all.* :man_shrugging:

## "Fork" the Repository

- The team must use a new GitHub repository, based on a "forked" version of the previous team's Project 2 repository
  - For this next step someone on your team must **fork the website in the repo** that the previous team used.  (See the link in [the shared Google Sheet](https://docs.google.com/spreadsheets/d/1z0z8gNCR0_-zW18ft0YDoiLPn6z4OTuAM5P8jVIa7cg/edit#gid=0) to find the previous team's Project 2.)  
  - It doesn't really matter who does what, however it would be helpful for someone who was *not* a Technician previously to do it this time ...so more people can get more experience.
  - Whoever sets-up the new repository, make sure everyone in your team is added as contributor and can sync it to their localhost on their desktop using the GitHub desktop software

## Suggested Workflow

As a team...

- **Search the #lab6-critiques** channel in Slack for critiques that refer to the design you have chosen
  - Reminder: Lab 6 was all about the C.R.A.P principles
  - If any critiques for your website exist, read and consider them for improvements you might make in Project 3
  - You are not required implement the Lab 6 critiques (they're not all great) but some of them might be a good idea

- **Pick approved Z-pattern and F-pattern** <s>comps</s> ...erm, ***wireframes*** from the #lab7-page-layout channel in Slack
  - You can pick any ...doesn't have to be your own; and you can mix and match F- and Z- patterns
  - Hint: look for ones that look like they fulfill the requirements from Lab 7 very well and is *implementable*
  - Note: you will be graded on how well you replicate the wireframes you chose
  - Note: although the Lab 7 F-patterns can be used for 21 line items (students) for Project 3 you will use it for three items (students) only ...not the entire class *this time*

- **Review ALL the possible principles of page design (parts 1, 2, and 3)** and make notes about all the opportunities to make improvements
  - This is important because it'll help your team work better as a team if you know what you're doing before everyone starts
  - Also, you'll need to document all the design improvements you make, so start writing things down here, during the planning phase
- Working as a team, **divide-up the planned improvements** and work toward implementation
  - Keep in mind the following requirements (next section, below) that should be divvied up among the team also

## Requirements

- Your team will be graded on:
  - Implementation of a **Z-pattern** as the new homepage as defined by the wireframe chosen
  - Implementation of an **F-pattern** as a secondary page as defined by the wireframe chosen
  - Use of **CRAP principles** everywhere (five webpages total)
  - Use of the 10 **principles for readability**, everywhere
  - Good choices for **typography** including **well-paired typefaces** (fonts)
  - Use of the **Rule of Thirds** and/or the **Golden Ratio** throughout the website
- Document all the design improvements in a **readme.md**
  - Include at the top of the readme:
    - Your city-team's name
    - Everyone's name
  -  Note: do *not* make a terribly long and detailed document about your design improvements; just a list of what and where was changed AND the design principle that was applied

- You have to **use the existing CSS** from the previous city-team's Project 2 as a basis for your Project 3
  - Although there should be lots of improvements to the design, the website should look *mostly* like the Project 2 from whence it came ...or at least somewhat recognizable
- You need to implement a **CSS Architecture**
  - It doesn't have to be a SMACSS architecture ...actually, a variant of it will probably work well; decide amongst yourselves
  - Although you have to use the previous teams' CSS styles as a basis for your Project 3, you can re-name and re-factor all their styles so they fit better into an architecture that wasn't there before (just be careful and go slow at this point! ...renaming styles is tricky business)
  - BTW, if you do this part well, you will realize the benefit of CSS architecture as you're all working on the same set of files in your repository at once; the CSS groupings you create *should* help minimize Git conflicts
- Although the goal of any designer is to ***not* make changes to the existing content in HTML**, but it happens - that's okay; just try to minimize that
  - Obviously, you'll need to add/change/rename use of classes (or maybe IDs) in the HTML as you see fit
  - You may need to add DIVs or SPANs if the HTML elements don't exist in places you need them (but always try to use the HTML elements that are there, first)
- It's assumed that the document structure and the document outline from the previous city-team's Project 2 is perfect ...but, it might not be! You are required to **fix any mistakes you inherited** from the Project 2 ...else you may lose points for them too!

## Other Considerations

Just to be clear about a few things:

- Project 3 will have five webpages
  - A homepage (Z-pattern)
  - A student list (F-pattern)
  - Three student pages that uses any appropriate layout
- You will throwing-out the original index page from Project 2, however you can re-purpose the content (in an obvious place!)
- Navigation for this website is very simple:
  - Need only one link to go from the homepage (Z-pattern) to the student list (F-pattern)
  - There needs to be a link on the student list (F-pattern) to get back to the homepage (Z-pattern)
  - The student list (F-pattern) does not need another navigation element to get to all the student pages; the links in the F-pattern will suffice
  - The three student pages need links to get back to the student list (F-pattern) and the homepage (Z-pattern); 
  - Optional (if you think it makes sense for your design): there can be links on each student page to go directly to the other student pages
- Remember the Technician's responsibilities! Although none of you will be identified as the Technician for the team, it is expected you will pull together as a team and watch out for all the things that all CSC 170 students know including:
  - Someone has to upload the final website from a repo to the class web server
    - Make sure ONLY the files of the website are on the web server (no .md files among other things!)
  - Someone has to do a quality control check to make sure everything works
    - Make sure each page passes HTML and CSS validation, within reason
    - Make sure there are no error_log files (indicating a PHP error) generated by the web server sitting in any of the directories
    - Make sure all the file and folder names meet industry best practices (meaningful names, all lowercase, no spaces)
    - Make sure PHP Include files are used appropriately
    - ...and the list goes on; basically, everything you learned in CSC 170
  - Someone has to turn-in the final links (website and repo) in Blackboard on behalf of the team

## Installation

- Whoever does the installation on the class web server, use the following web server credentials:

Note: each team will use the same FTP account. Be careful *not* to disturb other teams' files.

```
FTP Server (a.k.a. Hostname): ftp.csc174.org
FTP Port: 21
FTP Username: project3@csc174.org
FTP Password: [same]
```

*Notice above: it's "3" in the username this time*

- When you FTP-in to the account, create a folder using the name of your **city-team** and place your website in there

## Submit the Lab

To get credit for your work:

- One of you must submit a link to your website in Blackboard, in: **Project 3: Visual Design**
- Along with your link write in the **Write Submission** area (*not* the comments box):
  - **Your city-team name**
  - A list of **everyone's name** in your team (including your own)
  - A **link to your team's website** on the class web server
  - A **link to your team's repository** (which should be set to public)
