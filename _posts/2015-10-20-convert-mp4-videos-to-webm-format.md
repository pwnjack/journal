---
id: 573
title: Convert mp4 videos to webm format
date: 2015-10-20T12:42:20+00:00
author: pwnjack
layout: post
guid: http://pwnjack.com/?p=573
permalink: /convert-mp4-videos-to-webm-format/
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
  - batch
  - convert
  - converter
  - ffmpeg
  - mp4
  - mp4 to web
  - video
  - webm
---
The easiest way to convert mp4 video to webm, the format needed to properly embed an HTML5 video, is the following:

Install ffmpeg for CLI via brew (OSX):

    brew install ffmpeg --with-libvpx --with-libvorbis --with-fdk-aacc

Then use the following command to do the conversion:

    ffmpeg -i input-file.mp4 -c:v libvpx -crf 10 -b:v 1M -c:a libvorbis output-file.webm

The command format is as follows:

    ffmpeg [global options] [input file options] -i input-file-name [output options] output-file-name

To convert multiple videos at once create an .sh file, set its permission to 755 and paste the following code in it, then run it.

    #!/bin/bash
    VIDEOS=~/Desktop/video-folder/
    find "$VIDEOS" -name '*.mp4' -exec sh -c 'ffmpeg -i "$0" -c:v libvpx -crf 10 -b:v 1M -c:a libvorbis "${0%%.mp4}.webm"' {} \;
    exit;

Enjoy