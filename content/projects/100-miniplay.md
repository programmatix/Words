---
title: "MiniPlay"
date: 2018-01-21T09:50:29+07:00
layout: "project.html"
---
The web-based Google Play Music is great, but I was forever having to find the right browser tab just to change or like a song.  So I wrote this desktop widget.  It has two parts:

* Chrome extension: Written in Javascript, this is what interfaces with the Google Play Music tab.  [Source on Github](https://github.com/gropple/MiniPlayChrome).
* App: This widget runs on the user's desktop and is coded in Scala and uses ScalaFX for the UI, and Spring Boot to make a small Websockets server.  [Source on Github](https://github.com/gropple/MiniPlayDesktop).  

![MiniPlay](/Words/images/miniplay.jpg)
