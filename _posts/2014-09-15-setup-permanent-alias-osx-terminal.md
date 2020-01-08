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

<pre class="brush: bash; title: ; notranslate" title="">alias desk="cd ~/Desktop"
</pre>

This sortcut let you type just &#8220;desk&#8221; to go inside your Desktop directory through the terminal, from anywhere.

The problem is that the alias is lost if you close the terminal and start it again, so how to make it permanent?

Go in your home folder by typing just &#8220;cd&#8221; in your terminal, then use &#8220;nano&#8221; to open a file named .bash_profile (if it doesn&#8217;t exist create one), the file is invisible so to see it you have to use the command &#8220;ls -a&#8221;, open it and add the line there, save and quit. Now your alias is permenent.

If you are using something like &#8220;zsh&#8221; as a terminal shell, you have to do the same thing but instead on a file named .zshrc.

Enjoy.