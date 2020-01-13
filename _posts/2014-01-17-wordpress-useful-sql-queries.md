---
id: 72
title: WordPress useful SQL queries
date: 2014-01-17T11:05:10+00:00
author: pwnjack
layout: post
guid: http://pwnjack.com/?p=72
permalink: /wordpress-useful-sql-queries/
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
  - database
  - MySQL
  - phpmyadmin
  - query
  - wordpress
---
When moving a WordPress site you need to slightly modify the database to make it work properly with the new domain and hosting. You can use this commands to reset password, change website url, and to be sure every link is still working (like image links etc.) and much more, so instead of opening every single post and page and find out where you need to do this fixes, you can simply use some of this useful SQL queries to send the database ninja monkeys to do the work for you, all at once.

To do this you need to open your _phpmyadmin_ for managing the MySQL database, then open the SQL tab and there you can paste this lines of code.

Be sure to change the code with your correct data.  
Set new website URL:

    UPDATE wp_options SET option_value = 'http://www.yourdomain.com' WHERE option_name IN ('siteurl', 'home')

Replace URL in content:

    UPDATE wp_posts SET post_content=(REPLACE (post_content, '{old url}','{new url}'))

Change GUID:

    UPDATE wp_posts SET guid = REPLACE (guid, 'http://www.oldsiteurl.com', 'http://www.newsiteurl.com');

Change URL in Content:

    UPDATE wp_posts SET post_content = REPLACE (post_content, 'http://www.oldsiteurl.com', 'http://www.newsiteurl.com');

Change IMG URL in Content:

    UPDATE wp_posts SET post_content = REPLACE (post_content, 'src="http://www.oldsiteurl.com', 'src="http://yourcdn.newsiteurl.com');

Reset User password:

    UPDATE wp_users SET user_pass = MD5( 'new_password' ) WHERE user_login = 'your-username';

Enjoy!