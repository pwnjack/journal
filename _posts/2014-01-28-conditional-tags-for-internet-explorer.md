---
id: 101
title: Conditional tags for Internet Explorer
date: 2014-01-28T11:22:58+00:00
author: pwnjack
layout: post
guid: http://pwnjack.com/?p=101
permalink: /conditional-tags-for-internet-explorer/
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
  - conditional tags
  - cross-browser
  - css
  - css tags
  - ie
  - internet explorer
  - web design
---
Soemtimes you&#8217;ll need to apply some CSS rules only for Internet Explorer (the worst web browser ever created), this happens because at Microsoft they like to create problems and to be different from the whole world standards. If you are a good boy you MUST sign <a title="Please discontinue Internet Explorer" href="https://www.change.org/petitions/discontinue-internet-explorer" target="_blank">this petition</a> to discontinue Internet Explorer, and save to us (web developers) tons of wasted time.

Anyway if you need to optimize your web project to work with IE also, then you&#8217;ll find this queries pretty useful. They are meant to be used to assign some CSS rules to only Internet Explorer with a conditional tag, you can also specify the IE version on which you&#8217;d like to apply the CSS.

For example:

<pre class="brush: xml; title: ; notranslate" title="">&lt;!–[if IE]&gt; – All IE versions

&lt;!–[if IE 6]&gt; – IE version 6

&lt;!–[if !IE 6]&gt; – All IE versions except version 6

&lt;!–[if gt IE 6]&gt; – All IE versions greater than version 6 (excluded)

&lt;!–[if gte IE 6]&gt; –All IE versions greater than version 6 (included)

&lt;!–[if lt IE 6]&gt; – All IE versions less than version 6 (excluded)

&lt;!—[if lte IE 6]&gt; – All IE versions less than version 6 (included)

</pre>

These above are the opening tags and off course you can use any version number (5, 6, 7, 8, 9, 10, etc.)

Then apply your styles wrapped inside the style tag (because this is used HTML pages):

<pre class="brush: xml; title: ; notranslate" title="">&lt;style&gt;
/* your styles */
&lt;/style&gt;

</pre>

and then close the conditional tag:

<pre class="brush: xml; title: ; notranslate" title="">&lt;![endif]--&gt;

</pre>

You can also, instead of putting the styles directly there as explained above, conditionally link css files, that will apply only if the specified IE version is found.

Like this:

<pre class="brush: xml; title: ; notranslate" title="">&lt;!--[if IE]&gt;
  &lt;link href="ieOnlyStylesheet.css" /&gt;
&lt;![endif]--&gt;
</pre>

This is the common way to solve IE-related problems without messing up the entire project on the other browsers!

Good coding!