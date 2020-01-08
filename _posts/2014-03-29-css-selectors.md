---
id: 241
title: CSS Selectors
date: 2014-03-29T11:38:13+00:00
author: pwnjack
layout: post
guid: http://pwnjack.com/?p=241
permalink: /css-selectors/
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
  - classes
  - css
  - css3
  - ids
  - pseudo classes
  - selectors
---
The CSS selectors are important so it&#8217;s a good practice to familiarize with them, let&#8217;s understand how they work.

<pre class="brush: css; title: ; notranslate" title="">element</pre>

This is the default selector, you can use any html element like p, a, body, html, h1, etc.

<pre class="brush: css; title: ; notranslate" title="">#id</pre>

The id is unique on your page, so use this only if you want to use it once on you page.

<pre class="brush: css; title: ; notranslate" title="">.class</pre>

The most common, like id but can be used multiple times in your page, i almost use only calsses.

<pre class="brush: css; title: ; notranslate" title="">*</pre>

The asterisk select

<pre class="brush: css; title: ; notranslate" title="">.class p</pre>

This will select the descendant child p of the indicated class.

<pre class="brush: css; title: ; notranslate" title="">.class &gt; p</pre>

Like the example above this, with the only difference that it will select only the first child, not the nested ones.

<pre class="brush: css; title: ; notranslate" title="">.class + p</pre>

This will target the parent element, so in this example it will select the class that contains at least a p.

<pre class="brush: css; title: ; notranslate" title="">.class:hover .class:focus .class:active</pre>

These are status selectors that will be applied respectively on the indicated status of the element, before or after it.

<pre class="brush: plain; title: ; notranslate" title="">ul ~ p</pre>

any p elements, as long as they follow a ul.

<pre class="brush: css; title: ; notranslate" title="">a[title]

</pre>

This is the attribute selector, it will select only the a element that have the indicated attribute.

<pre class="brush: css; title: ; notranslate" title="">p::first-letter

</pre>

These are pseudo-selectors indicated by the double colons (::). In this case it will target only the first letter of every paragraph.

Happy coding!