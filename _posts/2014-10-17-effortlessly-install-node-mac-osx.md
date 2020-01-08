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

1. Install <a href="http://brew.sh" title="Homebrew" target="_blank">Homebrew</a> with this one-liner:

<pre class="brush: plain; title: ; notranslate" title="">ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
</pre>

2. Install <a href="http://nodejs.org/" title="NodeJS" target="_blank">Node</a> via Homebrew (NOTE: You don&#8217;t have to sudo with brew, it does everything for you.)

<pre class="brush: plain; title: ; notranslate" title="">brew install node
</pre>

3. You are done, but i suggest you to install also <a href="https://github.com/creationix/nvm" title="nvm" target="_blank">nvm</a>, the node version manager.

<pre class="brush: plain; title: ; notranslate" title="">curl https://raw.githubusercontent.com/creationix/nvm/v0.17.2/install.sh | bash
</pre>

With nvm you can easily install different versions of Node and activate them with few commands like:

<pre class="brush: plain; title: ; notranslate" title="">nvm install 0.10.32
nvm use 0.10.32
</pre>

Or to check what you are currently using if system version or an nvm-driven one.

<pre class="brush: plain; title: ; notranslate" title="">nvm ls
</pre>

To check that everything is installed fine.

<pre class="brush: plain; title: ; notranslate" title="">node -v
npm -v
nvm --version
</pre>

If the commands outputs the version numbers, all done.