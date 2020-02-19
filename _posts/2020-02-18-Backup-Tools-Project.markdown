---
title: "Backup Tools Project"
layout: post
date: 2020-02-18 20:28
image: /assets/images/markdown.jpg
headerImage: false
tag:
- Java
- GitHub
category: blog
author: drewhalverson
description: Published Backup Tools project to GitHub!
---


# First Official GitHub Project
Although I have made many personal coding projects in the past for my own fun and learning, this time I had the end goal of publishing it for others to use and be able to read. Right now this project is in a very early state and I still plan on adding much more to it later; it is currently in a "minimum viable product" state. Anyways, here is some information regarding the project:

# Backup Tools
This project will provide various tools to manage a file backup system. It is currently in its first basic version, and serves one purpose: to identify files deemed "extra" in a backup filesystem and delete them if wanted. The source folder described in this program is a folder that will be the template and the backup folder is where the extra files are being searched for; any file that is found in backup or in a folder inside of backup and is not found anywhere inside the source folder is flagged as extra.

Right now the program isn't extremely efficient, but the next step as I move forward is to implement the truly interesting piece. Right now each file system designated by source and backup folders as root is stored in a custom tree data structure. Next I plan on changing the traversal order of these trees when searching for a file in the contains method to be "smart" instead of linear. By "smart," I mean that I want the program to choose which folder it should start looking in based on the name of the file it's looking for and the names of the folders it has to choose from. For example, if it was looking for "Christmas_Picture_2019.png," it should start looking in folders like "Christmas" or "Xmas 2019" instead of a folder like "homework."

Information on running in Terminal: 
- Install latest version of JDK from Oracle's website
- Change your working directory to be in the bin folder of this project
- Run the command: {% highlight html %}java BackupTools{% endhighlight %}
- Follow onscreen instructions. 

Language: 100% Java ☕

[GitHub Link](https://github.com/d-halverson/File-Backup-Tools)

---

Disclaimer: Be careful! Run at your own risk, and only point to folders that you are ok with potentially losing data in if you want to test my project and be safe.