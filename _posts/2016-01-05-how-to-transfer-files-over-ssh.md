---
id: 609
title: How to transfer files over ssh
date: 2016-01-05T19:41:34+00:00
author: pwnjack
layout: post
guid: http://pwnjack.com/?p=609
permalink: /how-to-transfer-files-over-ssh/
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
  - scp
  - ssh copy
---
You need to use &#8220;scp&#8221; (ssh copy), here&#8217;s how.

To copy a file from B to A while logged into B:

<pre class="brush: plain; title: ; notranslate" title="">scp /path/to/file username@a:/path/to/destination
</pre>

To copy a file from B to A while logged into A:

<pre class="brush: plain; title: ; notranslate" title="">scp username@b:/path/to/file /path/to/destination
</pre>