---
id: 440
title: How to effortlessly install Node on Mac OSX
date: 2014-10-17T18:38:38+00:00
author: pwnjack
layout: post
guid: http://pwnjack.com/?p=440
permalink: /effortlessly-install-node-mac-osx/
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
  - web design
tags:
  - brew
  - install
  - node
  - nvm
---
To install Node with the minimum effort possible follow these instructions and you will be amazed how fast it is.

Install <a href="http://brew.sh" title="Homebrew" target="_blank">Homebrew</a> with this one-liner:

    ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"

Install <a href="http://nodejs.org/" title="NodeJS" target="_blank">Node</a> via Homebrew (NOTE: You don't have to sudo with brew, it does everything for you.)

    brew install node

You are done, but i suggest you to install also <a href="https://github.com/creationix/nvm" title="nvm" target="_blank">nvm</a>, the node version manager.

    curl https://raw.githubusercontent.com/creationix/nvm/v0.17.2/install.sh | bash

With nvm you can easily install different versions of Node and activate them with few commands like:

    nvm install 0.10.32
    nvm use 0.10.32

Or to check what you are currently using if system version or an nvm-driven one.

    nvm ls

To check that everything is installed fine.

    node -v
    npm -v
    nvm --version

If the commands outputs the version numbers, all done.