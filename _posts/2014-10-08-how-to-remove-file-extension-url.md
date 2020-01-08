---
id: 434
title: How to remove the file extension from the url
date: 2014-10-08T18:05:44+00:00
author: pwnjack
layout: post
guid: http://pwnjack.com/?p=434
permalink: /how-to-remove-file-extension-url/
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
  - htaccess
  - permalinks
  - url path
---
When developing websites i don&#8217;t like to show the file extension in the url like &#8220;about.html&#8221; or &#8220;contact.php&#8221;, I prefer to hide it and have a fancy permalink less technical and more SEO friendly like: &#8220;/about/&#8221; or &#8220;/contact/&#8221;.

Note: to achieve this you can setup the &#8220;.htaccess&#8221; file on your web server to do the work for you. To let it work properly you need to have the MOD_REWRITE module active on your web server.

Just add this lines to the `.htaccess`

<pre class="brush: plain; title: ; notranslate" title="">Options -MultiViews

 # enable the rewrite engine
 RewriteEngine On
 # Set your root directory
 RewriteBase /

 # remove the .html extension
 RewriteCond %{THE_REQUEST} ^GET\ (.*)\.html\ HTTP
 RewriteRule (.*)\.html$ $1 [R=301]

 # remove index and reference the directory
 RewriteRule (.*)/index$ $1/ [R=301]

 # remove trailing slash if not a directory
 RewriteCond %{REQUEST_FILENAME} !-d
 RewriteCond %{REQUEST_URI} /$
 RewriteRule (.*)/ $1 [R=301]

 # forward request to html file, **but don't redirect (bot friendly)**
 RewriteCond %{REQUEST_FILENAME}.html -f
 RewriteCond %{REQUEST_URI} !/$
 RewriteRule (.*) $1\.html [L]
</pre>

This removes the html extension, repeat the code above twice with .php instead to achieve the same effect on scripts.

Keep in mind that files starting with dots are hidden files, so to see them in your Finder, for instance, you have to tweak it a little, [this article](http://pwnjack.com/show-hidden-files-on-mac-osx/ "Show hidden files on Mac OSX") could help you.

Happy coding.