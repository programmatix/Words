---
title: "Desktop"
date: 2018-01-21T09:50:29+07:00
layout: "project.html"
---
## MiniPlay
The web-based Google Play Music is great, but I was forever having to find the right browser tab just to change or like a song.  So I wrote this desktop widget to be able to control my music easily without needing to go to the browser.  It has two parts:

* Chrome extension: Written in Javascript, this is what interfaces with the Google Play Music tab.  [Source on Github](https://github.com/programmatix/MiniPlayChrome).
* App: This widget runs on the user's desktop and is coded in Scala and uses ScalaFX for the UI, and embeds a mini Spring Boot server to handle the Websockets connection from the extension.  [Source on Github](https://github.com/programmatix/MiniPlayDesktop).

![MiniPlay](/Words/images/miniplay.jpg)
