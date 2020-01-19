---
layout: post
title: Lathe Problems. 
---

Taking a look at different parts of the mini-lathe that need serious attention for this project to work. 

### Top Slide

![topslide]({{ site.baseurl }}/images/lathe/backlashproblem.jpg)
This thing has about 1.5mm of backlash in the screw. Its honestly garbage and will need to be removed from the lathe entirely. I'll likely replace this with a solid block of aluminum or steel. The function of the top slide will be completely replaced by the computer control anyway so this isn't a big deal. This explains the really bad time I've had cutting tapers.

![drive gear]({{ site.baseurl }}/images/lathe/drivegear.jpg)
The drive gear for the spindle has a crack in it and the whole gear has a slight twist to it because of this. It looks like the cause of the crack is that the center hole was to far undersized and eventually with use it just cracked. The shaft is an even 5mm so I can easily replace this with a proper timing pulley and an appropriate belt. Its just a matter of specifying that part. 

![spindle speed disp]({{ site.baseurl }}/images/lathe/spindlespeedind.jpg)
The spindle speed indicator is the only place a microcontroller is found here. But it takes some serious shortcuts. The last digit is hardwired to display zero, I think this was done to increase the human readability of the display. But this will also be removed in favor of a custom spindle tachometer which will send the speed to the controller. 