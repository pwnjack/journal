---
id: 490
title: Setup a redirect in your hosted website
date: 2015-01-13T17:03:44+00:00
author: pwnjack
layout: post
guid: http://pwnjack.com/?p=490
permalink: /setup-redirect-hosted-website/
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
  - hosting
  - html
  - redirect
---
Create an empty index.html file and paste this string in it to redirect visitors to another desired page.

<pre class="brush: xml; title: ; notranslate" title="">&lt;META HTTP-EQUIV="REFRESH" CONTENT="1; URL=http://www.exampledomainname.com"&gt;
</pre>

Remember to change the destination url to fit your case, obviously.