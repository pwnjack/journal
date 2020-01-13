---
id: 35
title: Media queries
date: 2014-01-21T11:18:04+00:00
author: pwnjack
layout: post
guid: http://pwnjack.com/?p=35
permalink: /media-queries/
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
  - media query
  - responsive
---
The reponsive design for websites has become the new standard for developing next generation websites, this feature is essential nowadays with all the new devices like Tablet, Smartphones (etc.), with CSS3 is possible to use "media queries", simple css variables that applies rules only in the specified width of the browser, it detects the measures and applies the rules only when the screen size matches.

Here is an example on how to create a media query variable in your css file.

    @media only screen
    and (min-device-width : 320px)
    and (max-device-width : 480px) {
    /* Styles */
    }

Just wrap your styles inside there and they will be applied only if the device width is corresponding to the indicated range.

Note that

    max-device-width

is different from

    max-width

With the first one it will only apply on the device and not if you resize your browser window, with the second one it will apply on both cases.

And here is a list of the common measures for the most used devices:

    // Landscape phones and down
    @media (max-width: 480px) { ... }
    // Landscape phone to portrait tablet
    @media (max-width: 767px) { ... }
    // Portrait tablet to landscape and desktop
    @media (min-width: 768px) and (max-width: 979px) { ... }
    // Large desktop
    @media (min-width: 1200px) { ... }

By putting your css code inside this media queries you will be able to customize the css to obatin a different design for every device and/or screen size and make your website react and change the layout of your contents depending on your needs. Pretty nice uh?

Have fun!