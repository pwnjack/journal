---
id: 698
title: 'How to change bootstrap&#8217;s navbar buttons style, in all statuses'
date: 2016-09-05T18:15:27+00:00
author: pwnjack
layout: post
guid: http://pwnjack.com/?p=698
permalink: /change-bootstraps-navbar-buttons-style-statuses/
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
  - bootstrap
  - css
  - navbar
  - selector
  - style
---
Getting mad finding out how to change the styles for every single status of Bootstrap&#8217;s navbar buttons?

Sometimes is frustrating to waste time finding out all of them, in all behaviors (:active, :focus, .open, .dropdown, etc.).

So here&#8217;s an all-in-one selector to change the style of all of them:

<pre class="brush: css; title: ; notranslate" title="">.navbar-default .navbar-nav &gt; .open &gt; a,
.navbar-default .navbar-nav &gt; .open &gt; a:hover,
.navbar-default .navbar-nav &gt; .dropdown a:focus,
.navbar-default .navbar-nav &gt; .open &gt; a:focus {
	background: red;
	color: green;
}
</pre>

You&#8217;re welcome 🙂