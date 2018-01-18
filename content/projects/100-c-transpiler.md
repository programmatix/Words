---
title: "C Parser"
date: 2018-01-15T09:50:29+07:00
layout: "c-transpiler.html"
---
[CParser on github](https://github.com/gropple/CParser) is my library that turns valid C code into a clean abstract syntax tree (AST), and can be embedded in any JVM-language project.

This could be useful for e.g. a JVM-based C compiler, transpiler, prettifier, or IDE plugin.

The code is written in Scala and transpiled to Javascript with ScalaJS so it can be embedded directly here:
