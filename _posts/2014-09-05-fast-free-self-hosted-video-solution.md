---
id: 388
title: Fast and free self-hosted video solution
date: 2014-09-05T14:28:19+00:00
author: pwnjack
layout: post
guid: http://pwnjack.com/?p=388
permalink: /fast-free-self-hosted-video-solution/
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
  - web design
tags:
  - self hosted
  - self hosted video
  - video host
---
I was looking for a free and easy-to-setup way to have a self-hosted video on a website. although it might seem easy to find a plugin to do so, it's not so easdy to find a watermark-free solution out there.

If you need exactly this kind of thing, let me suggest you <a href="http://www.videojs.com" title="VideoJS" target="_blank">VideoJS</a>.

It's free, super easy to setup and HTML5 based, with a nice old-browser flash fallback solution. For more details visit their website.

To get started quick:

Embed the script via CDN just before your closing body tag

    <script src="//vjs.zencdn.net/4.8/video.js"></script>

Then paste this html5 video tag snippet and change the paths to point to your video files.

    <video id="example_video_1" class="video-js vjs-default-skin vjs-big-play-centered"
      controls preload="auto" width="640" height="264"
      poster="http://video-js.zencoder.com/oceans-clip.png"
      data-setup='{"example_option":true}'>
    <source src="http://video-js.zencoder.com/oceans-clip.mp4" type='video/mp4' />
    <source src="http://video-js.zencoder.com/oceans-clip.webm" type='video/webm' />
    <source src="http://video-js.zencoder.com/oceans-clip.ogv" type='video/ogg' />
    <p class="vjs-no-js">To view this video please enable JavaScript, and consider upgrading to a web browser that <a href="http://videojs.com/html5-video-support/" target="_blank">supports HTML5 video</a></p>
    </video>

Notice that you need at least 2 video formats .mp4 and .webm, fastest way to convert your video to webm is to upload it to youtube and then download it using something like <a href="http://jdownloader.org/" title="jDownloader" target="_blank">jDownloader</a> and voilà.

Enojy the fastest self-hosted video solution ever.