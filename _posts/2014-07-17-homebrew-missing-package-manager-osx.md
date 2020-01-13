---
id: 356
title: Homebrew, the missing package manager for OSX
date: 2014-07-17T14:17:59+00:00
author: pwnjack
layout: post
guid: http://pwnjack.com/?p=356
permalink: /homebrew-missing-package-manager-osx/
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
  - tool
tags:
  - brew
  - homebrew
  - osx nmap
  - osx package manager
  - osx wget
  - package manager
---
Ever wondered why OSX is missing some very useful CLI programs like "wget" or "nmap"?

Well, no one cares why, but here's the solution: <a href="http://brew.sh/index.html" title="Homebrew" target="_blank">Homebrew</a>, a package manager for OSX.

To install Homebrew open your terminal and run:

    ruby -e "$(curl -fsSL https://raw.github.com/Homebrew/homebrew/go/install)"

Ta dah.

Now how to use it (e.g.):

    brew install wget

And voilà, you are covered.

Don't sudo, it's not needed, Homebrew installs packages to their own directory and then symlinks their files into /usr/local. So you don't need to use sudo.

Enjoy!