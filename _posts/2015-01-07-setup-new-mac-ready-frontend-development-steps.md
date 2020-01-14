---
id: 475
title: How to setup your new Mac to be ready for frontend development in few steps
date: 2015-01-07T18:55:42+00:00
author: pwnjack
layout: post
guid: http://pwnjack.com/?p=475
permalink: /setup-new-mac-ready-frontend-development-steps/
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
  - development
  - frontend
  - mac
  - machine
  - setup
  - softwares
---
Setup your machine for frontend development (Mac)

1. First of all update your system's software, to do so simply open up the App Store application and install all available updates.

2. Install all needed apps that are:
- Sublime Text  
- Firefox (or Chrome)
- GitHub  
- FileZilla  
- MAMP  
- NodeJS  
- iTerm2

3. Install CLI Softwares that are:
- Homebrew  
- Github (comes as an option while installing the GitHub app)  
- Npm (comes with the NodeJS package)  
- Gulp  
- Bower

4. Customize your installed softwares with plugins and what else is needed, my personal favorites are:
- Browser Extensions like: AdBlock, Json viewer, Google url shortener
- Sublime Text's Package Control

5. With wich you can install every ST extension with ease, like:
- Emmet  
- jQuery Snippets  
- Enhanced Sidebar  
- SetiUI (UI theme)  
- Less Syntax Highlighting

6. Now your machine is ready, whenever you want to start a new project simply download the frontend script to setup a full frontend development workflow and all it's needed assets with these commands:

Open your terminal and type:

    git clone http://github.com/pwnjack/prime.git

    cd prime

    npm install && bower install

This will take a while, then:

    gulp

And everything will start and you will be ready to develop as smooth as it's possible featuring a lot of usefull plugins, to have a full explanation of what the script does, and what it sets up, you can find the documentation by following this [link](http://pwnjack.com/prime-scaffolding-frontend-projects-breeze/ "Prime, scaffolding frontend projects is a breeze").