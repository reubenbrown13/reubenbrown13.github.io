---
layout: post
title: "Octopress Install Notes"
date: 2015-04-14 09:05:19 -0500
comments: true
categories: [Octopress, Tech, Internet, Blogging]
---
<p>While searching for help on a project I am working on, I noticed one of my <a href="http://seancorfield.github.io/" target="_new">peers</a> had changed their blogging platform over to <a href="http://octopress.org/" target="_new">Octopress</a>.  I have used several systems in the past but always desired to have a certain level of control.  I loathed the idea of using WordPress and having a blog hosted on their servers.  The idea of using something so nerd-centric really appealed to me.  The install and setup guide looked like a very simple thing to follow.  This proved to be mostly true....</p>
<!-- more -->
<p>When following the <a href="http://octopress.org/docs/setup/" target="_new">Setup Guide</a>, there are several steps that must be done in the proper order.  The guide is well laid out and easy to read.  On my Ubuntu powered workstation I installed what I thought were all the required packages.  I discovered after the fact that to get Octopress to work on Ubuntu, you must install Node.JS as your javascript engine or else it doesn't work.  I tried to use 'therubyracer' first but it didn't allow me to generate the pages.</p>
<p>The second snag I hit was trying to get the order right for using <a href="http://octopress.org/docs/deploying/github/" target="_new">Github Pages</a>.   Where this got confusing to me was that the Octopress guide is clear, but when you setup the github pages repo, Github tells you to clone it.  You do not want to do this.  You want to stay in the Octopress folder you setup and follow the guide to setup the pages and generate the site.  If it fails to work you can always delete the site and recreate it since you have not saved anything there yet.</p>
<p>The last thing I would recommend is to update the _config.yml file right away before you generate the pages for the first time.  Get things setup nice and clean for yourself.  You might even want to preview the content prior to doing the the first "rake deploy" by using "rake preview" and opening your browser to localhost:4000.</p>
<p>These notes are of great benefit to me, and if they help anyone else awesome.</p>
