## Jake in Shenzhen ! 

I am two months away from defending [my thesis](https://jakeread.github.io/thesis/) on machine control at the [Center for Bits and Atoms](https://cba.mit.edu/about/index.html). There are about four different projects that I would like to work on once I'm done with the PhD, so I came to Shenzhen in a forwards-looking way, i.e. to learn about where my own hopes might fit into the world's manufacturing ecosystem. 

![joyous](images/2026-01-10_pic-0019.jpg)

I absorbed a lot, and am really grateful to Seeed and Cedric for hosting - I wrote much of this down in [this post](https://ekswhyzee.com/2026/01/20/shenzhen.html) on my 16 hour flight home. 

### Accelerometer PCBA with Seeed Fusion

As part of my thesis work, I needed to finish an [accelerometer module.](https://github.com/jakeread/knuckles-imu-lsm6-lis2-rp2354a) This is part of a [family of modular circuits](https://jakeread.github.io/thesis/04_00_knuckles.html) that I have been cooking up with the goal of enabling *almost anyone* to build or modify their own machine control system.

![knuckles](images/knuckles-kit.jpg) 

![knuckles](images/knuckles.png)

| | |
| --- | --- |
| ![](images/preview_back.jpg) | ![](images/preview_front.jpg) |
| ![](images/2026-01-13_pic-0065.jpg) | ![](images/2026-01-13_pic-0067.jpg)

![tweezies](images/2026-01-13_pic-0047.jpg)  
> PCBA ! My shaky hands could never tweeze those 0402's.    

![reflow](images/2026-01-13_pic-0052.jpg) 
> Accelerometer module in the oven at Seeed.

Watching this circuit go together at Seeed was awesome, although I was surprised at the volume required to move from PCBA-by-hand onto the PNP machines. 

<video controls width="100%" muted="true">
  <source src="videos/2026-01-13_vid-0016-timecrop.mp4" type="video/mp4">
</video>

I've been able to bring this board online and next week it will be integrated into my machine controllers to help better estimate machine kinematic [models](https://jakeread.github.io/thesis/06_00_models-motion.html) and stiffnesses - and hopefully detect chatter in CNC machining. 

### Motor Manufacturing and Controller Interfaces 

Machine control begins with motor control, and I've been working on [closed loop stepper controllers](https://ekswhyzee.com/2025/03/24/foc-stepper.html) for some time. 

Closing the loop on motors we use for machine design is helpful because we can read states out of the machine and treat them to controls more akin to what we see in modern robotics (ML, Dynamics, etc !) than what we see in industrial control (which is stuck in the 1990's).

<video controls width="100%" muted="true">
  <source src="videos/little-guy-digital-twin.mp4" type="video/mp4">
</video>

Making them modular also helps when we want to do silly projects really quickly... 

<video controls width="100%" muted="true">
  <source src="videos/2025-06-06_homing.mp4" type="video/mp4">
</video>

One pain point with these projects is integrating the motor and the controller, so I cooked up [this interface proposal](https://github.com/jakeread/nema-motor-controller-iface-proposal) as a prototype open spec. 

| | | | | |
| --- | --- | --- | --- | --- |
| [Jake's FOC Stepper](https://ekswhyzee.com/2025/03/24/foc-stepper.html) | [Mechaduino](https://hackaday.io/project/11224-mechaduino) | [CLN17](https://hackaday.io/project/192759/logs) | [SERVO42C](https://makerbase3d.com/product/servo42c-nema17-closed-loop-stepper-motor-driver-cnc-3d-printer-parts-prevents-losing-steps-for-gen_l-sgen_l/) | [PD Stepper](https://www.sparkfun.com/pd-stepper.html) |
| ![img](images/stepper-cl.jpg) | ![mecha](images/mechaduino.jpg) | ![cl](images/cln17.jpg) | ![42](images/servo42c.jpg) | ![pd](images/pd-stepper.webp) |

![](images/2026-01-15_proposal.png)

To get a better sense of how this might work, Seeed hooked me up with a visit to a motor factory. Docs from that visit are [in this post](https://ekswhyzee.com/2026/01/20/shenzhen.html) (about 70% down). It was a joy to see how the motor-sausage is made, and was really valuable for me to understand how to better interact with plants like this in the future. 

<video controls width="100%" muted="true">
  <source src="videos/2026-01-16_vid-0005.mp4" type="video/mp4">
</video>

### Labubus

A worthy sidequest, I helped Miranda to build the [mf labububot](https://github.com/mirandali707/labububot/tree/main), a twelve-headed monster-ball.

![](images/2026-01-11_labubu-cad.png)
![](../Miranda/labubu_guillotine.jpg) 

<video controls width="100%" muted="true">
  <source src="videos/2026-01-17_vid-0009.mp4" type="video/mp4">
</video>

<video controls width="100%" muted="true">
  <source src="videos/2026-01-17_vid-0010.mp4" type="video/mp4">
</video>

![](images/2026-01-18_pic-0008.jpg)