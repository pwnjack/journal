---
id: 406
title: How to setup a permanent alias in OSX Terminal
date: 2014-09-15T15:52:23+00:00
author: pwnjack
layout: post
guid: http://pwnjack.com/?p=406
permalink: /setup-permanent-alias-osx-terminal/
quote_link:
  - ""
other_media:
  - ""
video_link:
  - ""
main_video:
  - ""
video_hosted:
  - ""
video_hosted_ogv:
  - ""
categories:
  - tech
tags:
  - alias
  - cli
  - command
  - terminal
---
If you are a terminal guy you probably already know about aliases, an alias is a shortened command, something like:

    alias desk="cd ~/Desktop"

This sortcut let you type just "desk" to go inside your Desktop directory through the terminal, from anywhere.

The problem is that the alias is lost if you close the terminal and start it again, so how to make it permanent?

Go in your home folder by typing just "cd" in your terminal, then use "nano" to open a file named .bash_profile (if it doesn't exist create one), the file is invisible so to see it you have to use the command "ls -a", open it and add the line there, save and quit. Now your alias is permenent.

If you are using something like "zsh" as a terminal shell, you have to do the same thing but instead on a file named .zshrc.

Enjoy.