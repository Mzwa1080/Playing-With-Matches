---
layout: default
---

<h1 data-task-number="5">Publish your code to a website</h1>

> In this task, you'll use a special feature of GitHub to publish your work to the web.

Now we're going to publish your work to a website using [GitHub Pages](https://pages.github.com/), so that you can easily demo your work. If you have a git branch called `gh-pages` in a repository that you have pushed to GitHub, GitHub will publish the static HTML, CSS, and JavaScript for you at at `<username>.github.io`. You can use this for any static content, but not for applications that require a server.

Add a file called `index.html`. Inside it, make a list of links to the pages you made from task 1, 2, and 3. Add some CSS to make it look more interesting. You might want to look at [list-style](https://developer.mozilla.org/en-US/docs/Web/CSS/list-style) and  [list-style-type](https://developer.mozilla.org/en-US/docs/Web/CSS/list-style-type). In `task1.html`, `task2.html`, and `task3.html` add a (hyper)link back to `index.html`.


## Branches

In the terminal, change to your project folder and type

{% highlight bash %}
git branch
{% endhighlight %}

to see a list of your branches. You should see only one branch called `master`.
Now create a new branch called `gh-pages`, like this:

{% highlight bash %}
git branch gh-pages
{% endhighlight %}

This tells git to make a new branch called `gh-pages` based on your current branch (which is `master`).

Now do `git branch` again. What do you see? Does `git branch` tell you which branch you are on?

To move into your new branch, type:

{% highlight bash %}
git checkout gh-pages
{% endhighlight %}

Any commits you make now will be on the `gh-pages` branch (and won't show up on `master`). You'll be using this branch to publish the work you are doing to [GitHub Pages](https://pages.github.com/).

## Publishing using GitHub Pages

To push this branch to github type:

{% highlight bash %}
git push origin gh-pages
{% endhighlight %}

GitHub notices that you've pushed a branch called `gh-pages`, takes the HTML, CSS, and JavaScript, and publishes it. This can take a minute or two. Your RedAndGreen work is now published at https://&lt;username&gt;.github.io/RedAndGreen.

After you've done this you should checkout the master branch again by doing:

{% highlight bash %}
git checkout master
{% endhighlight %}

## Files we don't need git to watch

Let's learn a bit more about another part of git: [ignoring files](gitignore.md).
