---
layout: default
---

# Show a random number on page load

> Use JavaScript to generate a random number and update HTML and use external CSS.

![](./img/2.jpg)

Our next step is to use JavaScript to make our number random and changing rather than fixed. To do that, we need to find the number on the page, then change.

## Get your web page ready

Update your `index.html` by moving your CSS to an external file, like this:

{% highlight html %}
   <!-- Your CSS goes in the styles.css file -->
	<link rel="stylesheet" href="styles.css">
</head>
{% endhighlight %}

Add a space for your JavaScript at the bottom of the page, like this:

{% highlight html %}
  <script type="text/javascript">
		// JavaScript code goes here at the bottom
	</script>
</body>
{% endhighlight %}

## Write a random number function

In your `script` block, write a function that returns a random number from 1 to 9. Have a look at [Math.random() on the Mozilla Developer Network](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Math/random).

What's the function's name? What are it's parameters (sometimes called arguments)? What does `return` do?

Next we'll need to find a `div` on our page. Let's look at HTML documents in more detail.

## The DOM

DOM stands for Document Object Model. This is an in-memory representation of the elements contained in an HTML document. Eloquent JavaScript provides a good introduction to the DOM in [Chapter 13: The Document Object Model](http://eloquentjavascript.net/13_dom.html).

You can find elements in the DOM by their `id` or by their `class`. There are a couple ways of doing this. Have a read about these on the [Mozilla Developer Network](https://developer.mozilla.org/en-US/) about:

* [getElementById](https://developer.mozilla.org/en-US/docs/Web/API/Document/getElementById)
* [getElementsByClassName](https://developer.mozilla.org/en-US/docs/Web/API/Document/getElementsByClassName)
* [querySelector](https://developer.mozilla.org/en-US/docs/Web/API/Document/querySelector)

## Write a function that updates the HTML

Each function should only do one thing, so now let's write another function that finds your `div` and uses the random number function you wrote above.

Once you're finished, you'll need to **call your function**. How and where do you do this?

One you're done, every time the page loads you should see a new random number. Yay!

## Add your files to your repository

Once you are done, add your changes to git by using these commands:

* `git status` to see what changed.
* `git add index.html` to add the changes you made in `index.html` to git.
* `git add styles.css` to add the `styles.css` file to git.
* `git commit -m "your message"` to commit your changes.
* `git push origin master` to push your changes to GitHub.
