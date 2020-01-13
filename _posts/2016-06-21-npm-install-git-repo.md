---
id: 685
title: How to npm install from a git repo
date: 2016-06-21T16:25:07+00:00
author: pwnjack
layout: post
guid: http://pwnjack.com/?p=685
permalink: /npm-install-git-repo/
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
  - git
  - npm install
  - revision
---
Sometimes you'll need to install an npm package from a git repo, often more updated than the actual package's npm registry official release version.

To install a git repo via npm use the following syntax:

    ## Public repos
    npm install git+https://github.com/<repo-owner>/<repo>.git[#branch]
    npm install git+ssh://git@github.com/<repo-owner>/<repo>.git[#branch]
    npm install git://github.com/<repo-owner>/<repo>.git[#branch]

    ## Private repos
    npm install git+ssh://git@github.com/<repo-owner>/<repo>.git[#branch]

Working example given:

    npm install git+https://github.com/taptapship/wiredep.git

This is useful when in need to try beta versions or many other cases, hope this helps!