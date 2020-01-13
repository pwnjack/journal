---
id: 652
title: Replace all SVG images with inline SVG
date: 2016-04-01T19:56:09+00:00
author: pwnjack
layout: post
guid: http://pwnjack.com/?p=652
permalink: /replace-svg-images-inline-svg/
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
  - inline svg
  - replace
  - svg
  - vector graphic
---
SVG is the new era, nowadays with all these super-pixel-dense devices our poor jpg and png images are getting stretched, scaled, distorted all over and they render badly causing some bad-looking effects. This is why they are all being replaced with more modern, flexible SVGs.

The good thing about SVG is that they can be modified via CSS, so we can manipulate their aspect with code, this means we can dynamically change color, size, position and whatever we want, this is freaking awesome, isn't it?

But wait, stop the hype, because SVG are not that straight forward like linking an image:

    <img src="images/MyNiceImage.svg">

They are more like:

    <svg width="100" height="100">
      <circle cx="50" cy="50" r="40" stroke="green" stroke-width="4" fill="yellow" />
    </svg>

And they can get very complicated when the image is not a simple circle.

You can use it in an image tag but you can't manipulate nothing like that, this is just a simple image put in place without any possibility of image manipulation.

But with the following script it will be magically transformed in a properly structured inline SVG object, that on the contrary can be manipulated, and it's very flexible.

    /* Replace all SVG images with inline SVG */
    jQuery('img.svg').each(function(){
        var $img = jQuery(this);
        var imgID = $img.attr('id');
        var imgClass = $img.attr('class');
        var imgURL = $img.attr('src');

        jQuery.get(imgURL, function(data) {
            /* Get the SVG tag, ignore the rest */
            var $svg = jQuery(data).find('svg');

            /* Add replaced image's ID to the new SVG */
            if(typeof imgID !== 'undefined') {
                $svg = $svg.attr('id', imgID);
            }

            /* Add replaced image's classes to the new SVG */
            if(typeof imgClass !== 'undefined') {
                $svg = $svg.attr('class', imgClass+' replaced-svg');
            }

            /* Remove any invalid XML tags as per http://validator.w3.org */
            $svg = $svg.removeAttr('xmlns:a');

            /* Replace image with new SVG */
            $img.replaceWith($svg);

        }, 'xml');

    });

Now, while we have just put a simple image tag, we actually have an inline SVG object available in the DOM. And so we can easily change it's properties with code, the "svg" class is assigned to the element for easy targeting, example given:

    .svg {
        background: black;
    }
    .svg path {
        fill: white;
    }
    .svg:hover {
        fill: red;
    }

Look at what I did there, we can easily change it's color and background via CSS, imagine the possibilities.

If you want a more detailed and better written article about using SVGs, go <a href="https://css-tricks.com/using-svg/" target="_blank">ahead</a>.