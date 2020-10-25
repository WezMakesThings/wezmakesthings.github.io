---
layout: post
title: Autonomous Tri-Copter
---

I've been flying some micro quads recently. FPV is a lot of fun but there's only so much that can be done with a hobby drone under 250 grams. I wanted to build a multi-rotor that could do more than manual flight, something that could carry a payload  or scan an area with a camera guided by gps. I chose a tri-copter because I wanted to work on something more mechanically involved than a quad-copter, and they get better battery with less motors.
![]({{ site.baseurl }}/images/tricopter/YCopter2.jpg)

While more complex than a quad rotor the tri rotor (Tri-copter? Ycopter? Yrotor? Why-copter?) is pretty simple mechanically. The two front motors are counter rotating and fixed to the frame while the rear motor is on a pivot driven by a symmetric four bar linkage. The front two motors cancel each others moment force though the tail motor has to be on a pivot so that it can angle its thrust to keep the whole drone from spinning.

![]({{ site.baseurl }}/images/tricopter/Tail.jpg)

The motor is mounted on two small bearings from my leftover 3d printer parts. The servo is mounted to the other side of the arm and connected with Lego tie bars. These we're really the best option since they are ridged injection molded ABS and mounted on ball pivots to that the servo horn doesn't have to be directly lined up with the motor bracket. I need to redesign the servo horn so that I can screw it to the motor, one crash has been caused by the horn falling off and I don't have many propellers to spare. All printed parts are PETG and After re-printing some in different orientations seems to hold up well.

![]({{ site.baseurl }}/images/tricopter/YCopter.jpg)

The flight controller is an ArduFlyer APM 2.6 purchased off Ebay. These can be found every so often for about $30 since they're no longer supported by later versions of Ardupilot. Documentation can also be scarce though I was able to get this drone to fly in stabilize mode and hold altitude and position with gps. Though currently I'm having issues with the compass direction being off so no auto missions yet. Will update when I can get that working.