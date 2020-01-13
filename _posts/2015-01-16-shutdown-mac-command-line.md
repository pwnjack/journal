---
id: 508
title: Shutdown your mac from command line
date: 2015-01-16T18:48:29+00:00
author: pwnjack
layout: post
guid: http://pwnjack.com/?p=508
permalink: /shutdown-mac-command-line/
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
  - cli
  - mac
  - shutdown
  - terminal
---
Here's how you can shutdown your Mac from the command line interface, remember that you must have administration privileges to do so, infact every command must be prefixed with "sudo".

Shutdown now:

    sudo shutdown -h now

Reboot now:

    sudo shutdown -r now

Shutdown at 9pm:

    sudo shutdown -h 21:00

Shutdown in 5 minutes:

    sudo shutdown -h +5