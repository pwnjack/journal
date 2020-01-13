---
id: 512
title: Entering the Jade forest
date: 2015-01-20T23:00:02+00:00
author: pwnjack
layout: post
guid: http://pwnjack.com/?p=512
permalink: /entering-jade-forest/
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
  - tool
  - web design
tags:
  - html
  - jade
  - preprocessor
  - template
---
Why don't you enter the Jade forest with me, dare you?

Jade is a clean, short, awesome markup language, once you master it you will be able to build html pages in a matter of seconds, and best of all it's easy-to-read, scalable and clean as never before.

Jade is used a lot in dynamic web application but as a frontend developer I use it as a pre-processor for my html markup, and why not use it in conjunction with my frontend workflow script, [Prime](http://pwnjack.com/prime-scaffolding-frontend-projects-breeze/ "Prime, scaffolding frontend projects is a breeze")?

Let's do it.

Voilà here is <a href="https://github.com/pwnjack/jader" title="Jader" target="_blank">Jader</a>, the evolution of the previously mentioned Prime.

Let's see how Jade works, it's based a lot on indentation and code positioning so be careful with that.

For instance, you can write down this:

    doctype html
html(lang="en")
  head
    title= pageTitle
    script(type='text/javascript').
      if (foo) {
         bar(1 + 5)
      }
  body
    h1 Jade - node template engine
    #container.col
      if youAreUsingJade
        p You are amazing
      else
        p Get on it!
      p.
        Jade is a terse and simple
        templating language with a
        strong focus on performance
        and powerful features.



Will render as:



<html lang="en">
  <head>
    <title>Jade</title>
    <script type="text/javascript">
      if (foo) {
         bar(1 + 5)
      }
    </script>
  </head>
  <body>
    <h1>Jade - node template engine</h1>
    <div id="container" class="col">
      <p>You are amazing</p>
      <p>
        Jade is a terse and simple
        templating language with a
        strong focus on performance
        and powerful features.
      </p>
    </div>
  </body>
</html>



Go ahead and test your code on the <a href="http://jade-lang.com/" title="Jade" target="_blank">Jade official website</a>.

It features also a lot of common features like variables, if statements, mixins, includes and a lot more, imagine how easy will be to build even static html pages, just try it out with Jader, it's awesome how fast you can build an UI, give it a try!

Happy coding.