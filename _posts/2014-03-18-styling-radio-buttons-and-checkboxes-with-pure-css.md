---
id: 199
title: Styling radio buttons and checkboxes with pure CSS
date: 2014-03-18T11:32:50+00:00
author: pwnjack
layout: post
guid: http://pwnjack.com/?p=199
permalink: /styling-radio-buttons-and-checkboxes-with-pure-css/
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
  - checkbox
  - css
  - forms
  - pseudo-class
  - radio button
  - web design
---
There's a lot of debate around the HTML Form's radio buttons and checkboxes stylization, they're usually hard to be styled cross-browser because of their limited capabilities in older browsers, even using jQuery.

Here I'll show you a good technique to style form's elements precisely the way you want, using only pure CSS.

First of all put down some HTML markup like this:

    <input type="checkbox" id="mybutton"></input>
    <label for="mybutton">Label</label>

Note that we need to associate a label to the button using the "for" attribute.

Then switch to your css file and proceed as follows:

    input {
      display: none;
    }

    label {
      display: block;
      background: red;
      width: 50px;
      height: 50px;
      text-indent: -9999px;
    }

Let's analyize what's happening here.

We simply made the real radio/checkbox button disappear with a _display: none;_  CSS property and started to style the label associated to it, you can use a background, color,  text, anything you would normally do with any other HTML element. Then use your CSS selector for the status checked with the :checked pseudo-class and target the associated label with the + sign, as shown here:

    input[type=checkbox]:checked + label {
      background: green;
    }


This way, when you click on the stylized label,  you'll obatin the same effect of clicking on the button, that is actually gone, so you don't have to worry about the complicated and headaching way of stylizing directly the button, with poor cross-browser consistency results.

Here's a working example to show you exaclty how it works:<a title="Checkbox Stylization working example" href=" http://jsfiddle.net/7rBKT" target="_blank"> http://jsfiddle.net/7rBKT</a>

Enjoy.