---
weight: 100
title: "Web"
date: 2018-01-15T09:50:29+07:00
layout: "project.html"
---
## Undiscovered Guide
[Undiscovered Guide](https://www.undiscoveredguide.com) is a travel website I created with my partner while we were travelling, to help others explore our favourite parts of the world.  It's pretty popular, getting over 30,000 monthly page views.
![Undiscovered Guide](/Words/images/ug.JPG)
It's a completely custom web platform (no Wordpress or similar) which allowed us to create more useful travel guides than traditional blogs, and there's a lot going on under the hood:

* The frontend is written in Scala, transpiled to Javascript with ScalaJS.  This convoluted approach let me do a lot of cool code sharing with the backend.
* Parts of it are a dynamically-created single page app.  There's all sorts of cool widgets such as interactive maps dotted over the site.
* There's a fairly complex backend content management system (CMS), written in Scala and with its own UI transpiled in ScalaJS, using PostgreSQL for data storage.  It has too many features to list: a full Google rank tracker, a Wikitravel parser, bots for both Pinterest and Twitter, batch processing of images, a booking.com & Agoda accommodation browser (view all their hotels for a location on a map, filter by various criteria and add them to lists), and plenty more.
* The CMS includes a custom HTML-like language, with its own handwritten parser.  This let us convert all prices into the user's currency, amongst other features.
* It's all self-hosted so I'm now all too familiar with the joys of maintaining memory-hungry JVM processes on constrained server hardware... 

## Travelpouch
My partner and I needed a way to track our daily travel expenses, along with tracking who owed who what across a variety of currencies.  So Travelpouch was born, a web-based finance tracking app that is great for personal tracking and budgeting, and has some great features for couples and friends that holiday together and need to split expenses fairly.

The backend and frontend are both in Scala, with the frontend transpiled to Javascript with ScalaJS.  There's also an Android app, written in Scala.  

This was my first web project and went through several tech iterations while I explored different web tech stacks, including Grails (which is Groovy+Spring), then Angular, then its current version.  I'm pretty happy with the current Scala+ScalaJS stack, which I've used now on multiple projects and allows very productive code sharing, but I have my eye on Kotlin+KotlinJS as a successor.

We use Travelpouch daily, but it's a bit rough around the edges so is presently closed source and not generally available.
![Travelpouch](/Words/images/travelpouch.jpg)

## Smaller projects
* [One More Go](http://www.onemorego.net/) is a blog devoted to reviewing casual games, which I was briefly utterly addicted to.  It's on the Wordpress platform hosted on one of my servers.
* This site is coded with the static site generator Hugo.  Static site generators are awesome: they're much faster and simpler than something like Wordpress, both for adding and consuming content.  The source is [on Github](https://github.com/programmatix/Words) and it's hosted on Git Pages. 
