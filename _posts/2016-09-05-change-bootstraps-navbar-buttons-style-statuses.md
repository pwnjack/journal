---
id: 698
title: How to change bootstrap's navbar buttons style, in all statuses
date: 2016-09-05T18:15:27+00:00
author: pwnjack
layout: post
guid: http://pwnjack.com/?p=698
permalink: /change-bootstraps-navbar-buttons-style-statuses/
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
  - bootstrap
  - css
  - navbar
  - selector
  - style
---
Getting mad finding out how to change the styles for every single status of Bootstrap's navbar buttons?

Sometimes is frustrating to waste time finding out all of them, in all behaviors (:active, :focus, .open, .dropdown, etc.).

So here's an all-in-one selector to change the style of all of them:

    .navbar-default .navbar-nav > .open > a,
    .navbar-default .navbar-nav > .open > a:hover,
    .navbar-default .navbar-nav > .dropdown a:focus,
    .navbar-default .navbar-nav > .open > a:focus {
      background: red;
      color: green;
    }

You're welcome 🙂