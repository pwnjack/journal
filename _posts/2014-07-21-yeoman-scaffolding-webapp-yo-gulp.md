---
id: 359
title: Yeoman, scaffolding your webapp with Yo and Gulp
date: 2014-07-21T12:12:39+00:00
author: pwnjack
layout: post
guid: http://pwnjack.com/?p=359
permalink: /yeoman-scaffolding-webapp-yo-gulp/
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
  - web design
tags:
  - bower
  - front-end
  - grunt
  - gulp
  - scaffolding
  - workflow
  - yeoman
---
There&#8217;s an awesome scaffolding assistant out there, his name is Yeoman, he works just fine out-of-the box but I personally prefer Gulp over Grunt, so I thought it could be interesting to share <a href="https://github.com/yeoman/generator-gulp-webapp" title="Yeoman Gulp Generator" target="_blank">this project</a>.

This generator for Yeoman is made with Gulp instead of Grunt, it&#8217;s still in development but it&#8217;s already pretty usable, give it a try!

First of all install Yeoman via npm

<pre class="brush: plain; title: ; notranslate" title="">sudo npm install -g yeoman
</pre>

Then install the generator (globally)

<pre class="brush: plain; title: ; notranslate" title="">sudo npm install -g generator-gulp-webapp
</pre>

Then cd to your project&#8217;s folder and run it:

<pre class="brush: plain; title: ; notranslate" title="">yo gulp-webapp
</pre>

Now install your dependencies via Bower (e.g.):

<pre class="brush: plain; title: ; notranslate" title="">bower install --save magnific-popup
</pre>

Wire up your deps in index.html

<pre class="brush: plain; title: ; notranslate" title="">gulp wiredep
</pre>

Start the watch task and start editing and previewing in your browser:

<pre class="brush: plain; title: ; notranslate" title="">gulp watch
</pre>

When your app is ready to deploy, build it.

<pre class="brush: plain; title: ; notranslate" title="">gulp build
</pre>

The &#8220;dist&#8221; folder will be generated and ready to be published.

This is an awesome front-end development workflow, isn&#8217;t it? Yeah!!!

Enjoy you personal scaffolding assistant, Yeoman with Gulp!