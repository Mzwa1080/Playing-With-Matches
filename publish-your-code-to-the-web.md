---
layout: default
---

<h1 data-task-number="5">Publish your code to a website</h1>

> In this task, you'll use a special feature of GitHub to publish your work to the web.

Now we're going to publish your work to a website using [GitHub Pages](https://pages.github.com/), so that you can demo your work. If you have a git branch called `gh-pages` in a repository that you have pushed to GitHub, GitHub will publish the static HTML, CSS, and JavaScript for you at at `<username>.github.io`. You can use this for any static content, but not for applications that require a server.

## Branches

In the terminal, change to your project folder and type

```
git branch
```

to see a list of your branches. You should see only one branch called `master`.
Now create a new branch called `gh-pages`, like this:

```
git branch gh-pages
```

This tells git to make a new branch called `gh-pages` based on your current branch (which is `master`).

Now do `git branch` again. What do you see? Does `git branch` tell you which branch you are on?

To move into your new branch, type:

```
git checkout gh-pages
```

Any commits you make now will be on the `gh-pages` branch (and won't show up on `master`). You'll be using this branch to publish the work you are doing to [GitHub Pages](https://pages.github.com/).

## Publishing using GitHub Pages

To push this branch to GitHub type:

```
git push origin gh-pages
```

<!--codex ignore https-->
GitHub notices that you've pushed a branch called `gh-pages`, takes the HTML, CSS, and JavaScript, and publishes it. This can take a minute or two. Your Playing-With-Matches work is now published at https://&lt;username&gt;.github.io/Playing-With-Matches.

After you've done this you should checkout the master branch again by doing:

```
git checkout master
```

## Files we don't need git to watch

Let's learn a bit more about another part of git: [ignoring files](gitignore.html).
