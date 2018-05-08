# Week Two: Version Control: Git, Github

We introduce version control -- a core aspect of coding and collaborating. We connect to code repositories maintained by The New York Times, Washington Post, and The Guardian and 'clone' those onto our own machines.

## Week Two Readings

[Learn Version Control with Git](https://www.git-tower.com/learn/git/ebook/en/command-line/introduction#start), Chapter 2, Branching and Merging, and Chapter 3, Sharing Code<br>

## Week Two Diagnostic
You will have a diagnostic (quiz) on the basics of Git, Github, and the command line. This diagnostic will be at the END of class (normally diagnostics are at the beginning of class). <Br>
[Week 2 Diagnostic](https://github.com/fullstackjournalists/Week2-Diagnostic)

## Week Two Lab

### 1. Fork The Week Two Lab Repository

#### What happens when you fork a repository?

When you `fork` a repository, you make a copy of a repository in Github. That copy resides in your own Github account. Any changes you might make are not reflected automatically in the master or "upstream" repository.

**Do now:** Fork the Week 2 Lab repository: [Week 2 Lab](). You will see a button in the upper left that reads 'fork.' It looks like this: <br>
![Fork button, Github](http://)

Once you do that, you will see a cute little animation that looks like this: <br>

![Fork animation]()

Once this is done, you should have a new copy of the repository in your own Github account.

**Doublecheck:** Do you now have a new repository with the url `http://github.com/yourusername/Week2-Lab/`? If you are not on that page, request help from your instructor or a TA. If you are, proceed onto the next step.

### 2. Clone the repository

#### What happens when you clone a repository?

Forking a repository copies it from one account on Github to another account on Github (usually your own). `Cloning` the repository transfers a copy of the repository from your Github account to your local computer. It's generally a necessary first step for you to get working on the code in that repository!

**Do now:** Clone the repository. Be sure you are at YOUR copy of the repository -- the one at the url http://github.com/yourusername/Week2-Lab.

Open Terminal and go to your `projects` directory. Once you are in the directory, type:

`git clone` and then paste the URL you got from your forked repository. Press enter.

**Doublecheck:** At the command line, type `ls` and hit return. Do you see a folder called Week2Lab? If so, proceed to the next step.

### 3. Change into the directory.

At the command line, type `cd Week2Lab`.

Once you have done that, at the command line, type `touch Week2.md` and press return.

**Doublecheck:** At the command line, type `ls` and hit return. Do you see a file called `Week2.md`? If so, proceed to the next step.

### 4. Add the project folder in Atom.

In Week 1, you installed the Atom Text Editor. Open it now, and choose File > Add Project Folder. Add the Week 2 Lab folder.

Click on the Week2Lab.md file in the left column, and copy-paste the following text:

`# Week 2 Lab: Learning Git and Github`

In Atom, choose File > Save All.

**Doublecheck:** Look at the tab that says Week2.md. Does it have a blue dot? If so you have not saved the file. If it does not, proceed to the next step.

### 5. The Git/Github Cycle: Add, Commit, and Push

At the command line, type `git status` and hit return. You should see `Week2.md` as a file that has not been added.

Type `git add -A` to add all files.

Now, type `git commit -m "adding Week2.md file"` and hit return.

Type `git status` again. Do you see any differences?

Now, you have added files and "committed your changes" along with a commit message describing what you did. However, the copy of your repository on Github has not changed. Go take a look at it now.

Back at the command line, type `git push origin master` and hit return.

**Doublecheck:** Visit your version of the Week2 Lab repository in your account on Github. Do you see your commit message, and the new file? If so, proceed to the next step.















*Week Two Assignment*<br>
Fork and clone our class repository, add your name and a link to a project or your website on the students.md file, commit your changes, push them, and make a pull request. Due by Week 3 class.<br>
