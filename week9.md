# Week Nine: Scroll-Driven Storytelling & Other New Forms

We will take a look at three major new tech-driven news forms, including news apps, customizable stories, and scroll-driven stories. During this class, we will get a basic scrolling site up and running using the Scrollmagic.js library.

## Week Nine Readings

[How To Build a News App In Two Days](https://source.opennews.org/articles/news-app-in-two-days/), Al Shaw, ProPublica<br>
[Implementing Scrollytelling in Six Libraries](https://pudding.cool/process/how-to-implement-scrollytelling/), Russell Goldenberg, The Pudding<br>

## Week Nine Examples
[Homan Square: A Portrait of Chicago's Detainees](https://www.theguardian.com/us-news/ng-interactive/2015/oct/19/homan-square-chicago-police-detainees), The Guardian<br>
[Sin Luz: Life Without Power in Puerto Rico](https://www.washingtonpost.com/graphics/2017/national/puerto-rico-life-without-power/?utm_term=.6d792120fca8)<Br>
[Simone Biles, Gymnast](https://www.nytimes.com/interactive/2016/08/05/sports/olympics-gymnast-simone-biles.html)<br>
[Bulger on Trial](http://bulger.wbur.org/story/1977/)<br>
[Snowfall: The Avalanche at Tunnel Creek](http://www.nytimes.com/projects/2012/snow-fall/index.html#/?part=tunnel-creek)<br>
[Climate Change Claims a Lake and an Identity](https://www.nytimes.com/interactive/2016/07/07/world/americas/bolivia-climate-change-lake-poopo.html)

## Week 9 Lab

In this week's lab, we'll be taking a static HTML/CSS page and using the Scrollmagic.js library to create a scroll-driven page.

### Fork and clone the Week 9 Lab Repository

Fork and clone [the Week 9 Lab repository](https://github.com/fullstackjournalists/Week9-Lab).

### Code tour

In previous weeks, we've worked with code files where HTML, CSS, and Javascript have all been combined in a single file. As you do more complex projects, it's better practice to separate these elements.

_Questions_

Looking at `index.html`, what Javascript libraries and files are being referenced?

### Wrapping each section

We'll be using the Scrollmagic.js library to create a simple, scroll-driven page. Scrollmagic uses Javascript to add elements to the page and make changes to the CSS to change the appearance of the page.

In order to allow Scrollmagic.js to target a specific part of the page, we have to wrap it in a `<div>` tag with an ID.

Find the following line of code:

`<article id="slide01" class="slide">`

Immediately underneath this, add

`<div class="pin-wrapper">`

You'll need to close the `</div>` tag immediately above the `</article>` tag.

### Building the Javascript

Look at the `main.js` file. Right now, it has only one line in it.

First, you have to "initialize" the Scrollmagic.js. library.

Add this under the first line of the file:

`var controller = new ScrollMagic.Controller();`

Now, we have to tell ScrollMagic what to control:

```
var pinScene01 = new ScrollMagic.Scene({
  triggerElement: '#slide01',
  triggerHook: 0,
  duration: '100%'
})
.setPin('#slide01 .pin-wrapper')
.addTo(controller)
;
```

### Changing the CSS
