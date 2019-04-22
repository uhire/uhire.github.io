# Table of contents

* [Overview](#overview)
* [Development history](#development-history)
* [Developer guide](#developer-guide)
* [User Guide](#User-guide)
* [Milestone 1: Mockup development](#milestone-1-mockup-development)
* [Milestone 2: Update Functionality](#milestone-2-update-functionality)

# Overview

UHire is a Meteor application that provides company and student profiles. Based on the information provided companies can contact students to hire, or the students can view companies they are interested in and contact those companies as well. 

# Development History 

The development process for UHire conformed to [Issue Driven Project Management](http://courses.ics.hawaii.edu/ics314f16/modules/project-management/) practices. In a nutshell, development consists of a sequence of Milestones. Milestones consist of issues corresponding to 2-3 day tasks. GitHub projects are used to manage the processing of tasks during a milestone.  

UHire is being developed by Dre Cardinalli, John Yap, Keoni Fontanilla, Kyle Okamoto, and Peter Newton.

# Developer Guide
First, you can clone the app from Github [UHire](https://github.com/uhire/uhire-app) onto your Github Desktop app.
<img src="/images/GithubCloneDownolad.png">

If you do not already have Github desktop, you can download it here [Github Desktop](https://desktop.github.com/). 
<img src="/images/GithubDesktop.png">

You will then need to install [meteor](https://www.meteor.com/install) as well as [chocolately](https://chocolatey.org/install) by following the instructions provided on the website.
<img src="/images/MeteorDownload.png">
<img src="/images/ChocolatelyDownload.png">

After meteor and chocolately are installed on your system you are ready to start the app. You will need to cd into uhire-app/app like the example below.
<img src="/images/CommandPromptPath.png">

Once in the app you will invoke meteor npm run start to start the app.
The app is shown running at [http://localhost:3000/](http://localhost:3000/)
<img src="/images/RunStart.png">
<img src="/images/LocalHost.png">

The app can be modified using IntellijIdea. If you do not currently own IntellijIdea you can download it here [IntellijIdea](https://www.jetbrains.com/idea/download/#section=windows)
<img src="/images/IntelliJIdeaDownload.png">

The app is shown below in IntellijIdea.
<img src="/images/AppIntelliJIdea.png">

#User Guide
At this point the app should be running in your web browser.

First is the landing page.On this page you can click on sign up, sign in or the logo. Clicking on these buttons will redirect you to sign up page, sign in page and the landing page respectively.
<img src="/images/LandingPage.png">

Next is the Sign In page. On this page you can sign in to your account if you already have an account or you can click the link on the bottom of the card to redirect you to the sign up page.
<img src="/images/LoginV2.png">

The Sign up page allows you to fill out a form to create an account.
<img src="/images/SignUpV2.png">

If you are a Student you will have access to the StudentHomePage,BrowseCompany Page, and StudentProfile Page.
Before you can access those pages you will need to fill out a form for the StudentProfile.
<img src="/images/StudentInfo.png">

On the BrowseCompany Page, a student can look for companies that they are interested in.
<img src="/images/BrowseCompany.png">

All the information provided on the previous form will be put into a card on the StudentProfile Page. The information here can also be edited.
<img src="/images/StudentProfile.png">

If you are a Company you will have access to the CompanyHome Page, BrowseStudent Page, and CompanyProfile Page.
Before you can access those pages you will need to fill out a form for the CompanyProfile.
<img src="/images/CompanyInfo.png">

On the BrowseStudent Page companies can look at all the student currently using uhire.
<img src="/images/BrowserStudent.png">

On the CompanyProfile Page you can look at the information that you provided on here, and edit the information as well.
<img src="/images/CompanyProfile.png">

The student and company can also add positions onto their profiles to inform others of what they are looking for.
<img src="/images/AddPosition.png">

## Milestone 1: Mockup development

This milestone started on April 1, 2019 and is was finished on April 8, 2019.

The goal of Milestone 1 was to create a set of HTML pages providing a mockup of the pages in the system. To simplify things, the mockup was developed as a Meteor app. This meant that each page was a template and changed accordingly.
Mockups for the following four pages were implemented during M1:

Milestone 1 was implemented as [UHire GitHub Milestone M1](https://github.com/uhire/uhire-app/projects/1)::

Milestone 1 consisted of fourteen issues, and progress was managed via the [uhire GitHub Project M1]

Each issue was implemented in its own branch, and merged into master when completed.
Here is the running page on Galaxy: [UHire](http://uhire.meteorapp.com/#/)
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

## Milestone 2: Update Functionality
Link to [Milestone 2](https://github.com/uhire/uhire-app/projects/2)
Milestone 2 consisted of 22 issues, began on April 4, 2019 and was completed on April 21, 2019.
The goal of Milestone 2 is to update the functionality of the app. For example adding search functions, adding roles, and correcting the corresponding homepages.

We have successfully implemented the Browser function for both the company and student roles. We have also correctly redirected the corresponding homepages to student and company roles. The editing feature was added to the profile pages of company and student. The correct pages are being shown only to company roles or only to student roles.

## Milestone 3: Clean Up Pages
Link to [Milestone 3](https://github.com/uhire/uhire-app/milestone/3)
Milestone 3 consists of 9 issues, began on April 22, 2019 and is currently in progress.
The goal of Milestone 3 is to finalize any remaining issues as well as creating presentable pages by adding their own flare.







