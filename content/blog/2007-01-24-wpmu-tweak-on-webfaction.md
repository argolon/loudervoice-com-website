---
title: WPMU tweak on WebFaction
author: "Conor O'Neill"
type: post
date: 2007-01-24T15:21:49+00:00
url: /2007/01/24/wpmu-tweak-on-webfaction/
categories:
  - Blog

---
If you run any version of [WordPress][1] on a [WeFaction][2] hosted account you&#8217;ll run into the problem of sendmail being disabled so none of the notification mails get sent out. The way around this is to install the [wpPHPMailer][3] plug-in which uses SMTP instead. To get around the catch-22 of needing it installed to get your WP password, you&#8217;ll have to do the WP install, then go into phpMyAdmin and change your password using the MD5 function in the wp_users table and then login and enable the plugin and set the mail server options.

We had thought the same approach would work on WPMU but it appears it only works for the main admin blog at the &#8220;root&#8221; of the install. The problem is that wpPHPMailer is not picking up the extra username in the blog URL and it is impossible to save the options on the options page. The solution seems to be to change line 215 to `$action_url = $_SERVER[REQUEST_URI];`

Next to figure out the easiest way of setting tons of different WPMU options so they are the defaults for each new blog&#8230;&#8230;

 [1]: http://www.wordpress.org/
 [2]: http://www.webfaction.com/
 [3]: http://www.coffee2code.com/archives/2004/06/28/plugin-wpphpmailer/