---
title: "Backup Tools - Duplicate Files Searching"
layout: post
date: 2020-05-14 10:33
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


# Duplicate Files
I have added support for a "```duplicate files```" command to my Backup-Tools project. This command searches in just one file system (either the "source" or "backup" directories you provide) and locates files that appear more than once anywhere under that directory. When a file is found in two different places, the program looks to see if the file is in either place in the other file system. For example if at "```backup/folder1/file.txt```" and "```backup/folder2/file.txt```", "```file.txt```" is considered duplicate (they must also be the same filesize). Then, the program looks in ```source/folder1``` and ```source/folder2``` to see if ```file.txt``` is in either location. If for example it was located at "```source/folder1/file.txt```", the file that is flagged as the duplicate copy will be at "```backup/folder2/file.txt```" so that if the user decides to delete it, the one at "```backup/folder1/file.txt```" will remain unchanged, and the source and backup filesystems will remain more similar.

## Rebuilding filesystems after deleting files
I also have added code that rebuilds or reloades the internal data structures that represent the source and backup filesystems in the event that the user decides to delete files. For example, before this if someone found some extra files and deleted them, if they ran the extra files command again without restarting the program, it would look like the files are still there even though that they were actually deleted. This issue has been completely fixed and users do not need to worry about restarting the program anytime.

---

Read more at: [GitHub Link](https://github.com/d-halverson/File-Backup-Tools)
