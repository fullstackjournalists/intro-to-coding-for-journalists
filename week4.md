# Week Four: Javascript: The D3.js Library Introduction

We introduce Javascript concepts and begin using D3.js, a library created by Mike Bostock to do election data visualizations for the New York Times. D3.js has now become the dominant web-ready data visualization library. We also do a 'tour' of state of the art data visualizations from newsrooms.

## Week Four Readings

You must complete these readings by the beginning of Week 4 class time.

Interactive Data Visualization for the Web, Chapters 4 & 5<br>
[Data Journalism Must Live Up To Its Own Standards](http://www.niemanlab.org/2014/07/alberto-cairo-data-journalism-needs-to-up-its-own-standards/), Alberto Cairo, NiemanLab

# Week Four Diagnostic
You will have a diagnostic on the portions of Javascript covered in Chapters 3 & 4.

## Week Four Lab

During this class, we will build a simple interactive data visualization using D3.js.

### Fork and clone Week 4 Lab repository

Fork and clone the repository [Intro to Coding for Journalists: Week 3 Lab](https://github.com/fullstackjournalists/Week4-Lab) into your `projects` folder.

Using Terminal, navigate to the folder you just created using `git clone`.

Type `ls`, or if you are using Windows, `dir`.

You should see the following files and folders:

```
MA-EDU-DATA4.csv	cereal.csv		gruntfile.js		package-lock.json	start.html
README.md		finish.html		node_modules		package.json		working.html
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

If all goes well, you should be able to see a list of files in the /Week4-Lab/ directory.
Click here: [http://localhost:9000/](http://localhost:9000/). Then click on `start.html`.

You should see something like the following:

*If `grunt serve` gives you an error message, type `npm install -g grunt-cli`, and once it installs, run `grunt serve` again.*

### Add, Commit and Push

At the command line, type `git status`. There should be many files that have not yet been added.

Type `git add -A`. Then commit the files you added by typing `git commit -m " "`. Between the quotes, describe what you did, then hit return. Remember that I grade you on the quality of your commits, including your commit messages.

Finally, type `git push origin master` to save your changes to your repository in the cloud at Github.com.

## Code Exploration

Visit: [http://localhost:9000/](http://localhost:9000/). Then click on `working.html`.
It should look exactly the same as `start.html`, because it is. What you'll see
here is a scatterplot, showing data about cereal on two dimensions -- calories
and protein content. Be sure to mouseover some of the dots. Notice that tooltips pop up
when you do.

Visit: [http://localhost:9000/](http://localhost:9000/). Then click on `finish.html`.
Here, you'll see a different scatterplot that's a little more interesting from a journalistic point of view -- it compares per-pupil spending to standardized test scores in Massachusetts.

In this exercise, we are going to walk through all of the elements that create this data visualization, and then we are going to take our beginning dataviz -- the one on cereal -- and hook it up to our journalism-focused dataset on school scores vs. school spending.

### Doctype

Every HTML document you create should have a DOCTYPE declaration. This tells the browser what kind of document it is.  Beyond that, we have a few other items of interest. Can you tell what they mean? What are the items that begin with `<!--`?

```
<!DOCTYPE html>
<html>
<meta charset="utf-8">

<!-- Example based on http://bl.ocks.org/mbostock/3887118 -->
<!-- Tooltip example from http://www.d3noob.org/2013/01/adding-tooltips-to-d3js-graph.html -->

```

### Styling

After we declare a doctype, we have some styling information. In Week 3, you created a flat-file website that used CSS. In general, CSS is stored in a separate file from your HTML file, and you reference it. Here, the CSS is embedded right in the page between `<script>` tags. In general, you want your CSS in a separate file, but here, for simple styling purposes, it's okay.

What do these style elements do? Can you guess?

```
<style>
body {
  font: 11px sans-serif;
}

.axis path,
.axis line {
  fill: none;
  stroke: #000;
  shape-rendering: crispEdges;
}

.dot {
  stroke: #000;
}

.tooltip {
  position: absolute;
  width: 200px;
  height: 28px;
  pointer-events: none;
}
</style>

```

Notice the following code block:

```
.axis line {
  fill: none;
  stroke: #000;
  shape-rendering: crispEdges;
}
```

Change `stroke: #000;` to another color, using [ColorHex](http://www.color-hex.com/).

Visit[http://localhost:9000/working.html](http://localhost:9000/). Has the color of the axes changed? Great. Now change them back to black.

## Linking to the D3.js library

When we build an HTML page that makes use of a Javascript library, we have to link to it. Notice that this link always comes right at the top, before any Javascript we write that takes advantage of that library.

```
<script src="https://d3js.org/d3.v3.min.js"></script>

```
