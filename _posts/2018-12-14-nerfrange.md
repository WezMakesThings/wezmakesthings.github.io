---
layout: post
title: Nerf target range PCB and lighting.
---

A local company, Corman and Associates in Lexington, hired me on to do the programming and electrical design for a Nerf shooting range project. The contract is with the U.S Marines. Shown here is the finished PCB that detects the impact of the dart on the target, plays a sound, and runs a neopixel light animation. 
![Ring test]({{ site.baseurl }}/images/nerf/ringtest.gif)

###PCB

![PCB]({{ site.baseurl }}/images/nerf/firstboard.jpg)
The PCB for this project is the conjunction of two prefabricated modules from Adafruit, and five copies of a simple circuit that takes the electrical signal from the piezo disks and converts it to logic level of the microcontroller. 

The microcontroller (black daughter board) is the Adafruit Metro Mini 328 based on the ATmega328 chip. Form factor large flash/ram and supplier we're considerations for the choice. Retrospectively I should have went with a lower power microcontroller. Something that used less power while running. It only became aware to us later in the project that the cabinets would be mobile and need to run off of batteries. 

The other module pictured (blue daughter board) is the Adafruit Audio FX Sound Board. We used the version without the amplifiers included. This allowed us to use amplifiers that we're already on hand. This module is super easy to use. It can either directly connect to inputs on each of its pins for triggering audio or be controlled over serial. 

###Piezo impact signal

![piezo circuit]({{ site.baseurl }}/images/nerf/circuit-whole.png)
Image from [this site](https://defproc.co.uk/blog/sense-foam-dart/) which I came across while researching the methods of sensing impacts cheaply. I highly recommend this as a resource to anyone trying something similar. There is a full explanation of the theory and operation of this circuit on his site. This circuit is made up of three parts. A rectifier, made up of D1 and D2. The voltage is clamped by D3, and the signal is smoothed by R1 and C1.

###Mounted in an early version of the cabinet

![cabinet]({{ site.baseurl }}/images/nerf/targettest.gif)