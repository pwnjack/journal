---
id: 601
title: How to sniff authentication cookies over Wi-Fi
date: 2015-12-15T18:20:21+00:00
author: pwnjack
layout: post
guid: http://pwnjack.com/?p=601
permalink: /how-to-sniff-authentication-cookies-over-wi-fi/
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
  - authentication
  - cookies
  - sniff
  - spy
---
In the pre https era you can easily intercept authentication cookies over the network you are connected to, it being Wi-Fi or Ethernet, as long as the target is in your same subnet you can do it with ease, here's how:

Install <a href="http://filehippo.com/it/download_firefox/8604" target="_blank">Firefox 3.2.16</a>

Install <a href="https://codebutler.github.io/firesheep" target="_blank">Firesheep</a> as a Firefox Add-on

Show the Firesheep toolbar from the "View" menu

Click on the "Start Capturing" button, and you will start to see all authenticated users on the network, on many different websites, then click on one of the results and you will be able to browse the website from your computer with the target account, without the need of password input, already logged in, because what Firesheep does is stealing the cookies that contain the authentication, and pretend to be the authenticated user, but on your computer. Give it a try in your private network.

Happy sniffing, folks.