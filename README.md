# git-workshop
An exploratory sandbox to discover the magical wonders of git.

---

# Why git?

git is a simple but highly flexible system for keeping track of stuff on one or more computers. But, everyone probably already has some way of doing the same thing. Why should I spend my time learning git?

## How do you keep track of your changing files and documents?

If you're like most academics, you've probably got some version of this extremely versatile naming convention:

1. analysis.R
2. analysis_new.R
3. better_analysis_new.R
4. better_analysis_new_FINAL.R
5. better_analysis_new_FINAL_for_real.R
6. better_analysis_new_FINAL_for_real_for_real.R
7. F*$%^!HF@#KAJVRSAWEOH!#LD.R
8. ...

If you're working with a folder with multiple files changing inside, you probably do the same kind of thing: duplicate the folder and make some changes to some files.

Now, this might be all you need if you've got a fantastic memory. But have you ever come back to one of these sorts of projects after a month, or a year of not looking at it? If so, you probably know that it's basically impossible to tell what the differences between the files are, why they're all different, and which file is *really* the final version.

Thankfully, some programmers got sick of doing this, and they've made a tool to make everyone's lives just that much easier. It's called **git**.

## What does git *do*?
You can think of git as letting you set "save points" for your files, just like you hit save points in video games. Once you hit a save point, you can always go back to that version of your files at any time in the future.

To do this, git will put in a (hidden) folder named `.git` inside your project folder. This `.git` folder keeps a list of all of the save points you've hit in the past. Specifically, it keeps track of which files change and what changes are made between save points. You'll end up with something like the graph below of save-points, where every version is made by changing some previous version. So if you start with a version 1, make some changes for version 2A, make some more changes for version 3A, make some different changes to version 1 for version 2B, and merge together version 3A and version 2B into version 4, git will store this graph:

![You should see an image here...](graph.png)

As you can see, this is pretty useful: your older versions are always there for you to look back on, you can "branch" off into different directions from any version, and you can "merge" different branches with different sets of changes back into a final version.

## What if I'm working with other people, or on multiple computers?
This is where [GitHub](https://github.com) comes in. It's a place where you can put your files online, so that anyone (with access) can download your files, make changes to them, and upload the new version for others.

---

# Terminology

Before we get into the details of using git, let's set up some standard terminology:

| Jargon | Definition |
| :---: | --- |
| Repository | the folder that holds all of your files, as well as a `.git` sub-folder |
| Commit (noun) | a "save-point" that freezes on version of your repository |
| Commit (verb) | To create a new commit local to your computer |
| Branch (noun) | a sequential chain of commits that has a name (e.g., "master") |
| Branch (verb) | to create a new branch |
| Clone | to download a repository from the internet to your computer |
| Checkout | to switch to a commit (or, open a save-point) |
| Fetch  | to update your `.git` folder with changes made online  |
| Pull  | to apply new commits to your old repository- like "Fetch" but also applies new changes |
| Push  | to update the online repository with your new commits  |
| Merge | to mix together two sets of changes from two different branches |

---
# Setup
## Installation

| Windows | Mac OSX | Linux (Ubuntu) |
| ------- | ------- | -------------- |
| 1. [Follow these instructions!](https://gitforwindows.org/)<br> 2. Install [SourceTree](https://www.sourcetreeapp.com/) (optional) | 1. Install [HomeBrew](https://brew.sh/) <br> 2. Open a terminal <br> 3. Type in `brew install git` and press `Enter` <br> - Install [SourceTree](https://www.sourcetreeapp.com/) (optional) | 1. Open a terminal <br> 2. Type in `sudo apt-get install git` and press `Enter` |

## GitHub Registration
1. Sign up for a GitHub account [here](https://github.com/join)
2. Join the [DukeNeuroMethods Organization](https://github.com/DukeNeuroMethods)!

---
