# Week Three: Bootstrap and Flat File Websites

We use Bootstrap -- a template language developed by Twitter -- to create a template for a simple flat-file website, which we store and host on Github.

## Week Three Readings
By class time for week three, you should have completed the following readings

Interactive Data Visualization for the Web, Chapter 3<br>
[What Is Bootstrap and How Do I Use It?](https://www.taniarascia.com/what-is-bootstrap-and-how-do-i-use-it/)<br>
[Lessons from an Intermediate Programmer-Journalist](http://michelleminkoff.com/2015/03/27/lessons-from-an-intermediate-programmer-journalist-part-3-of-3/), Michelle Minkoff, AP<br>

## Week Three Diagnostic
You will have a diagnostic on the terms and concepts covered in Chapter 3 of Interactive Data Visualization for the Web, and terms and concepts covered in What Is Bootstrap and How Do I Use It?<Br>

[Week Three Diagnostic]()<br>

## Week Three Lab

During this class, we will build a simple flat-file website using Bootstrap and host it on Github Pages.

### Fork and clone Week 3 Lab repository

Fork and clone the repository [Intro to Coding for Journalists: Week 3 Lab](https://github.com/fullstackjournalists/Week3-Lab) into your `projects` folder.

Using Terminal, navigate to the folder you just created using `git clone`.

Type `ls`.

You should see the following files and folders:

```
LICENSE			gruntfile.js		index.html		package-lock.json	vendor
README.md		gulpfile.js		js			package.json
css			img			node_modules		scss
```

### NPM Install

At the command line, type `npm install`.

Your terminal should be telling you lots of things right now. That's because it
is downloading all the files specified in package.json.

**Errors?** If you get an error message when you try to run NPM install, you may need to install NPM (which stands for Node Package Manager). [Follow the instructions here](https://www.npmjs.com/get-npm) to download and install npm.

### Grunt serve

Once your `npm install` has completed, at the command line, type `grunt serve`.

Grunt is a "taskrunner." In this case, the task that it is running for us is
to spin up a local webserver so we can see the files in this directory in our
web browser.

If all goes well, you should be able to see a basic, blank website using
the "Grayscale" theme at [http://localhost:9000/](http://localhost:9000/).

### Lab Assignment

Your assignment is to create a website for Full Stack Journalists using this
template as a starting point.

The only two files you will need to alter are:

* index.html
* css/grayscale.css

Your site should include:

* A title
* An appropriate header image
* A description of our group
* A link to our Github organization
* Links to or descriptions of how to become a member and where/when we meet
* Social media links

Images in your site template are linked to through the CSS file -- `css/grayscale.css`.
Open that file in Atom and search for .jpg and you will see them.

#### 1. Changing the Title

In `index.html`, find the title on line 58. Change the title and the subtitle.
Save your work and look at it on [http://localhost:9000/](http://localhost:9000/).

In terminal, type `git status`. It should show that you have modified `index.html`.
If it doesn't, go back to Atom and save your work, and try again.

At the command line, type `git add index.html` and hit return.

Then type `git commit -m "Changed title and subtitle."` Feel free to get creative
with your commit messages!

Type `git push origin master`. Make sure your commit now shows up at
http://github.com/yourusername/week3-lab

#### 2. Change the header image

In Atom, look in the `img` folder.

In Atom, navigate to the CSS folder and open `grayscale.css`. Using the search
function, find `intro-bg.jpg`. Change this to `code.png`. Save your work and check it on [http://localhost:9000/](http://localhost:9000/).

In terminal, type `git status`. It should show that you have modified `grayscale.css`.
If it doesn't, go back to Atom and save your work, and try again.

At the command line, type `git add grayscale.css` and hit return.

Then type `git commit -m " "` Describe what you did between the quotes and press Return.

Type `git push origin master`. Make sure your commit now shows up at
http://github.com/yourusername/week3-lab

### Adding text content

Return to `index.html` and browse what's there. Note where text from the current
site template appears in the `index.html` file. Using those as a guide,
add the content for the remainder of the steps.

Check your work at each step on [http://localhost:9000/](http://localhost:9000/) and make commits frequently. Remember that commits are a big part of your grade.


### Setting up a web-available version

In your copy of the Week 3 repository at http://github.com/yourusername/week3-lab,
Scroll down until you see the section for Github Pages. Where it says "Source,"
use the pulldown menu to make `master` the branch that your Github page will
reflect online.

### Bonus: Changing nav elements & adding social media elements

You might have noticed that the navigational elements at the top of the page
don't really correspond with what we want for our site. Can you change them?

What about changing the social media elements to point toward our social media
accounts?

Remember to test locally and commit after each change.

### Extra Bonus: Fix something

Since you are such eagle-eyed students, you probably also noticed that there's something wrong with our template site: the map is broken.

How could you remove that section without actually deleting any code?

(Psst: the answer is `commenting out`!)

## Week Three Assignment

Due before class, Week 4: Fork and clone the week3-lab repository again, change the title and add links, content and images to make a bare-bones portfolio site about you and your work and interests. Make sure your new repository has a good name, like /yourname-portfolio. Commit changes and push frequently. When you are ready, post the link to the Github Pages version of your site to our class Slack workspace in the #assignments channel. Due by Week Four class time; you will show your work at the beginning of class. Impress us!
