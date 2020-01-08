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

1. First of all update your system&#8217;s software, to do so simply open up the App Store application and install all available updates.

2. Install all needed apps that are:

&#8211; Sublime Text  
&#8211; Firefox (or Chrome)  
&#8211; GitHub  
&#8211; FileZilla  
&#8211; MAMP  
&#8211; NodeJS  
&#8211; iTerm2

3. Install CLI Softwares that are:

Homebrew  
Github (comes as an option while installing the GitHub app)  
Npm (comes with the NodeJS package)  
Gulp  
Bower

4. Customize your installed softwares with plugins and what else is needed, my personal favorites are:

&#8211; Browser Extensions like: AdBlock, Json viewer, Google url shortener

&#8211; Sublime Text&#8217;s Package Control

With wich you can install every ST extension with ease, like:

&#8211; Emmet  
&#8211; jQuery Snippets  
&#8211; Enhanced Sidebar  
&#8211; SetiUI (UI theme)  
&#8211; Less Syntax Highlighting

5. Now your machine is ready, whenever you want to start a new project simply download the frontend script to setup a full frontend development workflow and all it&#8217;s needed assets with these commands:

Open your terminal and type:

<pre class="brush: plain; title: ; notranslate" title="">git clone http://github.com/pwnjack/prime.git

    cd prime

    npm install && bower install
</pre>

This will take a while, then:

<pre class="brush: plain; title: ; notranslate" title="">gulp
</pre>

And everything will start and you will be ready to develop as smooth as it&#8217;s possible featuring a lot of usefull plugins, to have a full explanation of what the script does, and what it sets up, you can find the documentation by following this [link](http://pwnjack.com/prime-scaffolding-frontend-projects-breeze/ "Prime, scaffolding frontend projects is a breeze").