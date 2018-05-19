# Intro To Coding For Journalists

This repository will hold a growing collection of resources and links to repositories to support a semester-long college level course aimed at journalists who want to learn coding skills.

### About this class

#### Basic requirements

This class enthusiastically welcomes beginners. No coding experience is necessary. You will need to be able to install and run the required software for the course on a machine that you will have access to between classes. The list of required software is [here](basic-requirements.md). If you are taking an in-person class, we will spend time in the first class installing those tools. 

#### Required Text

We will be using [Scott Murray's Interactive Data Visualization for the Web, 2nd Edition](https://www.amazon.com/Interactive-Data-Visualization-Web-Introduction/dp/1491921285/ref=dp_ob_title_bk).

#### Readings and assignments

Readings and assignments for a week are due the week they are listed; so readings and assignments listed under Week 3 are due at the beginning of Week 3. If your assignments include code, your commits or pull requests must be complete before class time on the week they are due.

#### Diagnostics

Diagnostics are quizzes done in class, typically at the beginning of class.

#### Labs

Labs are in-class exercises and activities. Each one is detailed in this repository with its own file, labeled like this: `week1.md`, `week2.md`, etc.

## Coding For Journalists: A Course Outline

### Week One: Why Code?/The Development Environment

We address the basic questions of 'why code' -- which go far beyond 'it will get me a job.' Accountability in our increasingly high-tech world requires more of us as journalists -- we want to have a working knowledge of the technologies that have an impact on public policy and the lives of individuals.

We introduce the idea of a 'development environment' -- the integrated suite of tools used by newsroom developers to create projects. Each student leaves with a working set of tools.

#### Week 1 Lab

[Week 1 Lab](week1.md)

#### Week 1 Readings
[Does Journalism Work?](http://jonathanstray.com/does-journalism-work), Jonathan Stray<br>
[Getting to Know The Command Line](https://www.davidbaumgold.com/tutorials/command-line/), David Baumgold<br>
[Learn Version Control with Git](https://www.git-tower.com/learn/git/ebook/en/command-line/introduction#start), Chapter 1, The Basics<br><br>

### Week Two: Version Control: Git, Github

We introduce version control -- a core aspect of coding and collaborating. We connect to code repositories maintained by The New York Times, Washington Post, and The Guardian and 'clone' those onto our own machines.

#### Week Two Readings
[Learn Version Control with Git](https://www.git-tower.com/learn/git/ebook/en/command-line/introduction#start), Chapter 2, Branching and Merging, and Chapter 3, Sharing Code<br>

#### Week Two Diagnostic
You will have a diagnostic (quiz) on the basics of Git, Github, and the command line.

#### Week Two Lab

[Week 2 Lab](week2.md)

#### Week Two Assignment

See the end of [Week 2 Lab](week2.md) for assignment details. Complete Week 3 Readings below. Assignment and readings must be completed by the beginning of class on Week 3.

### Week Three: Bootstrap and Flat File Websites

We use Bootstrap -- a template language developed by Twitter -- to create a template for a simple flat-file website, which we store and host on Github.

#### Week 3 Readings
Interactive Data Visualization for the Web, Chapter 3<br>
[What Is Bootstrap and How Do I Use It?](https://www.taniarascia.com/what-is-bootstrap-and-how-do-i-use-it/)<br>
[Lessons from an Intermediate Programmer-Journalist](http://michelleminkoff.com/2015/03/27/lessons-from-an-intermediate-programmer-journalist-part-3-of-3/), Michelle Minkoff, AP<br>

#### Week 3 Diagnostic
You will have a diagnostic on the terms and concepts covered in Chapter 3 of Interactive Data Visualization for the Web, and terms and concepts covered in What Is Bootstrap and How Do I Use It?

##### Week 3 Lab

We will build a basic flat-file site in class. Find repositories and directions here: [Week 3 Lab](https://github.com/fullstackjournalists/intro-to-coding-for-journalists/blob/master/week3.md)

#### Week 3 Assignment

See [Week 3 Lab](week3.md) for assignment details. Your code must be committed by class time to get credit for your assignment. You will show your work in class at the beginning of class on Week 4. Complete Week 4 readings by Week 4 class time.


### Week Four: Javascript: The D3.js Library Introduction

We introduce Javascript concepts and begin using D3.js, a library created by Mike Bostock to do election data visualizations for the New York Times. D3.js has now become the dominant web-ready data visualization library. We also do a 'tour' of state of the art data visualizations from newsrooms.

*Week Four Readings*<br>
Interactive Data Visualization for the Web, Chapters 4 & 5<br>
[Data Journalism Must Live Up To Its Own Standards](http://www.niemanlab.org/2014/07/alberto-cairo-data-journalism-needs-to-up-its-own-standards/), Alberto Cairo, NiemanLab

*Week Four Diagnostic*<br>
You will have a diagnostic on the portions of Javascript covered in Chapters 3 & 4.


### Week Five: Javascript: Using D3.js To Build Data Visualizations

We build a simple Javascript data visualization using D3.js.

*Week Five Readings*<br>
Interactive Data Visualization for the Web, Chapters 6-8

*Week Five Diagnostic*<br>
You will have a diagnostic on Chapters 6-8 of Interactive Data Visualization for the Web.<br>

*Week Five Assignment*<br>
Fork and clone the D3http repository, and follow the instructions to make a simple scatterplot. Connect the scatterplot to a new datasource as noted in the instructions. Push to Github Pages and drop a link to your work in the #assignments channel of the class Slack workspace.

### Week Six: Serving Data Visualizations to the Web

We will use the simple flat-file website we built in Week Three to 'host' our data visualization.  Reviews key development skills such as using a local webserver to test our work, and then 'pushing' it live to the web using version control tools.

*Week Six Readings*<br>
[Grunt.js Taskrunner: Getting Started](https://gruntjs.com/getting-started) Read this and install Grunt via npm. Be sure you can 'spin up' a local webserver in a directory on your own machine. <br>
[Creating a website on Github Pages](https://dev.to/programliftoff/create-your-first-website-on-github-pages)<br>
[Building News Apps on a Shoestring](https://source.opennews.org/articles/building-news-apps-shoestring/), Alan Palazzolo, ProPublica<br>

*Week Six Assignment*<br>
Fork and clone the Project Template repository, `npm install` the components, and spin up a local webserver. View the index.html file. If you have an issue, remember to [read the guide on how to file an issue](https://github.com/fullstackjournalists/fullstackjournalists/blob/master/how-to-file-an-issue.md) and file an issue.<br>

### Week Seven: Javascript: More Complex Data Visualizations

We take the basic D3 skills we have learned and, like art students, 'copy' a data visualization done by The Washington Post, and push it live to our own websites.

We also preview an app template -- either The Washington Post's Kyt or the NPR App Template, which will be used for a group project.

*Week Seven Readings*<br>
Chapter 10, Interactive Data Visualization for the Web<br>
[What I Learned Recreating One Chart Using 24 Tools](https://source.opennews.org/articles/what-i-learned-recreating-one-chart-using-24-tools/), Lisa Charlotte Rost, Source<br>
[Seeing Like A Geek](http://crookedtimber.org/2012/06/25/seeing-like-a-geek/), Tom Slee, Crooked Timber

*Week Seven Assignment*<br>
For the remainder of the semester, you will be working on an immersive story of your own creation. See the Story Standards document for requirements for this assignment. Next week, you will come to class and make a pitch to me and your fellow students for your semester project.

*Week Seven Diagnostic*
You will have a ten-question diagnostic on Chapter 9 of Interactive Data Visualization for the Web.

### Week Eight: Project Pitches; Project Planning & Collaboration

We will begin with students pitching a project. Practicing all of these skills in a real newsroom environment means having excellent project management and collaboration skills. We learn basic aspects of the Agile tech project management methodology, learn how to build and manage a project card board, and practice splitting up projects, doing tasks, and merging and launching code when it's from multiple team members.

*Week Eight Reading*<br>
[Interviewing Humans: A Guide to User Research](http://alistapart.com/article/interviewing-humans), Erika Hall<br>
[Painless Functional Specifications: Why Bother?](https://www.joelonsoftware.com/2000/10/02/painless-functional-specifications-part-1-why-bother/), Joel Spolsky<br>
[We can draw school zones to make classrooms less segregated. This is how well your district does.](https://www.vox.com/2018/1/8/16822374/school-segregation-gerrymander-map), Alvin Chang, Vox

*Week Eight Assignment*<br>

Fork and clone the Scroll Driven Story repo. Review the code and the README. Visit the examples of scroll-driven stories in the Examples.md file. _Add your own link to the list of scroll-driven story examples, using the format you see there -- it can't be one that's already there, and it can't be one of the ones we will review in Week Nine. Do a pull request to add your link to the list of examples.

### Week Nine: Scroll-Driven Storytelling & Other New Forms

We will take a look at three major new tech-driven news forms, including news apps, customizable stories, and scroll-driven stories. During this class, we will get a basic scrolling site up and running using the Scrollmagic.js library.

*Week Nine Readings*<br>
[How To Build a News App In Two Days](https://source.opennews.org/articles/news-app-in-two-days/), Al Shaw, ProPublica<br>
[Implementing Scrollytelling in Six Libraries](https://pudding.cool/process/how-to-implement-scrollytelling/), Russell Goldenberg, The Pudding<br>

*Week Nine Examples*
[Homan Square: A Portrait of Chicago's Detainees](https://www.theguardian.com/us-news/ng-interactive/2015/oct/19/homan-square-chicago-police-detainees), The Guardian<br>
[Sin Luz: Life Without Power in Puerto Rico](https://www.washingtonpost.com/graphics/2017/national/puerto-rico-life-without-power/?utm_term=.6d792120fca8)<Br>
[Simone Biles, Gymnast](https://www.nytimes.com/interactive/2016/08/05/sports/olympics-gymnast-simone-biles.html)<br>
[Bulger on Trial](http://bulger.wbur.org/story/1977/)<br>
[Snowfall: The Avalanche at Tunnel Creek](http://www.nytimes.com/projects/2012/snow-fall/index.html#/?part=tunnel-creek)<br>
[Climate Change Claims a Lake and an Identity](https://www.nytimes.com/interactive/2016/07/07/world/americas/bolivia-climate-change-lake-poopo.html)

### Week Ten: Scroll Driven Storytelling Hands-On

We will work with the Scroll Driven Storytelling repository and explore additional project transitions and features of the Scrollmagic.js library that you will use to create your story's immersive site.

### Week Eleven and Twelve: News App Project Workshop

Students will work together in teams and address issues they have encountered with their projects.

### Week Thirteen: News App Project Presentation & Final Pull Requests

Students give a live presentation of their app and do a final pull request on the class's repository, adding a link to their project to our class's official list of work.
