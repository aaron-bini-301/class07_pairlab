# Lab 07: Blog App w/ Functional Programming

The concepts of functional programming ("FP") have significantly shaped Computer Science from the early days. Apply some FP concepts to your MVC Blog app.

We'll create an "admin" page that shows statistics on how blog authors are doing. In the end, it should look something like [THIS](https://cf-mvc-blog--class07.aerobatic.io/admin.html).

There are many `TODO` items in this lab's starter code, but they are mostly smaller tasks.

## TODOs: MVP
1. Focus on what's new in the starter code. There is now an admin.html page. There are "`// DONE`" comments. There are new functions in articleView.js. Practice your code-reading skills. Spend about 30 minutes on this, including sandboxing at least two features in the starter code. Sandbox using a new git branch, and sandbox at least one feature in each person's repo.
1. Make sure each of our scripts are properly "enclosed". Wrap the contents of article.js and articleView.js in an IIFE. Set up your IIFE so it receives a parameter to which it can attach behavior. For now, you might want to attach your objects and constructor functions to the `window` object.
1. For both `index.html` and `admin.html` we want to access `Article.all` data, but we'll have different *view* functions to set up each of those pages. Modify the `fetchAll` function so that it takes a `next` parameter: a function that will be called when fetchAll has completed its job of fetching articles.
1. Set up both the index page and the admin page to call `fetchAll` in a way that properly triggers the appropriate page setup methods.
1. Use Handlebars to make a small template for each list item in the "Author Stats" section.
1. Use chained map/reduce calls to transform the data into what you need it to be
1. Finally, fill in author stats using your FP-style data methods.

# TODOs: Stretch Goals
- What statistical analysis would be of interest to you with this data set? Code it!

Find those `TODO` items in the codebase, and tackle each one of them.

## Pair Coding git/GitHub Workflow
The workflow for this lab will follow one of the popular methods used by coders who contribute to open-source projects. A project author welcomes contributions to her/his project, but doesn't want to let "just anyone" make changes directly to the project's code. Instead, contributors **fork** the original project repo, make and track changes, then submit PRs to the author. The author then has the option to accept or not accept PRs on a case-by-case basis. For pair coding, because you're working closely together, you'll review your partner's PRs, then accept the PR.

Use **two repositories** for this lab. Pick one person who'll own the "original" repo, and the other will own a **fork** of the original repo.

Switch off driving/navigating every 20 minutes. Use a timer (e.g. on your cell phone or web app mentioned during lecture).

Below, "Owner" denotes the owner of the "original" repo.

1. Owner: Create a new branch in your local workspace. Copy starter code to the workspace. git a-c-p the new branch.
- Driver: Fork the repo, clone it, switch to the new branch. Set up an upstream repo that tracks the original repo. Start typing. Test as you develop! Do a-c each time a new feature works. You may want to a-c even when just scaffold code for a new feature works.
- When it's time to switch: Driver: Push to GitHub, send PR. Owner: Accept PR, git pull, start driving.
- When it's time to switch again: Owner: push to GitHub, submit PR to master, accept PR. Other person: Update workspace using remote ("git pull upstream &lt;branch name&gt;"), start driving.
- Repeat steps 3 and 4 until done.

## Submit
1. URL for the sandbox app in *your* repo.
2. URL of the final PR. Both coders should submit the same URL.
3. Answers to these questions:
   - How long did this lab take?
   - What was most challenging?
   - What did you learn that you think will be useful to you as a coder?
