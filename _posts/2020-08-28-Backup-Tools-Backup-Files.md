---
title: "Backup Tools - Backing Up Files"
layout: post
date: 2020-08-28 13:16
image: /assets/images/markdown.jpg
headerImage: false
tag:
- Java
- GitHub
- Backup-Tools
category: blog
author: drewhalverson
description: Published Backup Tools project to GitHub!
---


# Backing Up Files
In the past, I was using a separate program that backed up my files to my backup hard drive, and then I began to develop this project so that I can identify and delete files on the backup hard drive that I already deleted on the source hard drive because that feature was not present in the program I was using. Anyways, since then I have added duplicate file searching, generic file searching, and now I have implemented the first version of backing up files. This means that I can just use this program on its own without the need for the old program I was using. Now, I can backup files from the source to the backup with "```backup files```", and when I delete files on the source, I can use the "```extra files```" command to also have them deleted on the backup drive. As I look to improve this functionality, I want to allow the user to also be able to select only some of the files found to be backed up when using backup and extra files commands, similarly to how "```duplicate files```" performs right now.

# Other Features for the Future
Aside from improving the extra files command, I also want to add a command for finding large files and folders in either hard drive. If the user is trying to free up space, the program could then find some of the files and/or folders that are taking up the most space, and could be deleted if the user wants them to be.

---

Read more at: [GitHub Link](https://github.com/d-halverson/File-Backup-Tools)
