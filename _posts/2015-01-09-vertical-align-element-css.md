---
id: 481
title: Vertical align an element with CSS
date: 2015-01-09T17:47:41+00:00
author: pwnjack
layout: post
guid: http://pwnjack.com/?p=481
permalink: /vertical-align-element-css/
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
  - web design
tags:
  - center
  - element
  - vertical-align
---
Here is the CSS code and remember that to preserve image quality (due to the half-pixel transformation issue) you have to apply this code to the parent element:

<pre class="brush: css; title: ; notranslate" title="">.parent-element {
  -webkit-transform-style: preserve-3d;
  -moz-transform-style: preserve-3d;
  transform-style: preserve-3d;
}

.element {
  position: relative;
  top: 50%;
  -webkit-transform: translateY(-50%);
  -moz-transform: translateY(-50%);
  transform: translateY(-50%);
}
</pre>