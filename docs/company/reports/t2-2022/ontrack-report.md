## Product Overview

## OnTrack

OnTrack is a platform designed to facilitate student learning by helping them achieve their unit
learning outcomes and goals. It reduces pressure on achieving unrealistic grades, and importance on
tailored content learning using tasks and a portfolio assessment. This approach provides students
with a simple but effective way to demonstrate their achievements and learning outcomes with the
assistance of teaching staff feedback throughout the unit. OnTrack is based on Doubtfire LMS and
Thoth Tech is working towards creating new and enhanced features that improve the teaching and
learning experience.

**Product Leads:** Shaine Christmas, Matthew Fletcher

### Voice Verification

#### Overview, Goals, and Objectives

Due to the rise in contract cheating, audio submissions to the OnTrack system need to be reviewed in
order to ensure that the Speaker within the submission is the student to be submitting the work. The
long term goal of this project is to implement a Voice Verification system into OnTrack Audio
submissions. This will allow assessors to identify cheating where possible, and to discourage
students from submitting work that is not their own.

#### Aims for Trimester

The Aims for this Trimester are:

- To Test the system for a range of different audio files with multiple speakers
- Implement the Voice Verification container into the OnTrack API

#### Deliverables

Short Term:

- Test how the system responds to audio submissions with multiple different speakers
- Integration of the Voice Verification API into the OnTrack API
- Documentation of implementing the Voice Verification container into the existing OnTrack API
- Working validation of voices through a local distribution of the OnTrack API

Long Term:

- Full implementation, Testing and Documentation of Voice Verification system within the existing
  OnTrack System.

#### Project Mid-Trimester Progress

Currently Completed Tasks:

- Local distribution of OnTrack running
- Voice Verification Container Tested
- Voice Verification API currently being tested

#### Project End-Trimester Progress

Completed Tasks:

- Local distribution of OnTrack running
- Voice Verification Container Tested
- Voice Verification Design Document
- Creation of Voice Verification Handover Document
- Creation of Audio System Interface Design Document
- Testing of Voice Verification API


#### Project Members (10)

_Delivery Representative:_ md fahim mizi

_Software Developers:_md fahim mizi 

OnTrack Overview
Author Information
Author(s):
Team:
Team (Delivery and/or Product) Lead:
Document Summary
Documentation Title:
Documentation Type: { Informative/Technical }
Documentation Information Summary:
Document Review Information
Date of Original Document Submission to GitHub:
Documentation Version:
Date of Previous Documentation Review:
Date of Next Documentation Review
Key Terms
Enter Key Terms here

Key Links/Resources
Enter Key Links/Resources here

Contacts for further information
Enter Contacts here

Related Documents
Enter Related Documents here

Introduction
Members of the OnTrack project concentrate on OnTrack, a Learning Management System (LMS) used by Deakin University, and its development and upkeep. A web program called OnTrack makes it easier to give students sign in and authenticate their credentials. It also supports students through task engagement.

The OnTrack team has been tasked with developing additional features to improve users experience for easy usability.

OnTrack is made up of several codebases for the front end and the back end, as well as a project for documentation:

Ruby on Rails was used to build the OnTrack API's back end.
Built on Angular/AngularJS, Doubtfire-front web's end.
DoubtFire project documentation can be found at doubtfire.io.
The OnTrack team worked on adding numerous new features and improvements to OnTrack throughout:

Implementations

Check passwords
Reset OnTrack password
Documentation updates on OnTrack
README.md file
Written Down/Partially Carried Out

Improvements to the admin panel and the portfolio
This document will explain each of those above, including references to pertinent artefacts.

Document Objectives
This document is a transfer log for all the data and materials generated this trimester. The following items are included in the delivery package and handover document:

The product owner was shown the initial feature docs or proposals that describe each item to be introduced.

Files > Docs > OnTrack > Deployment > Software Requirements Specifications Check Passwords Document

Files > Documents > OnTrack>Deployment> Software Requirements Specifications Reset Ontrack password Document

Updates to the documentation can be found under Files > OnTrack>Documentation.

Iteration retrospectives are presentations that offer an overview of the Ontrack development at the end of iterations 1 and 2.

Initial Presentation Iteration.

