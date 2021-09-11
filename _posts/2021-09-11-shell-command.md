---
title: 'Useful Shell Commands'
date: 2021-09-11
permalink: /posts/2021/09/shell-command/
tags:
  - linux
  - shell
  - terminal
  - command
---

Count number of fiels in a dir
==============================
- `ls | wc -l`, all regular files/folders just in this dir
- `ls -a | grep ^\\. | wc -l`, all hidden files/folders just in thid dir
- `tree -L 1`, list tree just in this dir, and count number of files and folders respectively
- `find ./ -maxdepth 1 -type f,d | wc -l`, but will match current dir and hidden files/folders
