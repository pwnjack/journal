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

It&#8217;s called <a href="https://github.com/pwnjack/prime" title="Prime" target="_blank">Prime</a>, you can find it on my <a href="https://github.com/pwnjack" title="Github pwnjack" target="_blank">github profile</a>.

When you develop front-end websites, as I do, you have to follow the good practice for the web standards, and sometime it can be a very tedious task, and here the automation comes in hand.

What you can do:

&#8211; Effortless dependencies installation via Bower  
&#8211; Real-time update every change in your browser  
&#8211; Minimization and optimization for /dist version  
&#8211; LESS CSS pre-processor and autoprefixer support

The script is based on <a href="http://bower.io/" title="Bower" target="_blank">Bower</a>, <a href="http://gulpjs.com/" title="Gulp" target="_blank">Gulp</a>, and consequentially, <a href="http://nodejs.org/" title="Node" target="_blank">Node</a>.

Note: You will also need <a href="https://github.com/" title="Github" target="_blank">Github</a> command line tools to download it from the terminal as this guide explains.

If your machine isn&#8217;t ready yet, install globally Node.

You can download the installer from the <a href="http://nodejs.org/" title="NodeJS" target="_blank">official Node website</a>.

If you use a package manager like <a href="http://brew.sh/" title="Brew" target="_blank">Brew</a>, it&#8217;s even easier, open the terminal and:

<pre class="brush: plain; title: ; notranslate" title="">brew install node
</pre>

When done, in your terminal shell type:

<pre class="brush: plain; title: ; notranslate" title="">npm install -g bower

npm install -g gulp
</pre>

At this point you should have your machine ready to use Prime.

To set it up you have to do a couple o things:

&#8211; Download it from github

In the terminal shell type:

<pre class="brush: plain; title: ; notranslate" title="">git clone http://github.com/pwnjack/prime
</pre>

&#8211; Move inside and install Prime dependencies:

<pre class="brush: plain; title: ; notranslate" title="">npm install
</pre>

Then install you project dependencies (default: jquery, bootstrap, modernizr)

To add new dependencies/packages do so using this format:

<pre class="brush: plain; title: ; notranslate" title="">bower install --save &lt;package-name&gt;
</pre>

When done defining the packages for your project run:

<pre class="brush: plain; title: ; notranslate" title="">gulp
</pre>

Work on your project with your favorite text editor and when your website is ready, build it up for production:

<pre class="brush: plain; title: ; notranslate" title="">gulp build
</pre>

Congratulations, your website is ready to be uploaded on your web host.

Happy coding folks.