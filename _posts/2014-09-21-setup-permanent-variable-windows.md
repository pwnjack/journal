---
id: 418
title: How to setup a permanent variable on Windows
date: 2014-09-21T21:24:49+00:00
author: pwnjack
layout: post
guid: http://pwnjack.com/?p=418
permalink: /setup-permanent-variable-windows/
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
  - cmd
  - enivronment
  - terminal
  - variable
  - windows
---
To setup a permanent environement variable in Windows, for instance if you want to use "nmap" from everywhere and not only in it's specific directory, do as follows:

In CMD set the variable like this:

    setx PATH "%PATH%;C:\Program Files (x86)\Nmap"

Now the variable not only is set-up but is also permanent even if you restart cmd.exe.

Hope this helps.