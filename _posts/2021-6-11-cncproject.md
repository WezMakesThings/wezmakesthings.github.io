---
layout: post
title: Second Hand Cheap CNC. Part 1
---

![cnc on my table]({{ site.baseurl }}/images/6040/cncontable.jpg)
I bought this practically brand new cnc router from a machine shop in Florida. They shipped it to me on a pallet and pictured above is the first time I got it off of the garage floor.

This machine is a "6040" they're cheap machines you find practically only on eBay and AliExpress. Cheap in the CNC world can mean different things to different people. In hobby CNC a $2,000 X-carve is cheap, some "Pro" routers can approach $10,000. These 6040 machines typically cost around $1,000 shipped from china. I was lucky to find a machine shop in Florida practically giving them away, likely because they were far under powered for their application.

The name comes from the bed dimensions. 600mm x 400mm although all of that doesn't translate into the size of a part you can cut out. The T slot aluminum bed itself is flimsy. 1/4-20 nuts fit into it so I plan to bolt a spoil board to it which will add some rigidity for cutting wood though when I want to start cutting aluminum I'll probably have to upgrade to a steel bed. 

After setting up all of the electronics on the table and getting the water pump set up for cooling the spindle it was time to turn on the included computer which should have had the software installed to drive the machine. Sometimes these will have a pirated or trial version of Mach 3 installed but I was hoping I might actually find a full version of it since this was set up at a machine shop.

![bluescreen]({{ site.baseurl }}/images/6040/bluescreen.jpg)

Unfortunatly something must have came loose during shipping since the computer that came with the machine is having a good ol fashion windows XP BSOD boot loop. Not the end of the world I likely need to open the computer and reseat all the connections but this got me thinking as to alternatives for controlling this router.

With no guarantee that I'll be able to use the software on this computer even if I fix it I've started doing research into open source alternatives to Mach 3 and control electronics for a 3 axis machine. LinuxCNC seems like the best bet but I need to spend a lot more time reading and understanding it's documentation since it requires specific hardware and doesn't have an easy getting started guide. While I may end up spending another couple $100 on control electronics going with linuxCNC saves me money and is full featured. I've also heard the electronics on these machines are crap.

![crap]({{ site.baseurl }}/images/6040/controller.jpg)

Here is the 3 axis stepper driver posing as a true control system. A quick google search pulls up some online schematics that are *close* to what I have. 

![schematic](https://uploads.tapatalk-cdn.com/20190327/f86ce97eb6ee356c310b5b8c2c5dc17b.jpg)

This is helpful enough, it shows where I need to connect limit switches if I want to use this board temporarily, and we can identify the stepper drivers here as TB6560 or similar. Might be a TB6600 which affords higher current and voltage. Though both packages have longevity issues from what I'm reading online. 

