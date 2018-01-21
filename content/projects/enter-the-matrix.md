---
title: "Enter the Matrix"
date: 2018-01-21T09:50:29+07:00
layout: "project.html"
---
A simple immutable library for vector and matrix maths, written in Scala.  There's a surprising lack of these, with the existing Scala matrix libraries being heavyweight, rather complex, and generally part of a much large statistical package.  I wanted something lightweight for 3D maths.  

It's designed to be very safe, concise, and easy to use:

```
    val m1 = Matrix4x4.identity
    val m2 = Matrix4x4.scale(1.0f)
    val m3 = Matrix4x4.rotateAroundXAxis(30.0f)
    val m4: Matrix4x4 = m3 * m2 * m1
    
    val v1 = Vector4(0.2f, 0.3f, 0.4f, 1.0f)
    val v2: Vector4 = m4 * v1
```

The [source is on Github](https://github.com/gropple/EnterTheMatrix).