---
layout: post
title: "Guide - Adding a post using the web client pt.1"
author: ekori
excerpt: "Part one of the step-by-step guide for adding a post using the web interface."
tags: [guide]
comments: true
---

This is a guide written specifically for interacting with the **XPMGla GitHub**. If you would like a general introduction, there are plenty of great guides out there for getting to grips with Git and GitHub. [^1]

####Before you begin...

This guide assumes that you **already have a GitHub account**, but **don't have Git or the client installed on your machine**.

Because it is possible that members of the group might not be able to install the GitHub client on their PC (if they are using a university computer), we have tried to create a workflow for uploading your content to the website using just the browser. This does have limitations, so if you would like to be more involved in the running of the page, you can either use your own machine or ask IT to install the client for you.


##Step 1 - Forking

The first thing you want to do is **fork** from a repository that you want to work on. This creates a copy of the repository under your user, and allows you to make changes without affecting the original repo.

A **repository** or **repo** for short is a "directory or storage space where your projects can live." [^2] For example the [XPMGla](https://github.com/xpmgla) github account has a [repo](https://github.com/xpmgla/xpmgla.github.io) where the webpage is stored. That is where you will be making your changes.
{: .notice}

A **fork** is "a copy of a repository. Forking a repository allows you to freely experiment with changes without affecting the original project." [^3]
{: .notice}

###To fork a copy of the **XPMGla** repo:

1. First, make sure that you are signed in to GitHub
2. Go to the XPMGla website [repo](https://github.com/xpmgla/xpmgla.github.io), and click on the **fork** button in the top right-hand corner of the page. It should look like this: ![fork]({{ site.url }}/images/guide-images/fork.png)
3. GitHub will now take you to your forked copy of the repository, which will sit under your own GitHub account. **You can make changes to this repo without any consequences to the original project.**
4. You can make sure that you are looking at your fork by checking the name of the repo at the top-left of the page.
	* You should see a fork symbol, followed by '*your-username*/*repository-name*' underneath which will be 'forked from *original-username*/*repository-name*'.
	* For example: 

![forked repo]({{ site.url }}/images/guide-images/forked-repo2.png)

You are now ready to make changes to the repo, add posts, events, and other content. Any changes you make will have to be approved and merged back into the original XPMGla repo before they appear on the page, so you are free to experiment with your own fork as much as you want.

To continue reading about adding a post to the XPMGla page, move on to **[Adding a post using the web client pt.2]({{ site.url }}/guide-adding-a-post-2/).**

---

[^1]:[Hello world](https://guides.github.com/activities/hello-world/) / [GitHub flow](https://guides.github.com/introduction/flow/) / [Using Git Cheatsheet](https://gist.github.com/hofmannsven/6814451) / [Atlassian's Git Tutorial](https://www.atlassian.com/git/tutorials)
[^2]: [ReadWrite - Understanding GitHub Pt.1](http://readwrite.com/2013/09/30/understanding-github-a-journey-for-beginners-part-1)
[^3]: [GitHub Help - Fork a Repo](https://help.github.com/articles/fork-a-repo/)
