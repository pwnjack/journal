---
id: 429
title: Install different versions of Node JS
date: 2014-10-08T16:00:22+00:00
author: pwnjack
layout: post
guid: http://pwnjack.com/?p=429
permalink: /install-different-versions-node-js/
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
  - 'n'
  - node
  - node version manager
  - nodejs
  - npm
  - nvm
---
How to install different versions of Node JS at the same time?

There&#8217;s an aweosme tool out there that make this task a breeze.

Acqually, there are 2 awesome tools out there:

&#8211; <a href="https://github.com/creationix/nvm" title="nvm" target="_blank">nvm</a>  
&#8211; <a href="https://github.com/visionmedia/n" title="n" target="_blank">n</a>

They are used to achieve the same goal: use different versions of Node, but they are slightly different, but this is not the scope of this post, we are here to explain how to do it.

Although there&#8217;s <a href="http://stackoverflow.com/questions/15462700/nvm-or-n-or-something-else-to-upgrade-node-js" title="n vs nvm" target="_blank">this</a> awesome stackoverflow answer that explains it pretty well.

But let&#8217;s get started!

## n

open your terminal and do as follow:

<pre class="brush: bash; title: ; notranslate" title="">npm install -g n
</pre>

once installed:

<pre class="brush: bash; title: ; notranslate" title="">sudo n 0.10.25
</pre>

This will install Node version 0.10.25

then to use it:

<pre class="brush: bash; title: ; notranslate" title="">sudo n use 0.10.25
</pre>

You are now using node version 0.10.25

There also some helpers like:

<pre class="brush: bash; title: ; notranslate" title="">sudo n stable

sudo n latest
</pre>

For the latest versions, stable and latest, as you can guess.

## nvm

Install it:

<pre class="brush: bash; title: ; notranslate" title="">curl https://raw.githubusercontent.com/creationix/nvm/v0.17.2/install.sh | bash
</pre>

Install desired version:

<pre class="brush: bash; title: ; notranslate" title="">nvm install 0.10
</pre>

Use it:

<pre class="brush: bash; title: ; notranslate" title="">nvm use 0.10
</pre>

or go back to your system version:

<pre class="brush: bash; title: ; notranslate" title="">nvm use system
</pre>