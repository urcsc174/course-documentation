# Project 1: Team “Flash” Website

*Due: Monday, July 6, 2020*

**The goal** of this project is to create a website using content from your *Initial Personal Website* (Lab 1), combined with two other students' lab 1s, and add a new index to act as a home page.

**The purpose** of this project demonstrate your ability to work as a team with defined roles to learn that it's possible to work more quickly and easily like this, with better results, compared to working alone.

*Note: in this exercise, the term "flash" does not refer to Adobe Flash; rather the idea of "sudden" ...meaning: this website should come together very quickly.*

## Establish a New Team

- Go to [our shared Google Sheet](https://docs.google.com/spreadsheets/d/1z0z8gNCR0_-zW18ft0YDoiLPn6z4OTuAM5P8jVIa7cg/edit#gid=0)  and **copy** (i.e. do *not* move) your name/email from the **Lab 2** city-teams to a *new* (different) city-team for **Project 1**
  - It doesn't matter what city you "move" to, but you need to pick what role you're going to be: 
    - Information Architect (IA),
    - Visual Designer, or
    - Technician (front-end only)
  - First come, first serve!  Not everyone will get their first choice - slots may fill-up before you get a chance to decide.
- When you have a team, follow the same steps from Lab 2: GitHub Collaboration to:
  - Create a private channel in Slack and invite the other members
  - If your city-team doesn't have a name yet (i.e. it still says "City-team #*n*") then decide amongst yourselves and name your city and update the Google Sheet

## Requirements

The final product of this assignment must meet the following requirements:

- The entire team must **use a GitHub repository**
  - **Technician:** setup the repo and make sure everyone can sync it to their desktop (using GitHub desktop software)
  - **Technician:** create four "stubs" - four empty HTML webpages with the proper HTML5 structure and no content.  (The IA will fill-in the content next.)

- Each one of the three students' initial personal websites from Lab 1 must be refactored into single webpages (four pages into one long scrolly page) and then combined to create a **three page website plus a new index page** (four webpages, total)
  - **IA:** organize the content into the webpage "stubs" created by the Technician
  - **IA:** ensure that the **document structure** (article, aside, whatever) is consistent on each student-page; and ensure that the **document outline** (h1, h2, et cetera) is *somewhat* consistent on each student-page ...note: it won't be, but you have to make it so!  
    - Take liberties with the content as you see fit.  
    - Note: if you're working with content that had an HTML form, you can throw that out.
  - **IA:** create some content for the new home page.  
    - You can fashion it like Project 3 from CSC 170 using snippets from the sub-pages to create "wells" (sections) with embedded links to the sub-pages ...or something like that.  It's up to you.

- There must be a new menu system
  - **IA:** code the navigation and make sure it works so you can go from page to page easily.  
    - Note: you don't have to install it in PHP Includes if the Technician didn't already set it up for you, and you don't have to style it nor make the current page highlighter work.
  - **IA:** there needs to be **links back to the original** Lab 1 websites in some appropriate place(s) ...you decide where
- There must a single look & feel for the entire website
  - **Visual Designer:** the entire website must have a single set of styles that make the website look unified and cohesive, like any normal website
    - Hint: you can pick and choose from any of the designs, or even "steal" a design from any other Lab 1 website ...it's up to you
    - Warning: have the **IA** work on setting up the document *structure* and document *outline* first; then even if they're still working on the content, you can start the design process when those things are (mostly) nailed down, or if the **IA** hasn't fleshed-out the content yet, you can use *lorem ipsum* content and *FPO*-images as needed that the IA can replace later.

- The HTML, CSS and JS code, files and file system must be clean and follow **industry best practices and standards** (note: "industry best practices" includes the use of PHP Includes as appropriate)
  - **Technician:** make sure the entire website works normally/correctly, and make sure all the HTML and CSS  pass W3C validation (within reason); also make sure the website is optimized and all file and folder names are correct. 

## Installation

- **Technician** must install the website on the class web server using the following web server credentials:

Note: each team will use the same FTP account. Be careful *not* to disturb other teams' files.

```
FTP Server (a.k.a. Hostname): ftp.csc174.org
FTP Port: 21
FTP Username: project1@csc174.org
FTP Password: [same]
```

- When you FTP-in to the account, create a folder using the name of your **city-team** and place your website in there

## Submit the Lab

To get credit for your work:

- ONE of you (typically the Technician) must submit a link to your website in Blackboard, in: **Project 1: Team “Flash” Website**
- Along with your link write in the **Write Submission** area (*not* the comments box):
  - **Your city-team name**
  - A list of **everyone's name** in your team (including your own), and...
  - Next to everyone's name **indicate everyone's role on the team** (IA, designer, or technician)
  - A **link to your team's website** on the class web server
  - A **link to your team's repository** (which should be set to public)
