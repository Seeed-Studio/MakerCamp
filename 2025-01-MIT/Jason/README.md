# My visit to Shenzhen
I had the amazing opportunity to visit Shenzhen in January 2025 for the Research at Scale residency and the Scalable HCI Symposium. It was my first time in Southern China, and I had a blast. Here are some of the highlights documented below. Big thank you to Seeed Studio for hosting us and sponsoring our trip!
<p align="center">
  <img src="./images/img1.jpg" width="600">
</p>
<p align="center"><em>MIT residents at Chaihuo Makerspace</em></p>

## Hackathon

We started off the trip with a 2-day hackathon sponsored by Seeed and Anker. The hackathon had a 'smart spaces' theme and featured talented engineering students and employees from Shenzhen and Symposium attendees.

We worked a couple of late nights to make the demo below. **[Little Brother](https://youtu.be/nWw6RP7YdS4)** (yes, Orwell reference) is an AI-powered camera end effector for a room-scale cable-driven gantry robot. That's right, a [Skycam](https://www.youtube.com/watch?v=WNtNBNoVFHI) for your room. Other than capturing b-roll footage of your life, we envisioned that Little Brother could be useful for helping direct you to lost items, tidy up, or address non-line of sight surveillance (too Orwellian). Little Brother is a helpful workshop companion! I helped build the robot, write the NLU speech-to-command core, and survive integration hell.

<p align="center">
  <img src="./images/img2.jpg" width="600">
</p>
<p align="center"><em>Check out the youtube video</em></p>

## Designing PCBs for ultrasound transducers

I had originally hoped to make use of the PCB-in-a-day ecosystem, but I was a bit caught up and ended up spending more time designing new PCBs. I found the hotel room lab with HQB equipment a nice environment to work. The end of our trip ran into the Chinese New Year holiday break, so I didn't assemble and test my boards until I got back. The first board is a battery-powered piezo driver that can output +/- 7V, 100mA and drive a programmed signal from 200kHz to 1MHz. This is a specialty driver board that does not really have an off-the-shelf counterpart other than a bulky tabletop function generator. We have to lug it around to BU/Harvard regularly, so it would be nice to have an alternative.
<p align="center">
  <img src="./images/img3.JPEG" width="600">
</p>
<p align="center"><em>Sine wave generator PCB with device after assembly</em></p>
<p align="center">
  <img src="./images/img4.png" width="600">
</p>
<p align="center"><em>SEPIC schematic</em></p>

I also designed a single-ended primary inductor coil (SEPIC) switching converter to convert a 5V USB supply into a +/-50V supply for ultrasound imaging/histotripsy.

I also bought and took apart a high intensity ultrasound unit for cosmetics to check out the ultrasound driver circuit. It was less interesting than I thought but it's a MOSFET off a 24V wallwart supply that drives a 1.73 MHz sine wave at 10Vpp through a 5 ohm piezo directly (with no matching layer or cover?). The piezo is run in thickness vibration mode. I was surprised but this device is easily able to atomize water droplets and induce a hot feeling in your skin. Likely a little sketch.
<p align="center">
  <img src="./images/img5.JPEG" width="600">
</p>
<p align="center"><em>HIFU cosmetic ultrasound teardown</em></p>
I was also able to source some curved piezoceramic disks that can be driven at 2MHz. They are curved and thus focused, allowing for fairly high pressures to be driven with lower voltages.
<p align="center">
  <img src="./images/img6.JPEG" width="600">
</p>
<p align="center"><em>Curved piezoceramic disks (excuse my dirty fingers)</em></p>

**Taobao** turned out to be a great resource for sourcing specialty materials such as custom piezoceramics, hydrogel chemicals, and just about anything else you could hope to buy in Shenzhen. The city provides the window shopping experience, but the online marketplace is up-to-date and all-encompassing. The app also has an excellent picture-search feature that bridges the experience. I ended up using Taobao to buy items that are really only available to Chinese addresses and phone numbers. It was also very useful for negotiating prices at the market and at least having a reference point.
<p align="center">
  <img src="./images/img7.PNG" width="600">
</p>
<p align="center"><em>Taobao image search</em></p>

## EEG device and printed electrodes
I was able to find an EEG frontend chip for about 10x cheaper than in the states. It's made by Kingsense, and I was able to source a dev board and a handful of chips. One of my goals on this trip was to integrate some 2-p 3D printed microneedle array dry electrodes into an EEG device. I made some prototypes with the Intan RHD2216, but I hope to put the whole system together in the coming months.
<p align="center">
  <img src="./images/img8.jpeg" width="600">
</p>
<p align="center"><em>KS1092 chip on Taobao</em></p>
<p align="center">
  <img src="./images/img10.png" width="600">
</p>
<p align="center"><em>2-p 3D printed microneedle array under scope</em></p>
<p align="center">
  <img src="./images/img9.JPEG" width="600">
</p>
<p align="center"><em>Dry electrodes silver epoxied onto EEG electrodes</em></p>


Also in the works is trying to formulate a PEDOT:PSS ink that can be thermal inkjet printed. I was able to source some PEDOT:PSS, sodium alginate, and calcium chloride, and I even brought a handheld inkjet printer and an empty cartridge (rare). I didn't get to put everything together yet, but I'm hoping to test it soon.
<p align="center">
  <img src="./images/img12.jpeg" width="600">
</p>
<p align="center"><em>Cheap PEDOT:PSS on Taobao</em></p>

## Finding specialty parts and materials
I was able to find some specialty parts and materials on Taobao and in Huang Qiang Bei market.
PEDOT:PSS (freeze-dried and screen-printable)
Sodium alginate + calcium chloride (for hydrogels)
EEG frontend chip
High Frequency Ultrasound cosmetic device
Portable spot welder
Mini dremel
3-in-one (multimeter, oscilloscope, function generator)
Mini Li-Po batteries
Tiny flashlight

## Manufacturing
There are countless scales of manufacturing in the Shenzhen ecosystem. In the past 10 years, many factories have found there niche in different areas of high-volume manufacturing and compete with each other by securing high-value contracts from global consumer product areas. Unfortunately, fewer factories can be bothered to support pilot runs with no prospect of MOQs in the 1000s. While it was very cool to see the various parts being built, it seemed that many factories are specialized for ODM, finished parts, or custom assembly and were thus trying to showcase their worker-friendly conditions, efficiency, and high-tech integrations. Few of them seemed like they were competing on innovation within the product but rather innovation in manufacturing. I was amazed by some of the assembly lines, which included conveyor belts, humans-in-the-loop, and custom testing and inspection systems. 
<p align="center">
  <img src="./images/gif1.gif" width="600">
</p>
<p align="center"><em>Fast LED testing</em></p>
<p align="center">
  <img src="./images/gif2.gif" width="600">
</p>
<p align="center"><em>Standard pick-and-place</em></p>

More videos here:
https://www.notion.so/highlights-182f6600914f81a9a535e7056ce2ce39?pvs=4

#Factories visited:
- E-ink display factory
- Seeed PCB assembly factory
- WorldSemi LED factory
- KTC display factory
- Flexible PCB factory
- Smart Ring factory
- Other visit highlights:
	- A room full of Cryo-EMs at SUSTech
	- LibreLive guitar demo at InnoX
	- Visit at BrainCo with CEO
	- The top floors at SEG, HQB
	- Giant salamanders, Maine coon kittens, axolotl for sale on the streets
	- Techno club on a Sunday (Oil)
 
## Art
We were able to see a good few exhibits and meet some attendees of the Symposium who all specialize in exploring the cross-section of Art and Technology. Thank you to AIRS art & tech studio for sharing their workspace and their new exhibit, "Question of the Question". Check out the art of [Shen Shaomin](https://www.galleryek.com/artists/shen-shaomin?view=slider#2), who hosted us for many nights of drinking, dancing, and food.
<p align="center">
  <img src="./images/gif3.gif" width="600">
</p>
<p align="center"><em>Art at the new 'Question of the Question' exhibit</em></p>
<p align="center">
  <img src="./images/tongyi.jpg" width="600">
</p>
<p align="center"><em>Tongyi at AIRS</em></p>

## Cedric 
I wanted to leave a quick note about Cedric Honnet, who is an MIT PhD student in Responsive Environments, and kept the program alive by raising funding, finding sponsors, and bringing together an amazing cohort of makers, hackers, and artists. He put so much care and effort into creating an environment to share ideas, skills, and passions in technology -- all while leading our trip in Shenzhen and sharing the true best eats and experiences from a certified local.
<p align="center">
  <img src="./images/cedric.jpg" width="600">
</p>
<p align="center"><em>Cedric playing with a big light</em></p>
## Film

I shot a couple rolls of film. Here are some of the pictures that developed well.
<p align="center">
  <img src="./images/1.jpeg" width="600">
</p>
<p align="center">
  <img src="./images/2.JPEG" width="600">
</p>
<p align="center">
  <img src="./images/3.jpeg" width="600">
</p>
<p align="center">
  <img src="./images/4.JPEG" width="600">
</p><p align="center">
  <img src="./images/5.jpeg" width="600">
</p>
<p align="center">
  <img src="./images/6.JPEG" width="600">
</p>
<p align="center">
  <img src="./images/7.jpeg" width="600">
</p>
<p align="center">
  <img src="./images/8.jpeg" width="600">
</p>
<p align="center">
  <img src="./images/9.jpeg" width="600">
</p>
<p align="center">
  <img src="./images/10.JPEG" width="600">
</p>
<p align="center">
  <img src="./images/11.jpeg" width="600">
</p>
<p align="center">
  <img src="./images/12.jpeg" width="600">
</p>
<p align="center">
  <img src="./images/13.jpeg" width="600">
</p>
<p align="center">
  <img src="./images/14.jpeg" width="600">
</p>
<p align="center">
  <img src="./images/15.jpeg" width="600">
</p>
<p align="center">
  <img src="./images/16.jpeg" width="600">
</p>
