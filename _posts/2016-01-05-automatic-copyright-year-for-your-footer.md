---
id: 605
title: Automatic copyright year for your footer
date: 2016-01-05T05:22:00+00:00
author: pwnjack
layout: post
guid: http://pwnjack.com/?p=605
permalink: /automatic-copyright-year-for-your-footer/
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
  - auto-update
  - copyright
  - year
---
Here&#8217;s a snippet that comes in handy when you need to write the current year in the footer and you want it to be always up to date.

PHP:

<pre class="brush: php; title: ; notranslate" title="">// Current year
&copy; &lt;?php echo date("Y") ?&gt;

// With starting year
&copy; 2015-&lt;?php echo date("Y") ?&gt;
</pre>

&nbsp;  
jQuery:

<pre class="brush: jscript; title: ; notranslate" title="">// Store year variable
var currentYear = (new Date).getFullYear();

// Apply text to id element with jQuery
$('#footerYear').text(currentYear);
</pre>

&nbsp;  
And Vanilla Javascript, because why not.

<pre class="brush: jscript; title: ; notranslate" title="">var d = new Date();
	var n = d.getFullYear();
	document.getElementById("year").innerHTML = n;
</pre>