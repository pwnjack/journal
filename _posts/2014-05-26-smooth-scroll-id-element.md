---
id: 319
title: Smooth scroll to ID element
date: 2014-05-26T18:22:03+00:00
author: pwnjack
layout: post
guid: http://pwnjack.com/?p=319
permalink: /smooth-scroll-id-element/
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
  - jquery
  - scroll
  - scrollto
  - smooth scroll
---
Have you ever wondered how does a one-page website work?  
It simply scrolls smoothly to a defined element on the page, instead of switching to another page.

Here is an example that explains how to scroll to an HTML element using a simple jQuery script.

This is the jQuery code:

    // Smooth scroll to section by targeting it's "name" attribute
    $( window ).load(function() {
        $('a.scrollto[href*=#]').click(function() {
            if (location.pathname.replace(/^\//,'') == this.pathname.replace(/^\//,'')
            && location.hostname == this.hostname) {
            var $target = $(this.hash);
            $target = $target.length && $target || $('[name=' + this.hash.slice(1) +']');
            if ($target.length) {
            var targetOffset = $target.offset().top;
            $('html,body').animate({scrollTop: targetOffset -82}, 1000);
            return false;}
            }
        });
    });

The script scrolls the page to the targeted "name" attribute, defined by the "id" attribute on the clicked element, here's an example:

Clicking on:






Will scroll the page to:

</section>

Give a name attribute to every section of your website and When you click on the "link" the page will scroll to the section with the corresponding _name="section-1"_ attribute.

With this technique building your one-page website with a neat navigation menu that scrolls smoothly, is a breeze. Usually these kind of navigation menus are intended to have a "fixed" position, to follow you up while the page scrolls, either way it will stay on the top of the page and become useless after the first scroll, keep that in mind when you design your website.