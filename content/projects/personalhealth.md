---
weight: 99
title: "Personal Health Dashboard"
date: 2024-07-29T17:20:00+01:00
layout: "project.html"
---
At the time of writing (2024), this is my main personal project.

I'm trying to track all the data related to personal health - particularly sleep and energy - as possible, and try to find patterns and correlations between them.
I'd like to optimise my energy levels as much as possible, and am solving that in the most Me way possible - by throwing inordinate amounts of time and software engineering at the problem :)

It's also been a good excuse to learn more about AI, ML data science.

The most recent development is I'm now capturing EEG (brainwave) data using an OpenBCI Cyton board:

![EEG Data](/Words/images/xl/eeg1.png)

and using it to train a model with Tensorflow that will estimate my energy levels.  
This has turned into a significant side-project as I build out software and visualisation for testing different model approaches - linear regression, neural nets, XGBoost, etc.

I'm using the same EEG data to plot a sleep hypnogram each night (the excellent YASA project is doing a lot of the heavy lifting):

![Hypnogram](/Words/images/xl/yasa.png)

Related projects:
* [Brainwave](https://github.com/programmatix/Brainwave-Python) - captures EEG data, performs FFT and other transforms, and sends the data on to files, visualisers and databases.
* [Brainwave-Processor](https://github.com/programmatix/Brainwave-Python) - processes the EEG data for sleep hypnogram.

I'm also capturing nearly 24x7 heart rate data, from which I calculated HRV using the RMSSD method, core body temperature, oxygen levels, exercise data, sleeping positions, and respiratory data.
This is all captured from several devices (a Polar H10, a CORE thermometer, a Viatom O2 device, a Google Pixel Watch, and an Oxa sensor) over Bluetooth Low Energy into an Android application I've written in Kotlin, and stored in Influx (a timeseries database).

![Metrics](/Words/images/xl/metrics.png)

I also capture a lot of data about my environment, including CO2, light, noise and temperature levels at night, and my presence in the house.  This is all fed into Home Assistant and ultimately Influx.

I have a WIP project (not yet tidied up to share publically) that's trying to estimate fatigue based on analysis webcam images, using the Google Mediapipe model to track where my eyes are, and training a neural net model to detect whether I'm blinking, based on labelling hundreds of such eye images as open or closed.  (There is research to suggest that blinking increases with tiredness)

I take pictures of what I eat and give them to ChatGPT to estimate nutritional content - an approach that works surprisingly well.

I'm then using all this captured data in various ways, including finding useful correlations between metrics, with the hope of finding how to optimise e.g. time asleep and energy levels next day.

![Correlations](/Words/images/xl/correlations.png)

Technologies used:
* Frontend: React, Firebase, Typescript
* Databases: Influx, Firebase
* Mobile app: Android, Kotlin