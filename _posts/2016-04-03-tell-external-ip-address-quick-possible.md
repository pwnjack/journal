---
id: 660
title: Tell me my external ip address, as quick as possible
date: 2016-04-03T19:18:55+00:00
author: pwnjack
layout: post
guid: http://pwnjack.com/?p=660
permalink: /tell-external-ip-address-quick-possible/
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
  - external ip
  - ip
  - ip address
  - tell me my ip
---
Need to know your external ip address as quick as possible? I found this website to be the cleanest and fastest solution.

<pre class="brush: plain; title: ; notranslate" title="">http://icanhazip.com
</pre>

I love it because it returns just plain text without ads or extra data.

This means that you can easily obtain the result from the terminal too, or programmatically, the geeks out there will love this (e.g.).

<pre class="brush: bash; title: ; notranslate" title="">curl http://icanhazip.com
</pre>

I appreciate the small things in life.

Some extra goodies:

<pre class="brush: bash; title: ; notranslate" title=""># returns the reverse DNS record for you ip
icanhazptr.com

# returns a traceroute
icanhaztrace.com

# returns Epoch time (for real nerds)
icanhazepoch.com

# can determine if your traffic is being proxied
icanhazproxy.com
</pre>

Thanks to the <a href="http://major.io" target="_blank">author</a> of these tools.