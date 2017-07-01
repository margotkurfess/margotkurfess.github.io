---
title: "How to Get Started with Github"
tags:
  - github
  - command-line
  - getting-started
---

I have had a few people recently ask for tips and resources on how to get started with using Github so thought I'd share some personal tips.

There are three interrelated components for how I use github:

1.  git
2.  the command line/terminal (this has lots of names)
3.  a text editor (Sublime Text, in my case)

I will discuss how these all work together in the steps below.

## Step by step

The following guide is for starting to use GitHub for personal use. GitHub is also used as a collaborative tool and was created as a means for multiple people to work on the same project without breaking code by allowing people to work on their own branches, but that will be for another post someday! I have found GitHub to be extremely valuable even just for personal use and I think it can be a great way to get started without the intimidation of working on different branches. 

There are a few main steps to getting started that I will outline below in more detail.

# Creating a repository and cloning it on your local machine

1.  Create a repository 

    This is a good [step-by-step guide](https://guides.github.com/activities/hello-world/) for how to create a repository (or "repo" as it is often called) straight from the horse's mouth and it has a good synopsis of what GitHub is. Just follow the "Create a repository step" and don't worry about the branches part just yet. Just stay on the `master` branch if you are using GitHub for more personal use.

2.  Go to your repo in github and clone the repository

3.  Open up the terminal and create a folder where you want your code to live
  
    For example, I have a folder called `github`. If you want to try to create a folder like this using the command line, do the following:

    First see which directory you are in by typing:

    `pwd`

    This stands for "print working directory" and it will always tell you where you are. For example, when I type `pwd` I see that I am in the directory `/Users/margotkurfess`, or my home directory.

    If you want your github folder to live in a different directory then use the `cd` ("change directory") command to move to a different directory. If you're not sure what folders are available where you are use the `ls` command to get a list.

    If you are happy creating a github folder where you are, simply type:

    `mkdir github`

    (You can also do this step in your Finder window if that is more comfortable!)

4.  In your github folder, clone your new repo

    To get to your new github folder, type the following in terminal:

    `cd github`

    Then clone your repository:

    Copy the link that is in your web browser in github and type the following in terminal:

    `git clone <paste the link>`


# Downloading a good text editor

Now that you have your repo on your local machin you are ready to start working. This is the point where it becomes really handy to have a good text editor. Good text editors make it much easier to read code and come with a ton of useful shortcuts like using multiple cursors to just name one. So find one that you like and don't ever look back to things like TextEdit.

I personally use [Sublime Text 3](https://www.sublimetext.com/3) as my text editor. I have also installed some packages in it to make it easier on the eyes like [Boxy Theme](https://packagecontrol.io/packages/Boxy%20Theme) and [A File Icons](https://github.com/ihodev/a-file-icon) to make it easier to navigate files. I also have friends who swear by [Atom](https://atom.io/) as their text editor, which is pretty and straight off the bat and easy to use.

# Using all three components to store code in your repo

When I started at Spotify I also started using Google BigQuery. BigQuery is amazing in a lot of ways, but one of the major drawbacks is the ability to store code. While you can _technically_ save queries, this feature leaves a lot to be desired and I found myself leveraging GitHub as a way to keep track of useful code. 

So at work I have a whole repo dedicated to queries which I work out of every day. This was especially useful not only as a reference in the beginning as I was learning what code lived where but also as a reference for projects that I have shared with others. 

**My workflow is this:**

1.  Open up terminal and change directory to your cloned repo
  
    `cd github/queries`

2.  Open up Sublime
  
    I actually do this from the terminal using installed packages within [iTerm](https://www.iterm2.com/), which is a Mac terminal replacement. If you are interested in doing this, I followed [this article by Mike Buss](http://mikebuss.com/2014/02/02/a-beautiful-productive-terminal-experience). 

    Otherwise open Sublime to your queries folder.

3.  Start doing work and save any changes

4. Use git commits to save changes

    In terminal:

    ```git add .
    git commit -m "description of the changes you made since your last commit"
    git push origin master
    ```

    It is also good practice before you start working to run the command:

    `git pull origin master`

    This is not really relevant when you are working in your own repo and on the master branch, but becomes more impoartant when you work collaboratively with others. This ensures that you have the lastest version of the `master` branch on your local machine so if anyone has made any changes that would have otherwise conflicted with yours, they will be updated.

5. Rinse & repeat!

# Additional resources

If you are still feeling fuzzy on the command line, this is a great resource:
  [Learn Command Line The Hard Way](https://learnpythonthehardway.org/book/appendixa.html)

And if you run into any trouble with git, this is an encyclopedia for all the git commands:
  [Git docs](https://git-scm.com/docs)

And feel free to reach out with questions!

