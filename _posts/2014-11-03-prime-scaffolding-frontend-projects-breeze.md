---
id: 445
title: Prime, scaffolding frontend projects is a breeze
date: 2014-11-03T15:26:05+00:00
author: pwnjack
layout: post
guid: http://pwnjack.com/?p=445
permalink: /prime-scaffolding-frontend-projects-breeze/
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
  - news
tags:
  - best practices
  - front-end
  - generator
  - scaffolding
  - workflow
---
Yeoman teaches, and as we know, the apprentice overcome the master sooner or later, no seriously, I made my own front-end web-app generator (sort of) from scratch, keeping it simple, clean, and free of useless junk.

It's called <a href="https://github.com/pwnjack/prime" title="Prime" target="_blank">Prime</a>, you can find it on my <a href="https://github.com/pwnjack" title="Github pwnjack" target="_blank">github profile</a>.

When you develop front-end websites, as I do, you have to follow the good practice for the web standards, and sometime it can be a very tedious task, and here the automation comes in hand.

What you can do:

- Effortless dependencies installation via Bower  
- Real-time update every change in your browser  
- Minimization and optimization for /dist version  
- LESS CSS pre-processor and autoprefixer support

The script is based on <a href="http://bower.io/" title="Bower" target="_blank">Bower</a>, <a href="http://gulpjs.com/" title="Gulp" target="_blank">Gulp</a>, and consequentially, <a href="http://nodejs.org/" title="Node" target="_blank">Node</a>.

Note: You will also need <a href="https://github.com/" title="Github" target="_blank">Github</a> command line tools to download it from the terminal as this guide explains.

If your machine isn't ready yet, install globally Node.

You can download the installer from the <a href="http://nodejs.org/" title="NodeJS" target="_blank">official Node website</a>.

If you use a package manager like <a href="http://brew.sh/" title="Brew" target="_blank">Brew</a>, it's even easier, open the terminal and:

    brew install node

When done, in your terminal shell type:

    npm install -g bower

    npm install -g gulp

At this point you should have your machine ready to use Prime.

To set it up you have to do a couple o things:

- Download it from github

In the terminal shell type:

    git clone http://github.com/pwnjack/prime



- Move inside and install Prime dependencies:

    npm install



Then install you project dependencies (default: jquery, bootstrap, modernizr)

To add new dependencies/packages do so using this format:

    bower install --save <package-name>



When done defining the packages for your project run:

    gulp



Work on your project with your favorite text editor and when your website is ready, build it up for production:

    gulp build



Congratulations, your website is ready to be uploaded on your web host.

Happy coding folks.