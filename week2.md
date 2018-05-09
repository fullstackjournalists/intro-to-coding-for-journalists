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
![Fork button, Github](/images/fork.png)

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

### 6. Branching

Git repositories can have "branches." In fact, your git repository already has a branch even if you don't remember creating one; the default branch is called `master`. Let's imagine you have written the code for a portfolio site where you can show off your work. But you'd like to spruce it up a little with a nice new navigation bar with fancy, fold-down menus. At the command line, you could type:

`git branch fancy-menu`

In that branch, you could try your experiments, but the code in your `master` branch stays untouched (and not messed up!). But what if you get your new, fancy menu working, and you want to integrate that code into your site? Well, that's where `merging` comes in.

If you wanted to merge the `fancy-menu` branch into your `master` branch, you would first "check out" the master branch like so:

`git checkout master`

If you haven't added your changes and committed them, git won't let you switch branches, so be sure you do that first.

Now you're in the `master` branch and ready to merge your changes. Then you'd type:

`git merge fancy-feature`

Now, all the work you did in `fancy-feature` is integrated into your `master` branch. It's also a great time to go through the add-commit-push cycle outlined in #5.

#### Exercise: Creating a branch

In your Week2-Lab directory, type:

`git branch fancy-feature` and hit return.

Then type `git checkout fancy-feature`.

Once you have done this, open your project folder in Atom.

**Doublecheck:** Look at the bottom left of the Atom editor window. Do you see the branch icon? Next to it, it has the name of the branch you are currently working in. Does it say `fancy-feature`? If so, move on to the next step.

In the  `week2-lab.md` file, type:

`# Testing branching and merging in Git`

Save your project. At the command line, go through the add, commit, push process.

**Doublecheck:** Visit your Github account. Does your Week 2 repository show your most recent commit message? If so, you can move on to the next step in the lab.


### 7. Merging

At the command line, type `git checkout master`. Now it's time to merge the code for our new `fancy-feature` branch.

At the command line, type `git merge fancy-feature`. Visit your code in Atom. Check the bottom rail to see that you are in the `master` branch. Does the Week2.md file contain your changes?

Finish up by going through the add, commit, and push cycle in Step 5.

### 8. Rolling back

In Atom, add the following random nonsense to your file:

```
naopwzdcrirvuxcsuhwuiqvzfaonbd rrjlukxeliivtcllmgbketmvnijfyn xqxlxbcwdkndjczroukiyhbqqaijdb runajaazawvccslkjrgvbkpgldaysp splvcgzcruyezjmvxohshhsjkcykfq cxnaonnaqsxiuiarjgqtodadkzbjtg bvgysrzbrtkmvvcjymbrwfseskxesf niktjjwegskuwyevofvtzlepbfyofe ygyzjzoluilinjrzskxeaeoriurskp lofqfhnwushcqnxqytwufmcaiysbpt

```
Save the file, and go through the add, commit, push sequence.

Hey, you were tired, you were undercaffeinated, and now...there's random nonsense in your repository on Github. Whatever shall we do?!

As a budding developer, you will make mistakes. As an experienced developer, you will make more complicated mistakes 😁. Either way? Mistakes.

Fortunately, we can now get to one of the truly magical parts of version control: the ability to roll back to any commit in your project.

Sure, you will break things. But NBD! You can roll it back in time to a point where it was working! Don't you wish you had that feature...for your life!?

Well, you might not be able to do it for your life, but you *can* do it with your code. Here's how.

Visit your repository on Github. See the "Commits" link, just above your code on the right?

![Image of commits link on Github](/images/commits.png)

Click on that.

You'll see a reverse-chronological list of all the commits on that repository, like so:

<img src ="/images/commit-list.png" width = "500">

Note the series of letters and numbers to the right of each commit, and the clipboard icon next to it.

Each of your commits has a unique alphanumeric identifier, called a SHA.

Look at the commit immediately below the one you just made. That's the commit that you made before your most recent one. We're going to "roll back" to that commit.

At the command line, type `git revert [paste your SHA here]` and click return.

Check out your file. Are the nonsense strings of characters we added gone? Great.

Now is a *great* time to go through the add, commit, push cycle. In fact, I insist.

**Resource:** [How to Undo Almost Anything With Git](https://blog.github.com/2015-06-08-how-to-undo-almost-anything-with-git/)


### 9. Make a pull request

What is a pull request?

At the beginning of this lab session, you forked (made your own copy of a repository in your own Github account) and cloned (copied that forked repository down to your computer) our Week 2 Lab repository. Let's imagine that you wanted to contribute some changes to the master directory. How would you do that?

You do that with a pull request.

Across the top row of tabs on your repository, you'll see one called "Pull requests."

Click on that and you'll see this:

<img src ="/images/pull-request.png" width = "500">

I'd like you to note a few things before moving on. It might be easiest to do so if you visit the Pull Requests tab in your own repository. First, note that underneath the name of your repository, it notes where it was forked from -- what your 'master' repository is.

When you make a "pull request," you are asking the maintainer of the master repository to consider "pulling" your changes into their repository.

Click on the "Pull request" button, and make a note in the dialog box. "First Pull Request 🎉" is always a good one if that happens to be true for you.

Finish your pull request and see what happens.

#### What happens on the other side?

There's a real live person or team on the other side of your pull request. They'll see your incoming request in their Pull Requests tab and choose to integrate those changes or not. Remember to write a good pull request message describing your changes and why you think they're an improvement if you want a better chance of having your "PR" approved.

*Week Two Assignment*<br>

Fork and clone our class repository, add your name and a link to a project or your website on the students.md file, commit your changes, push them, and make a pull request. Due by Week 3 class.<br>
