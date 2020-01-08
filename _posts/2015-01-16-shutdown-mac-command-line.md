---
id: 508
title: Shutdown your mac from command line
date: 2015-01-16T18:48:29+00:00
author: pwnjack
layout: post
guid: http://pwnjack.com/?p=508
permalink: /shutdown-mac-command-line/
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
  - cli
  - mac
  - shutdown
  - terminal
---
Here&#8217;s how you can shutdown your Mac from the command line interface, remember that you must have administration privileges to do so, infact every command must be prefixed with &#8220;sudo&#8221;.

Shutdown now:

<pre class="brush: plain; title: ; notranslate" title="">sudo shutdown -h now
</pre>

Reboot now:

<pre class="brush: plain; title: ; notranslate" title="">sudo shutdown -r now
</pre>

Shutdown at 9pm:

<pre class="brush: plain; title: ; notranslate" title="">sudo shutdown -h 21:00
</pre>

Shutdown in 5 minutes:

<pre class="brush: plain; title: ; notranslate" title="">sudo shutdown -h +5
</pre>