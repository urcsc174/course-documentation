# Project 4: Data Entry Application

*Due: Monday, August 3, 2020*

**The goal** of this project is to start with an existing website (another team's Project 3) and...

- Power the student index page from Project 3 (the F-pattern page) with a **backend database** to display the student information
- Create a **new front-end web form** on a new webpage to add records to that database (and update and delete records)
- Style the front-end web form using a **CSS Framework**

**The purpose** of this project is to work as a team to practice new skills: building a web application that has both a front-end and a back-end, and integrating it into an existing website

## Establish a New City-Team

For this project, not only do you need to choose a new city-team in which to work, you need to chose your role: **IA**, **Visual Designer**, **Technician**.

Be advised, the roles will involve the following responsibilities:

- The **Information Architect** will need to figure out how and where to include the new data-entry web page, and exactly what content is needed to explain it (headings, prompts, labels ...everything to explain what the user needs to know); the IA will also need to code the HTML form on the new data-entry web-page (although the Technician is tasked to make it valid and make it work).  The HTML form will need to allow the user to create, view (read) update,  and delete records (CRUD)

- The **Visual Designer** must take direction from the IA and apply styles to the new data-entry web page using a CSS Framework of their choice, *plus* custom styles to make the new web page look like it belongs to the website from a stylistic standpoint.  Also, since the existing student index page (the F-pattern) will be altered, the Visual Designer must make sure it still looks like it did originally in Project 3.

- The **Technician** will be working from both a front-end and back-end perspective to create a database and table on the class web server to hold the student index information, and then install the PHP scripts to...

  - **Input to the database:** the new data-entry webpage (designed by the IA and styled by the Visual Designer) will take the web form and populate the database table on the server with the entered data; the web form will allow the user to all four CRUD functions
  - **Display content from the database:** the existing student index page (the F-pattern) will pull content from the class web server and display it in an F-pattern

  Also, the technician is responsible for installing the finished website on the class web server, and the technical quality of the entire website.

## Requirements

- Go to [our shared Google Sheet](https://docs.google.com/spreadsheets/d/1z0z8gNCR0_-zW18ft0YDoiLPn6z4OTuAM5P8jVIa7cg/edit#gid=0)  and **copy** (do *not* move) your name/email from the **Project 3** city-teams to a *new* (different) city-team for **Project 4**
  - Your Project 4 city must be different than your Project 3 city
- Then, establish contact with your new City-Team
  - When you have a team, follow the same steps as before to create a *new* private channel in Slack and invite the other members

### NEW: Changes to the Student Index Page

*Keeping in mind that CSC 174 is a **Front-end** Web Course, we do not want to belabor the Technician's responsibilities with the back-end database.  So...*

- It is acceptable to *not* replicate the photos on the Student Index webpage

  - Doing so would require the Technician to figure out how to upload image files from the HTML form to the database, and then download them dynamically to display in the Student Index page

  - It is possible to implement the photos anyway using one of two methods: 

    - BLOBs in the database (not the industry standard) or 
    - File-pointer references (recommended but could be tricky) in the web server's file system 

    ...which would be GREAT if the Technician could do that!  But if the Technician does not want to spend the time implementing that, that's okay

- If the Technician choses to *not* implement the photos for the Student Index page, then the team must replace that element with something else

  - The existing ontology requires: (1) name; (2) photo; (3) excerpt; and (4) link to student page ...which can be changed to something/anything else.  
  - Suggestion: (1) name; (2) <s>photo</s> **favorite quote**; (3) excerpt; and (4) link to student page

  ...which would require someone (preferably the IA) getting the new content.

### Roles and Recommended Steps

1. **Technician:** use the city-team's repository created for their Project 3 as a basis for Project 4
   - Set-up the new repository and make sure everyone in the team is added as contributor and can sync it to their localhost on their desktop using the GitHub desktop software
   - Create the new database and table on the class web server, and share the database credentials with the team (host name, user name, password, and database name)

2. **Information Architect:** plan the new webpage that will capture user input to fill the database that will be used to fill the student index page 
   - When designing the HTML form, the IA needs to consider the **ontology** of the website - what's being captured and how it will be used; (don't over-think this part - hint: this part should be easy; you're just populating the data on the student index page)
   - Also, the IA needs to explain to the user what's going on - *why* they need to fill-out the HTML form; and *how* to fill out the form; are any of the field "required?" ...consider the **taxonomy** of the website, especially when considering the form's labels and legend(s), and any other text anywhere around the form
   - In addition to the HTML form itself and the order in which the fields are presented, the IA needs to consider the **choreography**: how does the user get to this new web page?  What happens after they click the submit button?  

3. **Visual Designer:** take direction from the IA and style the new webpage using a CSS Framework of your choosing, and then customize it (override it) to make it look like it belongs to the same website, visually
   - When styling the new data entry web page, the Visual Designer needs to use the framework to support **all the principles of design** (BTW - if you use the framework correctly, you'll find this is a lot easier!  ...it's one of the benefits of using frameworks)
   - Choices the Visual Designer makes to customize the new web page must not compromise (lessen) any of the principles of design
   - The Visual Designer is also responsible for the visual presentation of the entire website.  Any changes/additions anywhere must adhere to the principles of design, as much as possible

## Installation

- Use the following web server credentials (typically done by the technician):

Note: each team will use the same FTP account. Be careful *not* to disturb other teams' files.

```
FTP Server (a.k.a. Hostname): ftp.csc174.org
FTP Port: 21
FTP Username: project4@csc174.org
FTP Password: [same]
```

*Notice above: it's "4" in the username this time*

- When you FTP-in to the account, create a folder using the name of your **city-team** and place your website in there

## Submit the Lab

*NOTE: this is different! Everyone will be graded as individuals for Project 4.  Therefore everyone must make a submission in Blackboard to be graded.*

To get credit for your work:

- EVERYONE must submit a link to your website in Blackboard, in: **Project 4: Data Entry Application**
- Along with your link write in the **Write Submission** area (*not* the comments box):
  - **Your city-team name**
  - A list of **everyone's name** in your team (including your own) AND everyone's role
  - A **link to your team's website** on the class web server
  - A **link to your team's repository** (which should be set to public)
