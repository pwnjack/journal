---
id: 521
title: 'Download images of a target website using wget's magic'
date: 2015-01-28T15:28:06+00:00
author: pwnjack
layout: post
guid: http://pwnjack.com/?p=521
permalink: /download-images-target-website-using-wget-magic/
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
  - tech
tags:
  - download
  - images
  - wget
---
Ever wanted to download all the images present on a web page? Here's how you can do it automatically instead of one-by-one.

    wget -nd -r -P . -A jpeg,jpg,png,gif http://www.examplewebsite.com

To do this you need wget installed, after that open your terminal, move inside a desired directory and launch the said command.

**-nd** Removes all the directory and puts all images in the same folder

**-r** Downloads all the images by following the page's paths recursively, to be sure to download every image

**-P** Choose the destination path of the download (in the example the . (dot) means inside this folder)

**-A** Choose the filetype to download, in this case we are downloading images such as jpg, png, gif, etc.