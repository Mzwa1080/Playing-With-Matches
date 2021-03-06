---
layout: default
---

# Playing With Matches

We'll be making a web page with HTML, CSS, and JavaScript. Let's have a look at how these three pieces fit together.

![web triangle](./img/web-triangle.png)

The structure of every web page looks a bit like this. It's a triangle because the balance should mostly be like that: lots of HTML, quite a lot of CSS, and as little JavaScript as possible.

At the base you have your **HTML**. It's the **structured content** of the page: headings, paragraphs, images, videos.

On top of that you have your **CSS**. This handles the **presentation**: colours, fonts, layout. Note that it's a separate layer: see, there's a line there and everything. It exists apart from the structure and content (the HTML) of the page.

At the top, in the tiny triangle, is the **JavaScript** (JS). This adds behaviour and interactions to the page. It's the most fragile part of the three. An error in the code (perhaps introduced at midnight by a sleepy developer as a "quick fix") can break the whole block of the JS.

## Local set up

<!--codex ignore easily-->
You should have a projects folder in your home directory. It's good practice to create all your different projects in one place on your PC so that you can find them easily.

In your projects folder:

* create a folder called **Playing-With-Matches**;
* change into the folder **Playing-With-Matches** from the terminal using `cd Playing-With-Matches`;
* initialize it as a git repository using `git init`.

As you do each task create the files in the **Playing-With-Matches** folder.

After each task remember to commit your changes using git.

## The Steps

We're going to build up a page that shows a series of random numbers, checks for matches, and shows a message. The end result will look like this:

![matches](./img/matches.jpg)

Work your way through the 10 steps, starting with [Show a number](show-a-number.html).
