# Week 1: Why Code?/The Development Environment


We address the basic questions of 'why code' -- which go far beyond 'it will get me a job.' Accountability in our increasingly high-tech world requires more of us as journalists -- we want to have a working knowledge of the technologies that have an impact on public policy and the lives of individuals.

We introduce the idea of a 'development environment' -- the integrated suite of tools used by newsroom developers to create projects. Each student leaves with a working set of tools.

Weekly presentation: Each week a student or pair of students should select and be prepared to discuss a news app or data visualization.

## Week 1 Lab

## Install All The Things!

We will spend the first part of the class installing the necessary tools for this course on your machine. Please visit [Basic Requirements](basic-requirements.md) when instructed to do so by your sponsor. Do not skip ahead until asked to do so!

## The Command Line

Each week's session will contain a lab segment where we walk through code or use tools. In this lab, we're going to get familiar with the basics of the command line and set up your project folder for this course.

### Open Terminal

On your machine, visit Applications > Utilities > Terminal.

You will see something like this:

At the command line, type `cd ~`. That's a tilde, usually to the right of the 1 key on your keyboard. Press return.

You are now in the `root directory` of your machine (or your user account on your machine). By `root directory`, we mean that there are no higher levels of folders.

### List files and directories

At the command line, type `ls`, or if you are on a Windows machine, type `dir`. Press return. You should see a listing of files and directories that are currently in your root directory.

Now type `ls -a`. You'll notice that there are some files and folders that you didn't see before, most of which begin with a period. These are hidden files and folders.

*Commands and flags*

`cd` and `ls` are *commands.* Commands can have options, which are commonly known as "flags." `ls -a` is the `ls` (list) command with the `-a` "flag", modifying the command so that it lists *all* files and folders, including hidden ones.

### Make a directory

At the command line, type `mkdir project` and press return. Now, type `ls`. Do you see your new project folder?

### Switching into your new directory

At the command line, type `cd project`. You are now *inside* the folder you just created.

### Use touch to create files

At the command line, type `touch README.md` and hit return. Now type `ls`. Do you see the new file you created? It's empty, for now, but it exists!

### Navigate up and out of your directory

At the command line, type `cd ..` Now you will notice that you are one level "up" from your project folder, back in the root directory.

### Rename a directory

Hey! We're probably going to have more than one project this semester, right? Let's rename our `project` folder to `projects`.

At the command line, type `mv project projects`. The `mv` command is the "move" command. Technically, you just moved `project` to `projects` and renamed it at the same time. This is an example of commands taking *arguments.* In this case, the `mv` command needs two arguments -- the place you're coming from, and the place you are going to.

Type `ls` and hit return to see if your changes have been made.

### Removing directories

At the command line, let's switch into our projects directory by typing `cd projects`.

#### Exercise: Make a mistake

Make a new directory inside this directory, and call it `oops`.

Switch into the `oops` directory, and create a file at the command line called `oops.txt`.

#### Cleaning up your projects folder

You really didn't want that `oops` folder. Here's how to get rid of it. Type `cd ..` to navigate "up" one level. Type `ls`, and you should see the `oops` folder.

Now type `rm -rf oops`.

Type `ls` again. Is your folder gone?

Exercise: Visit this [terminal cheatsheet](https://gist.github.com/poopsplat/7195274) and tell us what the -r -f flags mean on the `rm` command.

#### The command line is powerful...use it wisely!

The command line is a powerful tool that does what you ask. It doesn't give you a lot of warnings asking you if you want to delete things. You can delete vast swaths of your work this way.

### Terminal shortcuts

Visit the command line and press the "up" key on your keyboard. You'll see the last command you typed. Keep pressing up -- it will go back to the beginning of your session. Down also works, and will work "down" to the last command you entered.

While at the command line, press Command + T. Your Terminal window can have tabs, just like your browser does. This will become useful as you progress.

Type `cd ~`. No matter where you are, this will always bring you to your root directory. Type `ls` so you can see your `projects` folder in the list of folders. Now type `cd proj` but don't finish typing "projects." Instead, hit the Tab button. Nifty, isn't it? Your terminal will autocomplete many things for you.



## Week 1 Readings

[Does Journalism Work?](http://jonathanstray.com/does-journalism-work), Jonathan Stray<br>
[Getting to Know The Command Line](https://www.davidbaumgold.com/tutorials/command-line/), David Baumgold<br>
[Learn Version Control with Git](https://www.git-tower.com/learn/git/ebook/en/command-line/introduction#start), Chapter 1, The Basics<br><br>

## Week 1 Assignments

Please complete the Week 1 and Week 2 readings and come to next week's class prepared to discuss them.
