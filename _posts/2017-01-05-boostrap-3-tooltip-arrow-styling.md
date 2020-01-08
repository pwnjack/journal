---
id: 709
title: Boostrap 3 tooltip arrow styling
date: 2017-01-05T19:01:51+00:00
author: pwnjack
layout: post
guid: http://pwnjack.com/?p=709
permalink: /boostrap-3-tooltip-arrow-styling/
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
  - boostrap
  - css
  - tooltip
---
At bootstrap they decided to get tooltip styling even more complicated. To get rid of the black arrow when changing a tooltip&#8217;s background you have to keep in mind the tooltip direction.

e.g.

<pre class="brush: xml; title: ; notranslate" title="">&lt;!-- The markup --&gt;
&lt;a href="#" data-toggle="tooltip" data-placement="bottom"
   title="" data-original-title="Tooltip on bottom"
   class="red-tooltip"&gt;Tooltip on bottom&lt;/a&gt;
</pre>

<pre class="brush: css; title: ; notranslate" title="">/* top tooltip */
.tooltip.top .tooltip-inner {
    background-color: red;
}
.tooltip.top .tooltip-arrow {
      border-top-color: red;
}

/* bottom tooltip */
.tooltip.bottom .tooltip-inner {
    background-color: red;
}
.tooltip.bottom .tooltip-arrow {
      border-bottom-color: red;
}

/* right tooltip */
.tooltip.right .tooltip-inner {
    background-color: red;
}
.tooltip.right .tooltip-arrow {
      border-right-color: red;
}

/* left tooltip */
.tooltip.left .tooltip-inner {
    background-color: red;
}
.tooltip.left .tooltip-arrow {
      border-left-color: red;
}
</pre>

Hurrayyy!!