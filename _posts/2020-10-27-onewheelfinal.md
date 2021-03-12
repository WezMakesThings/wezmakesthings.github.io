---
layout: post
title: DIY Onewheel Post Mortem
---

#### Summer 2020 Project 
![IT WORKS]({{ site.baseurl }}/images/owheelfinal/ridingit.jpg)
In the summer of 2020 I finished my Onewheel out of old parts. I had to complete it only using hand power tools which allowed me to learn a lot about how to do things the wrong way, and I gradually got better at it. All of the fabrication was done with an angle grinder, stepped drill bit, m4 taps and 3d printed parts, outside the parts that I had already fabricated. 

![Board itself]({{ site.baseurl }}/images/owheelfinal/indagrass.jpg)

The wooden decks were already machined back at the university before the break. The wheel hub was cast which I detailed in previous posts. The rest was cutting and drilling, tapping and screwing. The most complicated part was placing the controller boards and battery snugly in the frame. In the picture above you can see the button which is depressed by the front foot which activates the self balancing. The actual Onewheels use a pressure sensor, though I made sure to leave a large enough gap and use a strong enough spring so that this button can't get stuck. The main problems with this board and the reason I tore it down to use the parts in other projects was heat rejection in the wheel hub.

![Wheel casting]({{ site.baseurl }}/images/wheelcasting/WheelAssem.jpg)

The wheel assembly is two "hoverboard" wheels bolted together with a cast hub. This entire assembly is surrounded by an inner tube and 10" go-kart tire. During the first time I took it to the park to try and do a range test I found that not only was it pretty terrible at climbing hills, after being loaded for so long the motors had heated up quite a bit. I had no indication of the heat until the inner tube melted and deflated. Turns out enclosing most of the wheels in a insulating layer of rubber and air makes it not release heat as well, or maybe it didn't matter when it had a small solid core tire on.

![power button]({{ site.baseurl }}/images/owheelfinal/power button.jpg)
![xlr charging connector]({{ site.baseurl }}/images/owheelfinal/xlrconnector.jpg)

The power button and charger were recycled from the donor hoverboard and ported through the frame rail. Both the battery and control board were an enclosed module which could have been waterproofed if this ended up surviving longer than a couple days. 

![10s3p battery]({{ site.baseurl }}/images/owheelfinal/10s3p.jpg)

Here is the 36 volt about 100 Watt-hour battery I built for the board. I used some Vruzend 18650 caps to assemble the battery out of recycled cells. The Vruzend kit was much more affordable than a spot welder and it held up well. Many people use these to build E-Bike or offgrid power batteries with recycled cells since they can be easily disassembled and repaired if cells die. The battery pack was 10 cells in series since that was the same as the what the donor hoverboard used.

![Bumper]({{ site.baseurl }}/images/owheelfinal/enclosed.jpg)

Each side had a symmetrical bumper which was 3d printed and thick so that it would wear down over time to protect the batteries/control board.

![control board]({{ site.baseurl }}/images/owheelfinal/controller.jpg)

The motor controller was originally bolted to the casing and I bolted it to a metal plate on my creation as well, but I also covered it with PC thermal paste to help it reject heat. 

![steel sheet]({{ site.baseurl }}/images/owheelfinal/steelsheetadded.jpg)

Both sides were finished off with a steel sheet.

The main problem was the wheel hub overheating and I didn't have a good way to prevent that even if I did get another inner tube, so this project ended up getting disassembled so that I could use the parts for something else. Even though I drilled holes in each of the hoverboard motors I disconnected them from the hub and both motors can still be used independently. I would like to use them for a large robot, some kind of base I can build obstacle avoidance into and put an arm on top. Some kind of functional robot, perhaps using ROS. 