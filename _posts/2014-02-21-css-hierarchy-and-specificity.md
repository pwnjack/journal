---
id: 165
title: CSS hierarchy and specificity
date: 2014-02-21T11:16:15+00:00
author: pwnjack
layout: post
guid: http://pwnjack.com/?p=165
permalink: /css-hierarchy-and-specificity/
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
  - css
  - hierarchy
  - specificity
---
Sometimes there's some confusion around the CSS rules and their effectiveness. This post's scope is to clarify how it works and why sometimes it seems you are forced to use:

    !important

In CSS the last declared rule win, but the inline rule win over it, and the !important win over all of them. Then comes in the "specificity" factor, the more specific, the stronger.

Here's an example:

    h1 {font-size: 24px;}

    h1 {font-size: 28px;}

The font will render at 28px.

    body h1 {font-size: 24px;}

    h1 {font-size: 28px;}

The font will render at 24px.

    h1 {font-size: 24px !important;}

    h1 {font-size: 28px;}

The font will render at 24px.

If you want to understand better and go deep in this argument i suggest you to read the w3 official article over <a title="CSS3 Selectors Specificity" href="http://www.w3.org/TR/css3-selectors/#specificity" target="_blank">here</a>.

Happy coding!