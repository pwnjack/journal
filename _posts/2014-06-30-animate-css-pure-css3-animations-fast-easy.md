---
id: 341
title: Animate CSS, pure CSS3 animations fast and easy
date: 2014-06-30T14:23:20+00:00
author: pwnjack
layout: post
guid: http://pwnjack.com/?p=341
permalink: /animate-css-pure-css3-animations-fast-easy/
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
  - news
tags:
  - animateCSS
  - animation
  - css3
  - transition
---
CSS3 introduced animations, a nice and easy way to give a smooth feel to your content without using any javascript, these animation are widely supported by almost all browsers. except of course that crappy old IE7.

Anyway IE users don't deserve to view nice animations.

This CSS library (download it <a title="AnimateCSS" href="http://daneden.github.io/animate.css/" target="_blank">here</a>) is straight to go, there's a bunch of animation types just choose the one that you like more and use it right out of the box, here how:

Link it in the head of your page:

      <link rel="stylesheet" href="animate.min.css">
    </head>

Then simply:

    $('#yourElement').addClass('animated bounceOutLeft');

You can change the duration of your animations, add a delay or change the number of times that it plays:

    #yourElement {
      -vendor-animation-duration: 3s;
      -vendor-animation-delay: 2s;
      -vendor-animation-iteration-count: infinite;
    }

Go on to the <a href="https://github.com/daneden/animate.css" title="AnimateCSS on Github" target="_blank">github page</a> to see detailed documentation.

Happy coding.