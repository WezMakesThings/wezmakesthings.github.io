---
layout: post
title: Designing 3d printed parts for strength
---

#### Taking into account stress concentrations
![3d printed go pro mount]({{ site.baseurl }}/images/3dprintedgopromount.jpg)
With an FDM printer the strength of a 3d printed part depends on many factors as its being printed. So much so that a engineering strain curve for the plastic wouldn't be very helpful for a specific printed part. Many filaments have color and other additives that change the properties of the plastic. Material data sheets aren't popular for rolls of filament unlike UV resins. Its difficult to do some proper mechanical engineering without the elastic modulus and yield point of the plastic. Though a decent approximation can be done using the anisotrpoic nature in the layered structure of an FDM part.

![3D print layers](https://images.squarespace-cdn.com/content/v1/5aa7425d697a98647314b490/1561183950912-QPHXRH3CSPS6JLJ63CHJ/ke17ZwdGBToddI8pDm48kAdtU4fTrGbiKn7Ng_9KivlZw-zPPgdn4jUwVcJE1ZvWQUxwkmyExglNqGp0IvTJZUJFbgE-7XRK3dMEBRBhUpx2nX4JF6h6e2ZLpJYieoYH2iC55G3aPDaWeuWKkShdKaQRYo9CYmx5MdFwMlTbOOQ/3dPrintProcessDiagram.png?format=750w)
*3d-pros.com*

The anisotropic nature of FDM parts like all anisotropic structures is due to how it is formed, the layered construction of extruded filament fuses fully where it is a continuous line and only partly between layers since the layer below has cooled and is only partially melted and fused by the hot plastic on top. If we call the direction perpendicular to the layers Z, then the printed part is always weakest in the Z direction and strongest in the X and Y directions.

![3d part design]({{ site.baseurl }}/images/3dgpm/part.jpg)

Here is the part I would like to print. Its a simple part meant to bolt to the top of my quadcopter and have a GoPro connected to it. A few considerations: I would like for it to be a quick print, while I'm designing this to be as strong as possible, the 3d printed plastic is going to be weaker than the injection molded plastic GoPro case and the carbon fiber frame. In a crash this part will likely break before anything else does. Next, what orientation should this part be printed in. Lets consider the most obvious ones. Again the Z direction is the direction perpendicular to the print bed and layers. 

![Z up]({{ site.baseurl }}/images/3dgpm/ort1.jpg) 
*orientation with the largest face on the bottom*

If we orient the largest face on the bottom which would be the easiest to print lets look at where this part would fail. 

![Normal Failure]({{ site.baseurl }}/images/3dgpm/normal.jpg)

Shown here is the internal normal stress caused by the bolt holding the GoPro if it were to be pulled upward at stress concentration A-A. The normal stress is parallel to the layer lines thus a likely failure. 

![Shear Failure]({{ site.baseurl }}/images/3dgpm/shear.jpg)

Rotating the Z direction 90 degrees is not much help either since we would then expect a shear failure at the stress concentration. Ruling out these possibilities the optimal Z direction for this part would be out of the screen (towards you) Though its not that simple. Lets take a look at the rest of the part.

![To much support still shear failure]({{ site.baseurl }}/images/3dgpm/problem.jpg)

Printing the whole part in one piece like this would just move the shear failure down into the base and require a lot of support and post processing. This is not the solution either. In the end what I went with was printing in 4 parts.

![]({{ site.baseurl }}/images/3dgpm/1.jpg)
![]({{ site.baseurl }}/images/3dgpm/2.jpg)
![]({{ site.baseurl }}/images/3dgpm/3.jpg)

One slotted base and 3 identical vertical parts. These each slide in from the bottom and mate with a chamfer. When bolted to the top of the drone it is all held in place with mechanical retention and the part is strong in the directions it needs strength. Printed without supports in 20 minutes, meeting all requirements. Just like machining splitting up your part in creative ways can allow for easier fabrication and greater strength in 3d printing.