---
id: 298
title: Gulp JS a sleek streaming build system
date: 2014-05-12T19:55:14+00:00
author: pwnjack
layout: post
guid: http://pwnjack.com/?p=298
permalink: /gulp-js-a-sleek-streaming-build-system/
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
  - build system
  - grunt
  - gulp
  - gulpjs
  - stream
---
Ever wondered if, as front-end developers, we need a building system? Yes we do, definitely.

The most famous is <a href="http://gruntjs.com/" title="Grunt JS" target="_blank">Grunt JS</a>, a very useful task runner written in javascript.

Talking pratical this is a tool that help you build your website in an organized manner, to have a clean and maintanable code. Gulp JS comes in hand infact it have an even more direct approach, it&#8217;s based on the &#8220;stream&#8221; concept, but to better understand how it works i suggest you to check out their <a href="http://gulpjs.com/" title="Gulp JS" target="_blank">official website</a>.

It can become very handy to setup some tedious and repetitive tasks and save you tons of time, infact after configuring the first &#8220;gulpfile&#8221; you need almost nothing more to do, and you could use it for almost every new project if you built it well.

Gulp as a standalone it&#8217;s almost useless but it comes with thousands of community-driven plugins.

To install gulp you can do it using node package manager (npm), after installing <a href="http://nodejs.org/download/" title="Node JS" target="_blank">node.js</a> just open your terminal and type:

<pre class="brush: plain; title: ; notranslate" title="">npm install gulp -g
</pre>

The -g option stands for Globally, so you can use gulp wherever you want in your machine.

Then to install any gulp plugin go in your project&#8217;s folder and simply type (as an example):

<pre class="brush: plain; title: ; notranslate" title="">npm install gulp-less --save-dev
</pre>

Then you are ready to go, you just need to configure your gulpfile for your project and let it do whatever you want, isn&#8217;t that awesome?

To have an in-depth analysis and to see some concrete examples i suggest you to follow <a href="http://markgoodyear.com/2014/01/getting-started-with-gulp/" title="Starting with Gulp JS" target="_blank">this tutorial</a>.

Enjoy and happy coding!