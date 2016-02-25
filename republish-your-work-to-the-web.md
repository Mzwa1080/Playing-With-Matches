---
layout: default
---

<h1 data-task-number="8">Republish your work to the web</h1>

> In this task, you'll use GitHub Pages again to re-publish your work to the web.

Look at your `gh-pages` branch. Does it have your new work there? How can you check this?

You can use `git branch` to check what branch you are on, `git log` to see a list of commits you have made, and `git checkout <branchname>` to switch between branches.

When two branches have diverged (they have some commits the same and some commits different), you can perform a `merge` to bring the two together. Have a look at the `git merge` section of [this tutorial](https://www.atlassian.com/git/tutorials/using-branches/git-merge). Merge your `master` branch into your `gh-pages`.

First, checkout your `gh-pages` branch like this:

{% highlight bash %}
git checkout gh-pages
{% endhighlight %}

Now tell git to bring in your new work from your `master` branch like this:

{% highlight bash %}
git merge master
{% endhighlight %}

Now republish your work. If you're not sure how, have a look at [how you published your work the first time](publish-your-code-to-a-website.md#publishing-using-github-pages)?

Don't forget to change back to your `master` branch.
