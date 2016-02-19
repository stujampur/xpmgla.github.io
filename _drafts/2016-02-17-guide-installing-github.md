---
layout: post
title: "Guide - Installing the GitHub client"
author: ekori
excerpt: "Getting started with using GitHub from the command line"
tags: [guide]
comments: true
---

This is a guide written specifically for interacting with the **XPMGla GitHub**. If you would like a general introduction, there are plenty of great guides out there for getting to grips with Git and GitHub. [^1]

#### Before you begin...

This guide assumes that you **already have a GitHub account**, but **don't have Git or the client installed on your machine**. 

It also assumes that you have gone through at least [**part 1 of the GitHub web interface**]({{ site.url }}/guide-adding-a-post-1/) guides. So, before you continue, make sure that you have:

1. An understanding of what a repo, fork and a branch is;
2. Forked from the main [XPMGla repo](https://github.com/xpmgla/xpmgla.github.io);
3. And possibly made some changes and submitting a pull request.

If that's not the case, have a look at parts [1]({{ site.url }}/guide-adding-a-post-1/), [2]({{ site.url }}/guide-adding-a-post-2/), and [3]({{ site.url }}/guide-adding-a-post-3/) of the guide here.


## Step 1 - Installing Git

Git and GitHub are not one and the same. You'll be using both to interact with the XPMGla repo. 

**Git** 'is a very popular and efficient open source Version Control System. It tracks content such as files and directories.'[^2] A good way to think about Git is as 'a series of snapshots (commits)' of any revisions you make to your files. You can examine these snapshots in the order they were created. You can make branches to experiment and come then return to earlier snapshots if you want.[^3]
{: .notice}

**GitHub** 'is a Git repository hosting service, but it adds many of its own features. While Git is a command line tool, GitHub provides a Web-based graphical interface. It also provides access control and several collaboration features, such as a wikis and basic task management tools for every project.'[^4] 
{: .notice}

So, first you have to download and install Git. 

#### Downloading Git

Start by going to the [Git website](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git) and following the instructions there.
---

Terminal, then

`$ git config --global user.name "YOUR NAME"`

`$ git config --global user.email "YOUR EMAIL ADDRESS"`

or 

if you want to keep your email private:

`$ git config --global user.email "username@users.noreply.github.com"`

to check 

`$ git config --global user.email`

should return

`username@users.noreply.github.com`


## Step 2- Installing GitHub

Downloading GitHub is pretty straightforward. GitHub recently released [**GitHub Desktop**](https://desktop.github.com/), which is an all-in-one client that works on both Windows and OSX.

Following the link above should take you the right page for installing GitHub Desktop for your operating system.



**Shell**
{: .notice}

**Command Line**
{: .notice}

**`$`**
{: .notice}


## creating a local clone of your fork

1. On GitHub, navigate to your fork of the XPMGla repository.
2. Under your repository name, click  to copy the clone URL for the repository.
3. Open Terminal (for Mac and Linux users) or the command prompt (for Windows users).
4. Navigate to the folder you want to clone your repo into (cd)
* Type git clone, and then paste the URL you copied in Step 2.
* Press Enter. Your local clone will be created.


## Configure remote

1. navigate into the folder you just cloned
2. check the settings with `$ git remote -v`
3. you should see:
`origin  https://github.com/YOUR_USERNAME/YOUR_FORK.git (fetch)`
`origin  https://github.com/YOUR_USERNAME/YOUR_FORK.git (push)`
4. Go to the original XPMGla repo and copy the clone url
5. Type git remote add upstream, and then paste the URL you copied in Step 4 and press Enter. It will look like this:
`$ git remote add upstream https://github.com/octocat/Spoon-Knife.git`
6. To verify the new upstream repository you've specified for your fork, type git remote -v again. You should see the URL for your fork as origin, and the URL for the original repository as upstream.:
`$ git remote -v`
`origin    https://github.com/YOUR_USERNAME/YOUR_FORK.git (fetch)`
`origin    https://github.com/YOUR_USERNAME/YOUR_FORK.git (push)`
`upstream  https://github.com/ORIGINAL_OWNER/ORIGINAL_REPOSITORY.git (fetch)`
`upstream  https://github.com/ORIGINAL_OWNER/ORIGINAL_REPOSITORY.git (push)`


https://help.github.com/articles/syncing-a-fork/

---

![fork]({{ site.url }}/images/guide-images/fork.png)

To continue reading about adding a post to the XPMGla page, move on to **[Adding a post using the web client pt.2]({{ site.url }}/guide-adding-a-post-2/).**

---

[^1]:[Hello world](https://guides.github.com/activities/hello-world/) / [GitHub flow](https://guides.github.com/introduction/flow/) / [Using Git Cheatsheet](https://gist.github.com/hofmannsven/6814451) / [Atlassian's Git Tutorial](https://www.atlassian.com/git/tutorials)
[^2]:[SiteGround Git Tutorial](https://www.siteground.co.uk/tutorials/git/)
[^3]:[StackOverflow Q&A](http://stackoverflow.com/questions/11816424/understanding-the-basics-of-git-and-github)
[^4]:[Tech Crunch 'What Exactly is GitHub Anyway'](http://techcrunch.com/2012/07/14/what-exactly-is-github-anyway/)
