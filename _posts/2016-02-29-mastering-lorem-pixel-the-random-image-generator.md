---
id: 645
title: Mastering Lorem Pixel, the random image generator
date: 2016-02-29T18:45:52+00:00
author: pwnjack
layout: post
guid: http://pwnjack.com/?p=645
permalink: /mastering-lorem-pixel-the-random-image-generator/
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
  - image generator
  - img
  - placeholder
  - random images
---
Need a random image generator? <a href="http://lorempixel.com" target="_blank">LoremPixel</a> is the perfect tool.

Populate your images by just adding this link to the src attribute of your<img /> tags, like so:

<img src="http://lorempixel.com/250/250">

The numbers are the width and height of the image you want to display.

The problem comes when you have multiple images on the same page and, for instance, you want to create a grid of images all different from each other, here's a solution:

<img src="http://lorempixel.com/250/250/abstract/1">

You can choose a category (abstract, sport, etc, check the lorempixel website for more options) and a number, change the last number to always load a given image, so you can change it on every image tag and have all images different from each other.

Enjoy your favorite image placeholder.