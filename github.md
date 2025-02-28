# git and github (2025)

[**git**](https://xkcd.com/1597/) is arguably the most common Version
Control System on the market and very popular with Open Source
Software. https://github.com is one of the [major
contenders](https://en.wikipedia.org/wiki/Comparison_of_source-code-hosting_facilities),
although gitlab and bitbucket offer competative interfaces to maintain
your git repository. For private use you can also use git on
personal laptop or a home network. Obviously for collaboration something
like *github* is the way to go.

In this class you will learn git, and how to use github to maintain a
git repository, but if you already use another host, feel free to use
it. We will use git to submit the labs and the final project.

Even if these terms makes sense to you, we will **not** use git *branches*, or
learn how to submit a *pull request*, or force *main branch protection*.
In git terminology, all w/e need is:  clone, add, commit, pull and push. Maybe fork.

## Installation

### GUI: GitHub Desktop

Github has a nice GUI frontend to git called *GitHub Desktop*, which you can install
from https://desktop.github.com if you use Mac or Windows. This application greatly simplifies working with Git.

Linux users can get it from https://github.com/shiftkey/desktop/releases

### CLI: Linux / Mac / Win

With Linux, Mac or Window+WSL (Windows subsystem for Linux)
git is already included as a command. Try the command **git \-\-version** in
a terminal and you should see something like 2.34.1 - the exact version does not matter for
us very much. There is also an official "Github CLI", usually installed as the command
**gh**.  Nobody in class should need to use the CLI version, though it can be useful
for power users with fast fingers.


## Steps

0. Create an account on github.com and share your username with the instructors.
   This was already part of your Homework 1. You will probably be asked to set up 2FA.

1. Fork our existing repo from https://github.com/astroumd/PHYS265-spring25 into your personal github space.
   Keep the same name!

2. You should now be in your own https://github.com/Your_Github_Name/PHYS265-spring25 repository.

3. Notice the Lab1, Lab2, Lab3 and Project folders in the **Code** tab along the top.
   You submitted work will be in those folders.

4. Use File -> Clone Repository in the Github Desktop to get a local copy on your laptop.

5. Modify the NAME file, and complete it by puting your name in it.
   Upload this file back to github but first committing
   it to the **main** branch (blue button bottom left), after which on the right side you will see your
   pending actions, in this case **Push Origin**.

6. Update this repo with a **pull**, on Desktop it's called **fetch**. Most often there is nothing.
   Look at the *History* tab
   on the top left when the latest file was modified/added. You can also view differences between
   successive versions of the files.

7. New files you created will show up with the green + symbol to the right of the file in your left pane.
   Fill out a small description in the bottom part. This is important to keep track of why/what you
   committed this change.
   You now will see an option to push this change to the origin. A blue button in the right pane.
   Go ahead and commit this to github.


8. (optional) Create a public README.md file in your own github.com/yourname/yourname repository.
   For example look at my barebones one   https://github.com/teuben/teuben/   but there are many
   better examples online.

This document printed from: https://github.com/astroumd/PHYS265-spring25/blob/main/github.md

## Authentication (advanced)

This applies to the web interface

As of January 2024 github will enforce 2FA (two-factor authentication). Although you will find
everything you need to know to work with github on their website, there are numerous
web pages summarizing this. One example is on https://swcarpentry.github.io/git-novice/ which
covers the all important
[*Installing Git*](https://swcarpentry.github.io/git-novice/#installing-git)
and
[*Creating a GitHub Account*](https://swcarpentry.github.io/git-novice/#creating-a-github-account)
to get your started on Linux, Mac, or Windows.

To summarize, there are two methods how to automate your authentication with github:

### 1. Personal Access Tokens

Settings -> Developer Setting  -> Personal access tokens -> Tokens (classic) -> generate new token

https://github.com/settings/tokens

Typically you will get a token, something like

      ghp_blablablabla

that you will then use as a password. When it was generated, you also had to give it a lifetime. Pick one year,
or anything you prefer.

### 2. SSH keys

Settings -> SSH and GPG keys -> new SSH key

https://github.com/settings/keys

*There is more to come here how keys are generated with **ssh-keygen** and **ssh-copy-id**

## Class Repository

Our public class repository is available via two different style links: http and git:

      https://github.com/astroumd/PHYS265-spring25

      git@github.com:astroumd/PHYS265-spring25.git

