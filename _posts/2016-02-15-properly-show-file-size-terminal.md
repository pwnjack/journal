---
id: 632
title: Properly Show file size in terminal
date: 2016-02-15T20:09:26+00:00
author: pwnjack
layout: post
guid: http://pwnjack.com/?p=632
permalink: /properly-show-file-size-terminal/
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
tags:
  - file size
  - show size
  - terminal
---
Sometimes is difficult to have a quick view on which file is taking all that disk space, at least without opening every single folder to show it&#8217;s size information, which is a tedious task, instead there&#8217;s a quick command to show all file and folder size via terminal, very quickly.

Show current folder total size:

<pre class="brush: bash; title: ; notranslate" title="">du -smh
</pre>



Play with path:

In current folder, show every file&#8217;s size

<pre class="brush: bash; title: ; notranslate" title="">du -smh ./*
</pre>

To understand how the command works you can put it on <a href="http://explainshell.com/explain?cmd=du+-smh" target="_blank">explainshell.com</a>