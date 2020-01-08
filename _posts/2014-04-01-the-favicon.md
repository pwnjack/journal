---
id: 251
title: The Favicon
date: 2014-04-01T11:03:45+00:00
author: pwnjack
layout: post
guid: http://pwnjack.com/?p=251
permalink: /the-favicon/
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
  - favicon
  - icon
  - x-icon
---
Sometimes people forget about the favicon, that nice tiny icon on the tab of our browser that will also serve as an icon when you save the website on your favorites.

How to have a cross-browser 100% working favicon? Let&#8217;s see.

First of all you have to indicate in your markup the location of your favicon file with this snippet inside your <head>:

<pre class="brush: xml; title: ; notranslate" title="">&lt;link rel="shortcut icon" href="favicon.ico" type="image/x-icon"&gt;
</pre>

Remember that if you don&#8217;t specify where the favicon is with this snippet the browser will guess that it&#8217;s on the root folder (/), but it&#8217;s a good pratice to indicate it also when it&#8217;s in the default location.

You have to remember that the favicon to be cross-browser compatible must be an _.ico_ file, and not a _.png_.  
To have such file just create your favicon in Photoshop or any other image manipulation software and save it as a _.png_ at 16&#215;16 pixels. When you are done save it and import it in this useful online tool called <a title="ICO Converter" href="http://www.icoconverter.com/" target="_blank">ICO Converter</a>.

It will convert your _.png _ file in to the _.ico _ format, good for any browser as a favicon (even the damn IE).

Enjoy!