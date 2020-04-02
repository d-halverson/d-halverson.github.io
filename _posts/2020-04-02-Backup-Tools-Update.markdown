---
title: "Backup Tools - Faster Searching and More!"
layout: post
date: 2020-04-02 00:10
image: /assets/images/markdown.jpg
headerImage: false
tag:
- Java
- GitHub
- Backup-Tools
category: blog
author: drewhalverson
description: Updates to master branch published.
---

## Faster Search
I have reworked a lot of the internal methods, and the class structures are now cleaner and faster! Searching for extra files in file systems is now much faster on average cases! Here is a demonstration of the difference in speed that can be seen in a test run on my computer, searching through a directory with about 2TB of data in it (a good number of files and folders):

<iframe width="560" height="315" src="https://www.youtube.com/embed/hh4lt_koxO4" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

## What else changed?
I have also cleaned up the user's experience with interacting with the program. There are now several commands that can be entered (the program continues to accept multiple commands now until the user quits), and more will be added in the future to give the program more functionality, such as finding large files. As of right now, these are the available commands:

## Current commands available to the user:
- ```help```: Prints a list of commands the user has available to them.
- ```quit```: Stops execution of the program.
- ```extra files```: Command for finding extra files in either the "source" or "backup" file directories.
- ```search```: Allows search for a specific filename specified by the user in either the source or backup directories.

---

Read more about it here:
[GitHub Link](https://github.com/d-halverson/File-Backup-Tools)