---
id: 743
title: Getting mad refreshing the page and not seeing changes? Flush your DNS cache
date: 2017-06-15T14:37:16+00:00
author: pwnjack
layout: post
guid: http://pwnjack.com/?p=743
permalink: /getting-mad-refreshing-page-not-seeing-changes-flush-dns-cache/
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
---
Sometimes is frustrating to update remote systems and not being able to notice any change in your browser, even by refreshing the page several times. Whenever you step in to this, you might want to resolve the issue as fast as possible, you can do that by using the following command:

<pre class="brush: bash; title: ; notranslate" title="">// OSX 10.10.x &gt; 10.12.x
sudo killall -HUP mDNSResponder

// Windows
ipconfig /flushdns

// Linux
/etc/init.d/named restart
/etc/init.d/nscd restart
</pre>

&nbsp;

You&#8217;re welcome