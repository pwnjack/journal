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
We developers hate Internet Explorer, for various reasons, one of them is that we have to use specific conditional tag just for it, imagine how bad it is just by that.

Sometimes you'll need to apply some CSS rules only for Internet Explorer (the worst web browser ever created), this happens because at Microsoft they like to create problems and to be different from the whole world standards. If you are a good boy you MUST sign <a title="Please discontinue Internet Explorer" href="https://www.change.org/petitions/discontinue-internet-explorer" target="_blank">this petition</a> to discontinue Internet Explorer, and save to us (web developers) tons of wasted time.

Anyway if you need to optimize your web project to work with IE also, then you'll find this queries pretty useful. They are meant to be used to assign some CSS rules to only Internet Explorer with a conditional tag, you can also specify the IE version on which you'd like to apply the CSS.

For example:

    – All IE versions

    <!–[if IE 6]> – IE version 6

    <!–[if !IE 6]> – All IE versions except version 6

    <!–[if gt IE 6]> – All IE versions greater than version 6 (excluded)

    <!–[if gte IE 6]> –All IE versions greater than version 6 (included)

    <!–[if lt IE 6]> – All IE versions less than version 6 (excluded)

    <!—[if lte IE 6]> – All IE versions less than version 6 (included)

These above are the opening tags and off course you can use any version number (5, 6, 7, 8, 9, 10, etc.)

Then apply your styles wrapped inside the style tag (because this is used HTML pages):

    <style>
      /* your styles */
    </style>

and then close the conditional tag:

    <![endif]-->

You can also, instead of putting the styles directly there as explained above, conditionally link css files, that will apply only if the specified IE version is found.

Like this:

    <!--[if IE]>
      <link href="ieOnlyStylesheet.css" />
    <![endif]-->

This is the common way to solve IE-related problems without messing up the entire project on the other browsers!

Good coding!