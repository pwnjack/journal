---
id: 303
title: Remotely connect to a computer via ssh
date: 2014-05-15T18:28:06+00:00
author: pwnjack
layout: post
guid: http://pwnjack.com/?p=303
permalink: /remotely-connect-computer-via-ssh/
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
  - hack
  - tech
tags:
  - remote control
  - ssh
---
The most popular method of connecting via remote control to a machine is the ssh protocol.

It allows you to have total control of a computer from the command line, so if you know how, you can do (almost) everything.

First of all you need to know that prior to the ssh protocol the most used was the telnet, but it's not secure, infact the difference is that ssh use an encrypted connection.

Let's see how to do it.

First of all you have to make sure the ssh protocol is enabled on the computer to be controlled (hacking is not only technical, is also social engineering, keep this in mind), then, from any other computer in the same network (if not you have to jump over a bunch of firewalls, usually, so the thing becomes pretty difficult and is behind the scopre of this article).

When ready open your terminal and type:

    ssh username@ipaddress

You will be then prompted to insert a password, the host's password. Even if it's not appearing while you type go on normally, it's normal.

to show a valid example:

    ssh pwnjack@192.168.1.10

And then you'll be inside the target computer and you can use the terminal exactly as you where on that machine's terminal.

You can do a bunch of awesome stuff for example:

Write a text file and open it on the target computer (scary as fuck for an unsuspecting person)

    nano examplefile.txt

Write whatever you want then CTRL+X to exit, and type yes for save on exit when prompted. Then open the file like this:

    open examplefile.txt -t

Another nice trick you can do is opening a website from the users browser, so for example (Firefox on OSX).

    cd /Applications

This is to move to the Application folder of the target machine.

Then:

    open Firefox.app "http://google.com"

And Firefox will show up and load the specified web page, imagine what you can do!

Use it at your own risk!

Enjoy!