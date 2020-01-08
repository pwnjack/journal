---
id: 694
title: Convert multiple png images to a single multi-sized ico for the favicon
date: 2016-07-05T13:48:12+00:00
author: pwnjack
layout: post
guid: http://pwnjack.com/?p=694
permalink: /convert-multiple-png-images-single-multi-sized-ico-favicon/
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
  - convert ico
  - favicon
  - png
---
Nowadays you&#8217;ll need your favicon to be from 16&#215;16 to 48&#215;48 (at least). Sometimes converting all your png images to ico is a tedious task, right now I was using online services to do so, plenty of friendly ico converters out there. But, when you have to do it your way, it&#8217;s a lot simpler to use a command line tool to be more quick and efficient.

Here comes &#8220;imagemagick&#8221;, an awesome CLI software that a lot of tools use under the hood.

If you are on Mac you can easily install it with brew:

<pre class="brush: plain; title: ; notranslate" title="">brew install imagemagick
</pre>

When installed you can convert your multiple png images to a single all-in-one .ico file to use as a favicon.

Use the following syntax:

<pre class="brush: plain; title: ; notranslate" title="">convert image-16.png image-24.png image-48.png favicon.ico
</pre>

And the tool will do the conversion for you. As simple as that, awesome, isnt&#8217;it?