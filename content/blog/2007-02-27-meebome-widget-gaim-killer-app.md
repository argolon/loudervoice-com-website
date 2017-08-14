---
title: MeeboMe widget + Gaim = Killer App
author: "Conor O'Neill"
date: 2007-02-27T22:21:25+00:00
url: /blog/2007/02/27/meebome-widget-gaim-killer-app/
categories:
  - Blog

---
I&#8217;ve made good use of [Meebo][1] in the past working for silly places that block external IM but I&#8217;ve avoided putting the [MeeboMe][2] widget on our blogs for one simple reason; I&#8217;d have to have to be logged into Meebo in a browser window to get the messages rather than receiving them in my IM client where they belong.

Well it looks like I was totally wrong and you can configure [Gaim][3] or any other Jabber client to receive the messages from those who try to contact you on your blog via the MeeboMe widget. In Gaim you just add a new account where type=jabber, user=your\_meebo\_login, server=meebo.org and password=your_meebo password.

This is a fantastic resource for enabling people to contact you directly and quickly and they don&#8217;t need any IM software installed on their machines. The only small annoyance is that each new person who uses the widget needs to be authorised by you before you can start IM&#8217;ing. But that just means two extra clicks.

UPDATE 1: A teensy flaw in [the cunning plan][4]. You get an &#8220;authorize buddy&#8221; request every single time someone views the blog. Argghh. [But some nice person][5] has hacked the jabber.dll file in Gaim to handle those so you never see them. Seems to be working ok at the minute.

 [1]: http://www.meebo.com/
 [2]: http://www.meebome.com/?o
 [3]: http://gaim.sourceforge.net/
 [4]: http://forum.meebo.com/viewtopic.php?t=7605&postdays=0&postorder=asc&start=0
 [5]: http://www.tc.umn.edu/~beckvall/dan/MyFiles/MyFilesPage.html