Presentation for iteration two.

The Ontrack repository can be found at https://github.com/thoth-tech/documentation

There are pull requests for each feature, along with modifications' examples.

Long and Short Term Deliverables
Description	Issues	Contributors	Iteration
Check passwords: With the use of this function, DoubtFire groups may verify that their passwords are correct and make any necessary modifications. Back-end pull request Front-end pull request	Validating password in a secure manner		Documented iteration 1
Reset Ontrack password: Users cannot now reset their passwords after entering them into the system. This feature intends to add a different value to allow users to reset their password if they forget their original one. Back-end pull request Front-end pull request	It was understanding the various API endpoints that rely on the current "without reset password" value and where it has to be changed to "Reset password" might be challenging.		Documented iteration 1
Documentation updates on Ontrack: This feature enables the DoubtFire update icon to allow users to access new releases and updates for simple system functions. These will enable them to use the system effectively and become accustomed to the latest upgrades.Front-end pull request	The code had to be converted from Angular JS to Angular. The system update logic needed to be fixed because it was flawed.		Documented iteration 2
Readme file: This document aims to explain how to build up a working installation of Doubtfire on Windows using the Windows Subsystem for Linux (WSL). This document also includes instructions on how to alter the codebase correctly (using Visual Studio Code) so that there are no filesystem conflicts between Windows and Linux. Pull request	The "step-x" pages automatically use a different template exclusive to step pages. A fix was necessary to guarantee that the "Step 1 of 4" title was generated appropriately.		Documented iteration 1
Planned Work
Description	Issues	Contributors	Iteration
Open problems
Currently, the team only has one unresolved issue, which relates to a planned feature:

As seen in the admin and portfolio enhancements feature document, the team is unsure how the admin and portfolio enhancements feature will be implemented on the back end.

Lessons Learned
As an OnTrack team, one crucial lesson we discovered was the importance of experimenting with the Doubtfire environment on your own local computer. Instead than reading Ruby, Rails, or Angular tutorial after tutorial, working on a project is the greatest way to learn.

The project customer should be contacted more frequently so they may offer greater guidance on the project. A larger backlog needs to be formed for choosing which activities to do.

Product's High-Level Architecture
The components of the web application DoubtFire are as follows:

Ruby on Rails' web framework, the Grape REST API development framework, and a backend (API) written in Ruby. The backend uses the Ruby on Rails Active Record ORM to interacting with a database (PostgreSQL for development and MySQL for production). Active Record migrations are used to control the database schema (Soni, 2017).

A frontend currently primarily written in AngularJS and CoffeeScript is being upgraded to use Angular and TypeScript (Toal, Rivera, Schneider, & Eileen, 2016).

