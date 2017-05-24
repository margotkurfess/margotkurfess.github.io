---
title: "How to Get Started with Python"
tags:
  - python
  - data science
---

I have been meaning to write a post like this for a while now and now have an especially good reason to get a beginner's guide to python down on paper. My baby bro has developed an appetite for more advanced data analysis beyond what Excel can provide and I couldn't be more honored to help him out!

So this is a guide for someone who has experience with excel, but no familiariy (yet!) with coding languages.

# Setup

So technically Mac computers come with python installed, but it is a good idea to properly install it to make sure you have the production-stable version and to also get an idea of what is involved with the more 'backend' side of using coding languages.

The guide I like for this purpose is from the [Hitchhiker's Guide to Python](http://python-guide-pt-br.readthedocs.io/en/latest/starting/install/osx/#install-osx), which is also a [book](https://www.amazon.com/Hitchhikers-Guide-Python-Practices-Development/dp/1491933178/ref=sr_1_1?ie=UTF8&qid=1495588799&sr=8-1&keywords=hitchhiker%27s+guide+to+python) that I often reference (which is helpful, but not necessary at this point). Using this as a base, I will expand this guide to an even more beginner level.

## Command line

The only problem with the hitchhiker's guide is that is assumes knowledge of the command line, which I know I didn't have at this point.

This is [Codeacademy's working definition](https://www.codecademy.com/articles/command-line-commands) of what the command line is:

>"The command line is a text interface for your computer. It's a program that takes in commands, which it passes on to the computer's operating system to run."

The command line (also sometimes referred to as "the terminal" or a "shell") becomes increasingly useful as you code more, but for now it is essential for installing python. 

To use the command line, open up the Terminal application on your computer (or I actually prefer iTerm, but that's more of a style thing). This is already on your computer so either look in the application folder or use the Spotlight function mac and type in 'Terminal'. If it looks like a mixture of what you imagine people who code all day do and like a computer interface from the 80s - *you are in the right place.*

So now that you vaguely know what the command line is and how to find it on your computer, you can begin to take the steps outlined in the Hitchhiker's Guide to Python.

## Installing python

1.  Download XCode

    Download this from the [App Store](https://developer.apple.com/xcode/).
2.  Install Homebrew
    
    Using the command line, run the following command:
    ```$ /usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"```
3.  Download Sublime Text 3

    Click the download link for your operating system (in the case of Mac, OSX) using [this link](https://www.sublimetext.com/3).
4.  Insert the Homebrew directory at the top of your PATH environment variable

    This step is kind of complicated and I still find myself googling how to do this from time to time to make sure I'm doing it correctly. 
    - Open up Sublime Text (you can use any text editor, but I recommended downloading Sublime because I have a very strong preference for it over, for example, TextEdit)
    - Open your user folder (in my case, that is 'margotkurfess') within Sublime
    - Find the file `bash_profile` and open that up
    - Paste the following in at the top:
    ```export PATH=/usr/local/bin:/usr/local/sbin:$PATH```
    - Save
5.  Install python 2.7

    Run the following code in your Terminal:
    ```$ brew install python```

## Setuptools and pip

Installing Homebrew means that Setuptools and pip are installed for you. To make sure you have the most recent version of pip, run the following line in command line:

```$ pip install --upgrade pip```

## Installing jupyter

Jupyter is a web appication that allows you to run python code interactively. I find it to be the most accessible environment for using python and use it on a regular basis. The great thing about it is that, in a nutshell, you can code a bunch of stuff and visually see what that code outputs.

Since you now have the most recent version of pip installed, just run the following line of code in your terminal to install jupyter:

```$ pip install jupyter```

# Pick a topic

Now for the fun stuff. With python and jupyter installed, you can start to play with data and apply these tools to use cases. This is really subject to what you are interested and the type(s) of data you are using. My brother lives in Detroit and has experience in the auto industry so might be interested in analyzing data on all the cars produced in the US over a certain time period or the causes of car accidents over time (to name a couple!).

# Open up a jupyter notebook

Back to the technical stuff. Since you are all set up, try exploring a data question in your jupyter notebook.

To do this, open up your terminal and run the following code:

```jupyter notebook```

This will run a bunch of stuff in your terminal (my understanding is that it is creating a kernal and hosting that kernel on your local server) and it will open up a window in your browser that looks like this:

<center>
<img src="/assets/images/jupyter-directory.jpg" width="100%">
</center>


Find the 'New' dropdown and select 'Python 2' to create a new notebook. The new notebook should look like this:

<center>
<img src="/assets/images/jupyter-notebook.jpg" width="100%">
</center>


The `In []:` code cell is where you write your code. When you run the code cell (`Shift`+`Enter`), it will run the code. If the code you wrote in the cell is something that should produce something visual, that will show in an `Out []:` cell immediately below it. 

As an example of this, try running the code:
```print("Hi! This is what code looks like.")```

If you are feeling really keen and want to learn the keyboard shortcuts for jupyter notebook, now is as good a time as any as they will always save you time and mousing around ([link here](https://www.cheatography.com/weidadeyue/cheat-sheets/jupyter-notebook/)).

# Explore your topic

Use the jupyter notebook to explore the topic you picked!

I have created a [template notebook](https://github.com/margotkurfess/reference/blob/master/example_notebook.ipynb) as a starting point to do exactly this.

The general structure is this:

- Import the packages you need (pandas is basically the bread and butter for data analysis)
- Import a data file
- Explore the data set
- Try to answer a couple of questions about the data set (the easier the better to start!)

At this point, there will be a lot of trial and error and a LOT of googling. A lot of your answers will probably come from [stackoverflow](https://stackoverflow.com/) or other question forums. If you need any extra help, please reach out!