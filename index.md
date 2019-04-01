# Table of contents

* [About uhire](#about-uhire)
* [Development history](#development-history)
  * [Milestone 1: Mockup development](#milestone-1-mockup-development)

# About uhire

BowFolios is a Meteor application providing portfolios for the University of Hawaii community. When you come to the site, you are greeted by the following landing page:

# Development History

The development process for BowFolios conformed to [Issue Driven Project Management](http://courses.ics.hawaii.edu/ics314f16/modules/project-management/) practices. In a nutshell, development consists of a sequence of Milestones. Milestones consist of issues corresponding to 2-3 day tasks. GitHub projects are used to manage the processing of tasks during a milestone.  

The following sections document the development history of BowFolios.

## Milestone 1: Mockup development

This milestone started on December 6, 2016 and ended on January 31, 2017.

The goal of Milestone 1 was to create a set of HTML pages providing a mockup of the pages in the system. To simplify things, the mockup was developed as a Meteor app. This meant that each page was a template and that FlowRouter was used to implement routing to the pages. 

Mockups for the following four pages were implemented during M1:

<img width="200px" src="images/landing.png"/>
<img width="200px" src="images/profile.png"/>
<img width="200px" src="images/directory.png"/>
<img width="200px" src="images/filter.png"/>

Milestone 1 was implemented as [BowFolio GitHub Milestone M1](https://github.com/bowfolios/bowfolios/milestone/1)::

![](images/m1-milestone.png)


Milestone 1 consisted of five issues, and progress was managed via the [BowFolio GitHub Project M1](https://github.com/bowfolios/bowfolios/projects/1):

![](images/m1-project.png)

Each issue was implemented in its own branch, and merged into master when completed:

![](images/m1-branch-graph.png)

## Milestone 2: Data model development 

This milestone started on Jan 31, 2017 and ended on Feb 2, 2017.

The goal of Milestone 2 was to implement the data model: the underlying set of Mongo Collections and the operations upon them that would support the BowFolio application.  We implemented the data model as a set of Javascript classes. The BaseCollection class provides common fields and operations. The ProfileCollection and InterestCollection classes inherit from BaseCollection and provide the persistent data structures useful for BowFolios. 
 
Also in this milestone, we implemented a set of mocha tests for the data model classes. These tests make sure we can create, manipulate, and delete the data model documents successfully.  These tests are documented above.

Milestone 2 was implemented as [BowFolio GitHub Milestone M2](https://github.com/bowfolios/bowfolios/milestone/2)::

![](images/m2-milestone.png)


Milestone 2 consisted of two issues, and progress was managed via the [BowFolio GitHub Project M2](https://github.com/bowfolios/bowfolios/projects/2):

![](images/m2-project.png)

Each issue was implemented in its own branch, and merged into master when completed:

![](images/m2-branch-graph.png)

## Milestone 3: Connect UI to data model

This milestone started on Feb 2, 2017 and ended on Feb 10, 2017.

The goal of Milestone 3 was to connect the user interface to the underlying data model. This meant that we updated the templates for each page with calls to helper functions, and we created Javascript files for the templates with helper functions. We used the form control templates from [meteor-example-form](https://ics-software-engineering.github.io/meteor-example-form/) to simplify implementation of form processing.

Milestone 3 was implemented as [BowFolio GitHub Milestone M3](https://github.com/bowfolios/bowfolios/milestone/3)::

![](images/m3-milestone.png)


Milestone 3 consisted of four issues, and progress was managed via the [BowFolio GitHub Project M3](https://github.com/bowfolios/bowfolios/projects/3):

![](images/m3-project.png)

Each issue was implemented in its own branch, and merged into master when completed:

![](images/m3-branch-graph.png)

## Milestone 4: Authentication

This milestone started on Feb 10, 2017 and ended on Feb 14, 2017.

The goal of Milestone 4 was to set up authentication using the University of Hawaii test CAS system. We used the templates from [meteor-example-uh-cas](http://ics-software-engineering.github.io/meteor-example-uh-cas/) to guide the implementation. Although the example restricts logins to those in a list in the configuration file, BowFolios allows anyone with a UH account to access the system. 

Authentication also implies that users cannot access the profile or filter page associated with another user.

Milestone 4 was implemented as [BowFolio GitHub Milestone M4](https://github.com/bowfolios/bowfolios/milestone/4)::

![](images/m4-milestone.png)


Milestone 4 consisted of two issues, and progress was managed via the [BowFolio GitHub Project M4](https://github.com/bowfolios/bowfolios/projects/4):

![](images/m4-project.png)

Each issue was implemented in its own branch, and merged into master when completed:

![](images/m4-branch-graph.png)

## Milestone 5: Administration

This milestone started on Feb 14, 2017 and is ongoing.

[BowFolio GitHub Milestone 5](https://github.com/bowfolios/bowfolios/milestone/5) involves the creation of an administrator role in the system. The administrator can manage the set of defined interests. (Currently, interests are defined in the database file loaded at system startup time.)

This milestone will also include the implementation of Meteor methods and removal of the insecure package. 

We will manage progress on this milestone using [BowFolio GitHub Project M5](https://github.com/bowfolios/bowfolios/projects/5).

# Walkthrough videos

BowFolios is intended as a model of how an ICS 314 project could be organized and executed. Here are some videos to walk through various aspects of the system and development process:

* [BowFolios: User Interface](https://www.youtube.com/watch?v=aZvxRQfQdkE)
* [BowFolios: Development Process](https://www.youtube.com/watch?v=8pTgFtbcjTc)
* [BowFolios: Application Structure](https://www.youtube.com/watch?v=_5g5CzZ0Toc)
* [BowFolios: Authentication and Authorization](https://www.youtube.com/watch?v=AaXShN8cYNY)
* [BowFolios: Initialization](https://www.youtube.com/watch?v=P3Kigb1gtVo)
* [BowFolios: Unit Testing](https://www.youtube.com/watch?v=EexZfw1yMJs)
* [BowFolios: Design Patterns](https://www.youtube.com/watch?v=yP-t44HBCPQ). Maybe watch [this](https://www.youtube.com/watch?v=Z2yjimK_MJU) first.










