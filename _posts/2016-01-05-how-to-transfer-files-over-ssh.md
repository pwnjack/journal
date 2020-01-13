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
You need to use "scp" (ssh copy), here's how.

To copy a file from B to A while logged into B:

    scp /path/to/file username@a:/path/to/destination

To copy a file from B to A while logged into A:

    scp username@b:/path/to/file /path/to/destination