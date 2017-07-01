---
title: "How to Get Started with Github"
tags:
  - github
  - command-line
  - getting-started
---

# How to Get Started with Github

I have had a few people recently ask for tips and resources on how to get started with using Github so thought I'd share some personal tips.

There are three interrelated components for how I use github:

1.  git
2.  the command line
3.  a text editor (Sublime Text, in my case)

I will discuss how these all work together in the steps below.

## Step by step

There are a few main steps for using GitHub.

# Creating a repository and cloning it on your local machine

1.  Create a repository 

  This is a good [step-by-step guide](https://guides.github.com/activities/hello-world/) for how to create a repository (or "repo" as it is often called) straight from the horse's mouth and it has a good synopsis of what GitHub is. Just follow the "Create a repository step" and don't worry about the branches part just yet.

2.  Go to your repo in github and clone the repository

3.  Open up the terminal and create a folder where you want your code to live
  
  For example, I have a folder called `github`. If you want to try this using the command line, do the following:

  First see which directory you are in by typing:

  `pwd`

  This stands for "print working directory" and it will always tell you where you are. For example, when I type `pwd` I see that I am in the directory `/Users/margotkurfess`, or my home directory.

  If you want your github folder to live in a different directory then use the `cd` ("change directory") command to move to a different directory. If you're not sure what folders are available where you are use the `ls` command to get a list.

  If you are happy creating a github folder where you are, simply type:

  `mkdir github`

4.  In your github folder, clone your new repo

  To get to your new github folder, type the following in terminal:

  `cd github`

  Then clone your repository:

  Copy the link that is in your web browser in github and type the following in terminal:

  `git clone <paste the link>`


# The workflow

Now that you have your repo on your local machin you are ready to start working. This is the point where it becomes really handy to have a good text editor.

