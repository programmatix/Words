---
title: "Languages"
date: 2018-01-15T09:50:29+07:00
layout: "project.html"
---
# JVM
I've written several projects to do with the low-level JVM internals, which has been a great learning experience:

* [JOak JVM](https://github.com/programmatix/JOakJVM): a basic, but functioning, JVM written in Scala.
* [JOak Analyser](https://github.com/programmatix/JOakAnalyser): a command-line tool for debugging & analysing JVM .class files.
* [JOak ClassFiles](https://github.com/programmatix/JOakClassFiles): a JVM micro-library for reading JVM .class files.

# C Language
C is a great language for learning, as it's relatively simple.

* [CParser](https://github.com/programmatix/CParser): turns valid C code into a nice clean abstract syntax tree (AST) to be used in your JVM project.  Written in Scala.
* [CParserWebDemo](https://github.com/programmatix/CParserWebDemo): turns CParser into a Javascript widget (it's in Scala, but transpiles to JS with ScalaJS) that you can embed in a website.

Though these aren't very useful on their own (I wrote them mostly as a learning exercise for exploring parsing libraries on Scala, and to start learning compiler theory), they're a good starting point for e.g. a JVM-based C compiler, transpiler, prettifier, or IDE plugin.
