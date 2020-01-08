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
Why don&#8217;t you enter the Jade forest with me, dare you?

Jade is a clean, short, awesome markup language, once you master it you will be able to build html pages in a matter of seconds, and best of all it&#8217;s easy-to-read, scalable and clean as never before.

Jade is used a lot in dynamic web application but as a frontend developer I use it as a pre-processor for my html markup, and why not use it in conjunction with my frontend workflow script, [Prime](http://pwnjack.com/prime-scaffolding-frontend-projects-breeze/ "Prime, scaffolding frontend projects is a breeze")?

Let&#8217;s do it.

Voilà here is <a href="https://github.com/pwnjack/jader" title="Jader" target="_blank">Jader</a>, the evolution of the previously mentioned Prime.

Let&#8217;s see how Jade works, it&#8217;s based a lot on indentation and code positioning so be careful with that.

For instance, you can write down this:

<pre class="brush: plain; title: ; notranslate" title="">doctype html
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
</pre>

Will render as:

<pre class="brush: xml; title: ; notranslate" title="">&lt;!DOCTYPE html&gt;
&lt;html lang="en"&gt;
  &lt;head&gt;
    &lt;title&gt;Jade&lt;/title&gt;
    &lt;script type="text/javascript"&gt;
      if (foo) {
         bar(1 + 5)
      }
    &lt;/script&gt;
  &lt;/head&gt;
  &lt;body&gt;
    &lt;h1&gt;Jade - node template engine&lt;/h1&gt;
    &lt;div id="container" class="col"&gt;
      &lt;p&gt;You are amazing&lt;/p&gt;
      &lt;p&gt;
        Jade is a terse and simple
        templating language with a
        strong focus on performance
        and powerful features.
      &lt;/p&gt;
    &lt;/div&gt;
  &lt;/body&gt;
&lt;/html&gt;
</pre>

Go ahead and test your code on the <a href="http://jade-lang.com/" title="Jade" target="_blank">Jade official website</a>.

It features also a lot of common features like variables, if statements, mixins, includes and a lot more, imagine how easy will be to build even static html pages, just try it out with Jader, it&#8217;s awesome how fast you can build an UI, give it a try!

Happy coding.