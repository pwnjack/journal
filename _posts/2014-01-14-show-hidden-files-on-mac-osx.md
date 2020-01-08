---
id: 89
title: Show hidden files on Mac OSX
date: 2014-01-14T11:15:35+00:00
author: pwnjack
layout: post
guid: http://pwnjack.com/?p=89
permalink: /show-hidden-files-on-mac-osx/
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
  - hidden files
  - mac
  - osx
  - terminal
---
Sometimes is useful to show hidden files on Mac, altough there is no option for doing that, for security reasons.

If you need to show the hidden files, the files starting whit a dot (.), like .htaccess and such, you can open the Terminal and paste this code strings in it.

The first one is to show hidden files, the second one to hide them again.

For OSX 10.9:

<pre class="brush: powershell; title: ; notranslate" title="">defaults write com.apple.finder AppleShowAllFiles TRUE

defaults write com.apple.finder AppleShowAllFiles FALSE
</pre>

For OSX 10.8 and earlier:

<pre class="brush: powershell; title: ; notranslate" title="">defaults write com.apple.Finder AppleShowAllFiles TRUE

defaults write com.apple.Finder AppleShowAllFiles FALSE
</pre>

After that, you need to reset the Finder with this command:

<pre class="brush: powershell; title: ; notranslate" title="">killall Finder
</pre>