User manual
Since Doubtfire is an established platform, there isn't a handbook available to help users access the front and back ends of the site. The readme file provided above may be a helpful starting guide; it will act as the foundation for Doubtfire's development ("Doubtfire-api/CONTRIBUTING.md at development · doubtfire-LMS/doubtfire-api”)

XML
Here is a very basic XML sitemap that includes the location of a single URL:

<?xml version="1.0" encoding="UTF-8"?> 
<urlset xmlns="http://www.sitemaps.org/schemas/sitemap/0.9"> 
    <url> 
        <loc>http://www.example.com/foo.html</loc> 
        <lastmod>2018-06-04</lastmod> 
    </url> 
</urlset>
Encode your file using UTF-8 encoding.

Don't put anything other than URLs in the sitemap file.

You can name the text file anything you wish, provided it has a .txt extension (for instance, sitemap.txt).

General Sitemap Guidelines
Use consistent, fully-qualified URLs. Google will crawl your URLs exactly as listed. For instance, if your site is at https://www.example.com/, don't specify a URL as https://example.com/ (missing www) or ./mypage.html (a relative URL).

A sitemap can be posted anywhere on your site, but a sitemap affects only descendants of the parent directory. Therefore, a sitemap posted at the site root can affect all files on the site, which is where we recommend posting your sitemaps.

Don't include session IDs from URLs in your sitemap. This reduces duplicate crawling of those URLs.

Tell Google about alternate language versions of a URL using hreflang annotations.

Sitemap files must be UTF-8 encoded, and URLs escaped appropriately.

Break up large sitemaps into smaller sitemaps: a sitemap can contain up to 50,000 URLs and must not exceed 50MB uncompressed. Use a sitemap index file to list all the individual sitemaps and submit this single file to Google rather than submitting individual sitemaps.

List only canonical URLs in your sitemaps. If you have two versions of a page, list in the sitemap only the one you prefer to appear in search results. If you have two versions of your site (for example, www and non-www), decide which is your preferred site, and put the sitemap there, and add rel=canonical or redirects on the other site.

If you have different URLs for mobile and desktop versions of a page, we recommend pointing to only one version in a sitemap. However, if you want to point to both URLs, annotate your URLs to indicate the desktop and mobile versions.

Use sitemap extensions for pointing to additional media types such as video, images, and news.

If you have alternate pages for different languages or regions, you can use hreflang in either a sitemap or html tags to indicate the alternate URLs.

Non-alphanumeric and non-latin characters. We require your sitemap file to be UTF-8 encoded (you can generally do this when you save the file). As with all XML files, any data values (including URLs) must use entity escape codes for the characters listed in the following table. A sitemap can contain only ASCII characters; it can't contain extended ASCII characters or certain control codes or special characters such as * and {}. If your sitemap URL contains these characters, you'll receive an error when you try to add it.

OnTrack-deploy Analysis
Current State:

Readme file is Incomplete and needs updates. A lot of information is missing about the repository an API integration and functionalities.

Almost all the sub directory’s markdown files are empty or lack proper readability.

Contributing.md is complete and has great amount of information for individuals looking to contribute to doubtfire-deploy.

Changelog.md is up to date and all of the functionalities are current and recent. However, the file is missing a header.

Docker connection files are within the root of the repository.

All the links are opening to external pages from the same window, limiting readability and flow.

Quality assurance files are missing.

Problem Statement
As a documentation team member, Our report will focus on a solution based on the analysis and we want to document everything on Doubtfire-deploy repository.

There is incomplete documentation of the Doubtfire-deploy repository that is rising empty links within readme file, poor contributing.md formatting, empty markdown files within multiple sub-folders, missing header on CHANGELOG.md, missing Quality Assurance files and documentation links opening from within the same tab, limiting fluent readability.

Proposed solution

Producing a report that is efficient and effective on Doubtfire-deploy repository basing on the:

Review and update readme.md file updating each link and exhaustively review every user guide within the file, keeping in mind the versions.
Review all the .md user manuals within each subdirectory, to ensure they are not just present, but contain meaningful information they are intended for.

Improve the CHANGELOG.md file header and outlook.

Add quality assurance files within the repository.

Format all hyperlinks to load on a new tab.

Scope
Analysis of OnTrack Deploy

Definition of success
Implementation can be straight away and fix things to solve the problem immediately

OnTrack-Web Analysis
Problem Statement
To analyse and record the current state of documentation in the Wodoubtfire-web repo from this report work we can make recommendations for documentation solutions. To create an overview of each repo (Wodoubtfire-web and doubtfire deploy) so I can understand what each file and folder does.

There is incomplete documentation of the wodoubtfire-web repository that is arising from empty links within readme file, poor and in complete contributing.md file and its formatting, missing Quality Assurance files and documentation links opening from within the same tab, limiting fluent readability.

Current state as per the analysis tabulated
Readme file is complete but needs a lot of updates and correction. It has a lot of valuable information about the

MIGRAION_GUIDE.md is present and has valuable details for both upgrade and reverting.

Contributing.md is incomplete and lacks great amount of information useful to developers willing to contribute to this repository.

Changelog.md is present, complete correct and up to date but has a poor formatting and lacks a headers.

Docker connection files are within the root of the repository.

All the links are opening to external pages from the same window, limiting readability and flow.

Quality assurance files are missing.

Problem Statement
To analyse and record the current state of documentation in the Wodoubtfire-web repo from this report work we can make recommendations for documentation solutions.

There is incomplete documentation of the wodoubtfire-web repository that is arising from empty links within readme file, poor and in complete contributing.md file and its formatting, missing Quality Assurance files and documentation links opening from within the same tab, limiting fluent readability.

Proposed solution
The solution will ensure smooth recording details in the Analysis document in line with the existing template. The analysis is appropriately detailed so that a report can be produced and documentation solutions can be recommended.

It will as well:

Remove the Migration files and histories form the readme.md file and properly format the readme file.

Review all the .md user manuals within each subdirectory, to ensure they aren’t just present, but contain meaningful information they are intended for.

Improve the CHANGELOG.md file header and outlook.

Add quality assurance files within the repository.

Expectation
The analysis makes it quick and easy for the report to be produced

Automatic production of Documentation and Recommendation using the template

Ensuring template reuse by other schooler, researchers and UX experts

Challenges
Time consuming analysing every single file in the repo

#### Project Members (6)

_Delivery Representative:_ Shaine Christmas

_Software Developers:_ Ha Nguyen, Devin Oshada Uvin Jayasinghe, Daniel Le, Simon Agahi, Jesse Kyle
Hancock

### Task and Submission Redesign

#### Overview, Goals, and Objectives

The objective of this project is to redesign the task view and submission process for students. This
project should empower students, connecting them with tutors and facilitating personalised learning
experiences. Our goal is creating UI and software designs for a "next generation" update to tasks in
OnTrack. The project effects all users of OnTrack, mostly affecting student viewing of tasks.
Additionally, the project affects how submission is handled for students and assessors.

#### Aims for Trimester

The aims for this trimester are:

- Production of UI/UX design process for the task view and submission process of students.
- Begin the build and Integration of final design.

#### Deliverables

Short Term:

- Documentation Epic and User stories.
- Develop and deliver 4 wire frames.
- Develop and deliver 2 visual designs.

Long Term:

- Develop and deliver a final UI/UX design.
- Code review of final design
- Build and implementation of final design into OnTrack

#### Project Mid-Trimester Progress

Currently Completed Tasks:

- Creation of OnTrack User Flow map
- Creation of first Iteration Wire frames
- Creation of Project Epic and User Stories
- Development of Proof of Concept for upload and chat history log feature

#### Project End-Trimester Progress

Completed Tasks:

- Documentation of Project
- Completion of Iteration 3 wire frames
- Coded example of time-based log back-end functioning

#### Project Members (4)

_Delivery Representative:_ Grady Ramsay

_Software Developers:_ Daniel Patrick Norris, Ricky Dodd, Mat Perkins

### File Submission Enhancements

#### Overview, Goals, and Objectives

This project aims for enhance the file submission project for the OnTrack system. By increasing the
types of files that can be used for submission to OnTrack, ease of submitting tasks for students and
importing submissions for assessors will be increased. This project mainly effects the students, as
it will reduce steps needed to submit tasks; specifically the conversion of different file types.
Long term, this project aims to document accepted file types, identify file types that can be used
for the OnTrack system, and implement and document any new file types added to the system.

#### Aims for Trimester

The aims for this trimester are:

- Increase the compatability of different file systems for submission to the OnTrack System.
- Document currently available file types.
- Implement the Jupter Notebook file type for OnTrack submissions.

#### Deliverables

Short Term:

- Implement compatability for Jupiter Notebook file submissions.
- Investigation of different file types for future integration.
- Creation of Documentation for new file type implmentation.

Long Term:

- Maintenence of file updates and compatability of change file types.
- Integration of relevant file types into the OnTrack submission system.
- Ongoing documentation of valid file types new formats to add.

#### Project Mid-Trimester Progress

Currently Completed Tasks:

- Completed Local installation of OnTrack Project
- Committed Changes for Jupiter Notebook Submission

#### Project End-Trimester Progress

Completed Tasks:

- Completed Local installation of OnTrack Project
- Committed Changes for Jupiter Notebook Submission

#### Project Members (7)

_Delivery Representative:_ Nandini Kaushal

_Software Developers:_ Keerat Kaur, Aaryan Sharma, Gurpartap Singh Panesar, Jayant, Yongqi Huang,
Aryan Bagoria

### Security Analysis

#### Overview, Goals, and Objectives

The aim of the Security Analysis project is to understand the vulnerabilities in the OnTrack system,
to aid in the implementation of security measures. Given that OnTrack has a high throughput of task
submission and user data, protecting the students and assessors data is paramount for ensuring that
both technical system remain secure. This will effect all users of Ontrack, as well as the ongoing
development of the OnTrack system.

#### Aims for Trimester

The aims for this trimester are:

- Creation of documentation on testing standards to be used in the OnTrack project.
- Testing of OnTrack systems for vulnerabilities.
- Creation of testing documents for existing parts of the OnTrack system.

#### Deliverables

Short Term:

- Identification of current security vulnerabilities.
- Creation of testing standards.
- Documentation of issues and proposed fixes.

Long Term:

- Further ongoing testing of the OnTrack system for vulnerabilities.
- Implementation of fixes for identified security vulnerabilities.
- Further documentation of vulnerabilities and proposed fixes.

#### Project Mid-Trimester Progress

Currently Completed Tasks:

- Creation of Github and Trello Resources
- Research for Authenitcation and Authorisation Services
- Meeting with Hardhat Industries to initiate Security Analysis

#### Project End-Trimester Progress

Completed Tasks:

- Creation of Github and Trello Resources
- Research for Authenitcation and Authorisation Services
- Meeting with Hardhat Industries to initiate Security Analysis

#### Project Members (2)

_Delivery Representative:_ Ereena Bagga

_Developers:_ Ben Thomas

### User Interface Enhancement

#### Overview, Goals, and Objectives

The overarching goal of this project is to migrate the current components, which utilise
CoffeeScript and Bootstrap, to Angular framework with Typescript. CoffeeScript has outlived its
usefulness and falls short of more contemporary frameworks in terms of support, functionality, and
security. Developers can easily design dynamic single-page applications using Angular because to its
component-based architecture. As TypeScript provides types and enables early problem identification,
its use in its construction ensures improved security.

#### Aims for Trimester

The aims for this trimester are:

- Use bottom-up progression to migrate at existing components
- Restrict the conflicts between the old and new components
- Gain experience to enable speedier growth in future trimesters

#### Deliverables

Short Term:

- Develop and deliver at least 5 migrated components
- Carry on the components that are in the middle of migrating in last trimester

Long Term:

- Ensure all migrated components have been tested and function as expected by implementing test
  units.
- Prior to CoffeeScript support being removed, make sure that future team members are supported and
  set up for success to migrate all remaining components

#### Project Mid-Trimester Progress

Currently Completed Tasks:

- Creation of List of files to migrate from CoffeeScript to Typescript
- Initiated migration of 5 sections, with 2 completed.

#### Project End-Trimester Progress

Completed Tasks:

- Creation of List of files to migrate from CoffeeScript to Typescript
- Completed migration of 6 Components.
- Creation of Documentation of Migration.

#### Project Members (6)

_Delivery Representative:_ Leo Luong

_Software Developers:_ Anthony Papoutsis, Ahmed Ali, Aldy Putra Shavira, Kosta Constantinou, Nelson
Lai

### Google Cloud Deployment

#### Overview, Goals, and Objectives

The Google Cloud Deployment team aims to deploy the existing OnTrack system to the Google Cloud
Platform. This will aid in the interactions of the internal parts of the system, as well as scaling
the system for future development of the platform. The overall goal for this project is to fully
deploy and maintain the OnTrack system using the Google Cloud Platform.

#### Aims for Trimester

The aims for this trimester are:

- Build an Understanding of the OnTrack System and Google Cloud Platform to plan deployment.
- Deploy all parts of the OnTrack system to Google Cloud Platform
- Test relevant interactions between different systems to maintain current usability.
- Maintain OnTrack system using Google Cloud Platform tools.

#### Deliverables

Short Term:

- Creation of documentation of Google Cloud deployment of OnTrack.
- Initiate process of deployment of OnTrack system.

Long Term:

- Maintenence of the OnTrack system using the Google Cloud platform.
- Implementation of Google Cloud Platform tools to aid in testing and deployment of the OnTrack
  system.
- Ongoing Documentation of the OnTrack deployment to Google Cloud Platform.

#### Project Mid-Trimester Progress

Currently Completed Tasks:

- Creation of list of Tasks for Project Completion
- Building understanding of Docker
- Building understanding of the Google Cloud Platform

#### Project End-Trimester Progress

Completed Tasks:

- Creation of list of Tasks for Project Completion
- Building understanding of Docker
- Building understanding of the Google Cloud Platform
- Deployment of CI/CD system for Docker Watchtower
- Resources for Kubernetes deployment
- Plan of action for Deakin IAM and Security Permisions Policies.

#### Project Members (7)

_Delivery Representative:_ Harshpreet Kaur

_Developers:_ Anshuman Bishnoi, Dan Eastaugh, Sicheng Liu, Chetan Nagar, Pratham Gupta, Xuetong Zhao

### OnTrack Documentation

#### Overview, Goals, and Objectives

OnTrack is a growing and evolving system. OnTrack should be documented to ensure that future teams
who work on the project have a starting point to understanding and making changes to the existing
system. This will help all members of the OnTrack development team, current and future.

#### Aims for Trimester

The Aims for this Trimester are:

- Map out the existing OnTrack project, and related systems
- Discover areas of OnTrack that still need to be documented
- Ensure all mapped areas of the OnTrack Project are appropriately documented

#### Deliverables

Short Term:

- Mapping the existing OnTrack project
- Identifying areas to document
- Writing documentation for identified areas

Long Term:

- Ensuring the entirety of the current OnTrack project are documented
- Formatting documentation of new areas to match OnTrack documentation standards

#### Project Mid-Trimester Progress

Currently Completed Tasks:

- Creation of Map of OnTrack system
- Creation of List of areas to document
- Creation of OnTrack Local Distribution User Guide

#### Project End-Trimester Progress

Completed Tasks:

- Creation of Map of OnTrack system
- Creation of List of areas to document
- Creation of OnTrack Local Distribution User Guide
- Creation of OnTrack Documentation Template
- Creation of OnTrack Documentation Template User Guide
- Creation of OnTrack Architecture Document

#### Project Members (6)

_Delivery Representative:_ Shaine Christmas

_Documentors:_ Matt Clark, Jasdeep Singh, MD Fahim Mizi, Shiv Bhanu, Adrienne Gelbhauer

### Quality Assurance and Testing

#### Overview, Goals, and Objectives

This projects main goal is to identify and document the current features of OnTrack and put in place
a Quality Assurance and Testing infrastructure to better maintain the quality of OnTrack and allow
for more polished product. As OnTrack continues in its development, ensuring that robust testing is
important for ensuring the quality of OnTrack as a system. The overarching goal of this project is
to ensure that the OnTrack product is robust and completes rigorous testing.

#### Aims for Trimester

The aims for this trimester are:

- Help strengthen the QA and testing structure within Toth Tech
- Maintain/Create testing practices withing OnTrack and the greater Toth Tech
- Create use cases and then test cases for existing features within OnTrack
- Develop Unit, Integration and possibly UI testing for OnTrack

#### Deliverables

Short Term:

- Identify QA best practices withing Toth Tech
- Investigate existing QA process in OnTrack and Thoth Tech
- Define testing balance and scope
- Creation of Test Cases for standardising OnTrack QA
- Create/Maintain bug board
- Define/Find feature list for different features of OnTrack
- Create use and test cases for existing functionality

Long Term:

- Create and maintain testing framework(s) and an automation codebase on Git
- Create an automated practice for Unit, Integration and UI testing.
- Create a suite of automated tests that can be run easily
- Maintain a bug tracker
- Create/use documentation for standardising the creation of use cases and test cases

#### Project Mid-Trimester Progress

Currently Completed Tasks:

- Creation of Documentation for QA and Testing Procedures
- Up-skilling in QA technologies
- Creation of Automation Framework
- Creation of OnTrack current and developing feature list

#### Project End-Trimester Progress

Completed Tasks:

- Creation of Documentation for QA and Testing Procedures
- Up-skilling in QA technologies
- Creation of Automation Framework
- Creation of UI automation Repository
- Creation of OnTrack current and developing feature list
- Creation of Use Cases for Students, Markers, and Administrators
- Creation of Test Strategy Document
- Creation of Automation On-boarding Document
- Creation of Test Case Template
- Creation of Test Case List

#### Project Members (3)

_Delivery Representative:_ Matthew Paul Fletcher

_Testers:_ David Kwiatkowski, Parth Aneja

---
