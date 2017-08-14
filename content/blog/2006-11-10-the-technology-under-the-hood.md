---
title: The technology under the hood
author: "Conor O'Neill"
date: 2006-11-10T10:44:16+00:00
url: /blog/2006/11/10/the-technology-under-the-hood/
categories:
  - Blog

---
When we first kicked off this new venture, I made a few simple decisions on technology. The first was that we were going to take an agile approach with everything and particularly using agile languages and web frameworks. Over the past ten years I&#8217;ve had major success with projects which used Tcl, Perl and Python where the accepted wisdom would often have been to build some monster C++ or Java app. Most of those projects were not web related but some of the more recent ones were and the productivity of the developers was often gob-smacking.

Given that, I did not want to direct \_which\_ approach to use with outsourcers, I was happy for them to suggest solutions to me. As expected, it boiled down to three main approaches: PHP, Python and Ruby. Obviously Ruby was with Rails but PHP was suggested both with and without a framework and the frameworks were all homegrown (as opposed to CodeIgniter or Symfony). In the Python world I was surprised to find no-one in Europe using Django despite its high profile and saw zero mention of Pylons. However, I got a bunch of companies working in [TurboGears][1] which encouraged me as I did have a bias towards using Python+TG.

TG takes the Rails view of the world and provides a huge amount of the infrastructure you need to build a web application. It is quite new, only appearing last year, but the energy behind it has been incredible. I instantly felt comfortable with both the approach and the community despite not being a hardcore developer myself any longer. The company we have hired to do our development has write access to the TG subversion repository which provides a strong degree of comfort in their ability to deliver and so far they have exceeded expectations.

Whilst the number of web-sites built using TG is still quite small, all of the ones that are out there are impressive and convince me that we have made the right technology choice. Once the full prototype is ready at the end of the month, we&#8217;ll have a great opportunity to beat the hell out of it and see how both the app and TG perform. The prototype is not being built to be immediately scalable but we should be able to evaluate some core metrics.

There are a few drawbacks to using something like TG. The first is that it is a moving target with 1.0 not available yet. A side effect of this is that the docs tend to always be slightly behind making the learning process harder. And finally, the base of developers in TG is still small so if we want to bring our own devs on board later next year, there is going to be a longer learning curve than if we had just used Rails or pure PHP.

I&#8217;d be interested to hear others experiences of using frameworks like TG and Rails for scalable public sites. Positives and negatives? Areas to be careful? Approaches to scaling using MySQL etc. I&#8217;ll continue to post our experiences with TG here. Actually, I&#8217;m also interested to hear of people going down the MS route. Are there any benefits for a startup to use .NET on Windows 2003? The numbers just don&#8217;t stack up for me and surely that is a major challenge for MS? If every startup out there is using some variation of LAMP on a cheap hosting platform, how does MS get a look-in where everything from the dev tools to the DB to the OS costs money? Maybe the solution is for them to build a Windows based EC2 clone with clustered SQL Server 2005 and free Dev tools at a knock-down $/GB and $/MIPS rate?

 [1]: http://www.turbogears.org/