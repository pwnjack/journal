---
id: 537
title: DotDotDot, jQuery truncate text with ellipsis, even for fluid layouts
date: 2015-04-22T15:51:55+00:00
author: pwnjack
layout: post
guid: http://pwnjack.com/?p=537
permalink: /dotdotdot-jquery-truncate-text-with-ellipsis-even-for-fluid-layouts/
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
  - tool
  - web design
tags:
  - fluid
  - javascript
  - js
  - responsive
  - text
  - truncate
---
Sometimes you'll need to truncate text, with an ending ellipsis. This task can often be a pain, infact plain CSS offer an ellipsis truncation solution with the "text-overflow: ellipsis" parameter, but it works only on the first line of text.

To have a more flexible solution, that works in all cases. Use this neat jquery plugin, called <a title="DotDotDot" href="http://dotdotdot.frebsite.nl/" target="_blank">DotDotDot</a>.

It's very simple to use. Here's how:

On your markup, select a wrapper like this:

    <div id="wrapper">
      <p>Lorem Ipsum is simply dummy text.</p>
    </div>

and instantiate the plugin on the element, on DOM ready:

    $(document).ready(function() {
      $("#wrapper").dotdotdot({
        //	configuration goes here
      });
    });

Then setup an height in CSS for the element, and the plugin will do the rest, if needed, the text will be automatically truncated and ellipsed.

Nice.