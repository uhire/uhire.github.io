# Table of contents

* [Overview](#overview)
* [Developer Guide](#developer-guide)  
  * [Structure of Directory](#structure-of-directory)  
  * [Imports](#imports)  
  * [Naming Conventions](#naming-conventions)
  * [Data Model](#data-model)
  * [Style](#style)
  * [Authorization](#authorization)
  * [Configuration](#configuration)
  * [Coding Standards](#coding-standards)
* [Installation Steps](#installation-steps)
* [User Guide](#user-guide)
* [Development history](#development-history)
  * [Milestone 1: Mockup development](#milestone-1-mockup-development)
  * [Milestone 2: Update Functionality](#milestone-2-update-functionality)
  * [Milestone 3: Clean Up Pages](#milestone-3-clean-up-pages)
* [Community Feedback](#community-feedback)
  * [Kimo Nakata](#kimo-nakata)

# Overview

UHire is a Meteor application that provides company and student profiles. Based on the information provided companies can contact students to hire, or the students can view companies they are interested in and contact those companies as well. 
Here is the running page on Galaxy: [UHire](http://uhire.meteorapp.com/#/)

UHire is being developed by Dre Cardinalli, John Yap, Keoni Fontanilla, Kyle Okamoto, and Peter Newton.

# Developer Guide
## Structure of Directory
The very top level of the directory contains these files:  
<img src="/images/DirectoryStructureTopLevel.png">

The top level of the app contains these files:  
<img src="/images/DirectoryStructureApp.png">

## Imports
Imports are used to load the server and client contents. Only two files are invoking the main.js file and are in the server and client files. Here is an example of client\main.js which imports both, which contains the company and student collections, the client itself, and the style.css.  
<img src="/images/ImportExample.png">

Other imports are used as well throughout the components directory and the pages directory to incorporate the purpose of the application built.

## Naming Conventions
* Pascal Case was used as the naming convention of the JSX files. For example, StudentHome.jsx.  
* Camel Case was used as the naming convention for the naming of variables. For example, emailRegex.

## Data Model
The Uhire data model uses four different Javascript classes, [StudentCollection](https://github.com/uhire/uhire-app/blob/master/app/imports/api/stuff/student.js), [InterestCollection](https://github.com/uhire/uhire-app/blob/master/app/imports/api/stuff/interests.js), [CompanyCollection](https://github.com/uhire/uhire-app/blob/master/app/imports/api/company/company.js), and [PositionCollection](https://github.com/uhire/uhire-app/blob/master/app/imports/api/position/position.js). You can add a new item to each collection or you can get an item from each collection, depending on what kind of operation you want to do.

## Style
The style used for Uhire is the same style based on Semantic-UI CSS. The [CSS](https://github.com/uhire/uhire-app/blob/master/app/client/style.css) was used for every page generated in the application. The style we decided to implement was to put the nav-bar on the top followed by the contents of the body, while also leaving some color in the background, so the site isn't plain.

## Authorization
The landing page is public to all users, whether they have accounts or not. A user must sign up and login to gain access to either the student role or company role. The student role has access to the student home page, landing page, and browse company page. The company role has access to the company home page, landing page, and browse student page.

## Configuration
The [config](https://github.com/uhire/uhire-app/tree/master/config) directory is used for default data as well as some test data. When mongoDB is started these accounts are created.

## Coding Standards
The coding standard used for the development of the application was ESLint. This coding standard helps to create good coding habits and notifies users when certain things are missing. Go to this website to learn more about [ESLint](https://eslint.org/).

## Installation Steps
First, you can clone the app from Github [UHire](https://github.com/uhire/uhire-app) onto your Github Desktop app.
<img src="/images/GithubCloneDownolad.png">

If you do not already have Github desktop, you can download it here [Github Desktop](https://desktop.github.com/). 
<img src="/images/GithubDesktop.png">

You will then need to install [meteor](https://www.meteor.com/install) as well as [chocolately](https://chocolatey.org/install) by following the instructions provided on the website.
<img src="/images/MeteorDownload.png">
<img src="/images/ChocolatelyDownload.png">

After meteor and chocolately are installed on your system you are ready to start the app. You will need to cd into uhire-app/app like the example below.
<img src="/images/CommandPromptPath.png">

The following commands should be run to install required packages:

* meteor add aldeed:collection2@3.0.0
* meteor npm install --save simpl-schema
* meteor npm install --save google-map-react
* meteor add aldeed:schema-index





Once in the app you will invoke meteor npm run start to start the app.
The app is shown running at [http://localhost:3000/](http://localhost:3000/)
<img src="/images/RunStart.png">
<img src="/images/LocalHost.png">

The app can be modified using IntellijIdea. If you do not currently own IntellijIdea you can download it here [IntellijIdea](https://www.jetbrains.com/idea/download/#section=windows)
<img src="/images/IntelliJIdeaDownload.png">

The app is shown below in IntellijIdea.
<img src="/images/AppIntelliJIdea.png">

# User Guide
At this point the app should be running in your web browser.

### Landing Page
First is the landing page.On this page you can click on sign up, sign in or the logo. Clicking on these buttons will redirect you to sign up page, sign in page and the landing page respectively.
<img src="/images/LandingPage.png">

### Sign In Page
Next is the Sign In page. On this page you can sign in to your account if you already have an account or you can click the link on the bottom of the card to redirect you to the sign up page.
<img src="/images/FinalSignIn.png">

### Sign Up Page
The Sign up page allows you to fill out a form to create an account.
<img src="/images/FinalSignUp.png">

### Add Student Page
If you are a Student you will have access to the StudentHomePage and Company Search Page.
Before you can access those pages you will need to fill out a form for the StudentHome.
<img src="/images/FinalAddStudent.png">

### Browse Companies Page
The most important feature on this website is the search feature.
The student is able to search for companies and can filter by location and company name.
<img src="/images/CompanySearch.png">

### Student Home Page
On this page you can look at the information that you previously filled out in the form
<img src="/images/StudentHome.png">

If you are a Company you will have access to the CompanyHome Page and BrowseStudent Page.

### Add Company Page
Before you can access those pages you will need to fill out a form for the CompanyProfile.
<img src="/images/FinalAddCompany.png">

### Browse Student Page
On the BrowseStudent Page companies can look at all the student currently using uhire.
<img src="/images/FinalBrowseStudent.png">

### Company Home Page
On the CompanyHome Page you can look at the information that you provided on here, and edit the information as well.
<img src="/images/FinalCompanyHome.png">

### Add Position Page
The student and company can also add positions onto their profiles to inform others of what they are looking for.
<img src="/images/FinalAddPosition.png">

# Development History 

The development process for UHire conformed to [Issue Driven Project Management](http://courses.ics.hawaii.edu/ics314f16/modules/project-management/) practices. In a nutshell, development consists of a sequence of Milestones. Milestones consist of issues corresponding to 2-3 day tasks. GitHub projects are used to manage the processing of tasks during a milestone.  

## Milestone 1: Mockup development

Milestone 1 started on April 1, 2019 and is was finished on April 8, 2019.

The goal of Milestone 1 was to create a set of HTML pages providing a mockup of the pages in the system. To simplify things, the mockup was developed as a Meteor app. This meant that each page was a template and changed accordingly.
Mockups for the following four pages were implemented during M1:

Each issue was implemented in its own branch, and merged into master when completed.
Below each updated image of the MileStone1 Issues, are links to the corresponding page on galaxy.

Student Collection:
FirstName,LastName,Image,CurrentYear,CurrentOccupation,Interests,Location, Image

Company Collection:
Name,Location,Description,Contact Info, Image

Landing Page:
<img src="/images/LandingPage.png">
[LandingPage](http://uhire.meteorapp.com/#/)

Company Home:
<img src="/images/CompanyHome.png">
[CompanyHome](http://uhire.meteorapp.com/#/cohome)

Student Home:
<img src="/images/StudentHome.png">
[StudentHome](http://uhire.meteorapp.com/#/studentHome)

Admin Home:
<img src="/images/AdminHome.png">
[AdminHome](http://uhire.meteorapp.com/#/admin)

Footer:
<img src="/images/Footer1.png">

Nav Bar:
<img src="/images/LandingPage.png">

Company Profile:
<img src="/images/Company Profile.png">
[CompanyProfile](http://uhire.meteorapp.com/#/list)

Student Profile:
<img src="/images/StudentProfile.png">
[StudentProfile](http://uhire.meteorapp.com/#/sprofile)

Milestone 1 was implemented as [Milestone M1](https://github.com/uhire/uhire-app/milestone/1?closed=1):
<img src="/images/M1Project.png">

Milestone 1 consisted of 14 issues, and progress was managed via the [Uhire GitHub Project M1](https://github.com/uhire/uhire-app/projects/1):
<img src="/images/M1Closed.png">

## Milestone 2: Update Functionality
Link to [Milestone 2](https://github.com/uhire/uhire-app/projects/2)
Milestone 2 began on April 4, 2019 and was completed on April 21, 2019.
The goal of Milestone 2 is to update the functionality of the app. For example adding search functions, adding roles, and correcting the corresponding homepages.

We have successfully implemented the Browser function for both the company and student roles. We have also correctly redirected the corresponding homepages to student and company roles. 
The editing feature was added to the profile pages of company and student. 
The correct pages are being shown only to company roles or only to student roles.

Milestone 2 was implemented as [Milestone 2](https://github.com/uhire/uhire-app/milestone/2?closed=1):
<img src="/images/M2Project.png">

Milestone 2 consisted of 22 issues, and progress was managed via the [Uhire GitHub Project M2](https://github.com/uhire/uhire-app/projects/2):
<img src="/images/M2Closed.png">

## Milestone 3: Clean Up Pages
Link to [Milestone 3](https://github.com/uhire/uhire-app/milestone/3)
Milestone 3 began on April 22, 2019 and was completed on April 30, 2019.
The goal of Milestone 3 is to finalize any remaining issues as well as creating presentable pages by adding their own flare.
We have successfully corrected any previous errors from Milestone 2, improved form validation, and corrected the search functions.

Milestone 3 was implemented as [Milestone 3](https://github.com/uhire/uhire-app/milestone/3?closed=1):
<img src="/images/M3Project.png">

Milestone 3 consisted of 16 issues, and progress was managed via the [Uhire GitHub Project M3](https://github.com/uhire/uhire-app/projects/3):
<img src="/images/M3Closed.png">

# Community Feedback
To ensure that we are satisfying our customer's needs, we have requested responses from random customers and and asked their opinon on the concept, look, functionality and overall performance of our web application.  These are the summarized testimonies of our customers.

## Kimo Nakata
- I like how you can apply for the job right there.
- It's pretty cool that you can look at all the companies and isolate the ones you're interested in.
- The landing page looks pretty messy.  Too much going on.

## Fred Sanford
- Being able to see the location on the map is great.
...think of more











