---
title: "Games"
date: 2018-01-15T09:50:29+07:00
layout: "nonograms.html"
---
## Nonograms
Nonograms!  I'm absurdly addicted to these.  

It's written in Scala, compiled to JS with ScalaJS so it can be embedded here.  The engine is almost completely pure/immutable, and all components are nicely separated with no strong binding between UI and game logic.  It includes an AI capable of solving most Nonograms.

<b>How to play:</b> Left-click to mark a block, right-click to delete empty ones (and you can click-drag ranges too).  Clues are at the edges of the board.  Clues of "3 2" mean there's a set of 3 contiguous blocks somewhere on that row or column, followed by a set of 2, with at least one empty space inbetween. 