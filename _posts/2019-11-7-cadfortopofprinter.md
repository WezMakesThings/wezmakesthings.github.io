---
layout: post
title: Linear Rail Printer Design
---

Continuing work on the 3D printer. 
![Steel and Rails]({{ site.baseurl }}/images/3dprinter/v4struct.png)

A major design criteria for this project is that the physical design is as rigid and consistent as possible. For this I looked into what sort of equipment is used in desktop milling machines and high performance printers. All sources point to linear rails or much thicker high quality bearing rods. It is the general consensus (in the 3d printing community) that even low quality linear rails will be better than possibly bent or low quality rods. 

Another criteria is ease on manufacture. I'm in contact with a member of the college who works with LEAN manufacturing and he's been an amazing resource. I've made only three parts of this assembly out of metal, and they're all 2d profiles. Only one requires a bend.

Although the main plate is very large. In the next iteration I'll be splitting that plate into two identical halves. 

An important note is the kinematics we've chosen for the printer. This design is commonly called H-bot. It does have some drawbacks such as a torque around the main gantry arm. This is mitigated in the design by using two bearing blocks on each side of the arm. Many who try this design and fail are using 3d printed or other parts that have lots of play and thus cause issues. The main advantage of this design over CoreXY for example is only one belt path that is all in the same plane. CoreXY printers require the belt to pass over itself and many more idlers adding lots of complexity to the design.