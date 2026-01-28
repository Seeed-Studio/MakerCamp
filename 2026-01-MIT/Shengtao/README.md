# Future Diary Phone (Prototype) — Shengtao

## Overview
This is a prototype built during a residency in Shenzhen. It started from Huaqiangbei (repair / resale culture + old phone designs) and the anime *Mirai Nikki (Future Diary)*.

At the beginning, the goal was simple: make a “Future Diary Phone” that outputs messages about what will happen next. After testing, I realized that “prediction” is not the right framing for this device (at least not with the inputs I had). The project shifted toward a keypad-based fortune / diary machine, with a rewriting trigger that updates the result when your movement changes.

This README documents the concept shift and what I built so far.

---

## Huaqiangbei
I went to Huaqiangbei and saw many phone repair and phone resale stores. The density of services and parts is very different from what I’m used to: screens, batteries, camera modules, cables, tiny screws, and many “micro-skills” that people learn through practice. It feels like the phone is not a sealed product here. It is something that can be opened, replaced, and recombined.

A place that caught my attention was the Huaqiangbei Museum. It collects phones from around the 2000s (flip phones, feature phones, early mobile products). These phones are not used anymore, but their form factor and button-driven interaction are still impressive.

What I like about these devices:
- Clear constraints (small screens, limited input)
- Strong physical feedback (buttons, hinges, covers)
- Dedicated actions (each press does something specific)
- The device feels like a tool, not a feed

This visit set the tone for the project: I wanted my prototype to feel more like a “device” than a generic app.

<img src="1.png" width="100%" />
<img src="2.png" width="100%" />

<img src="3.png" width="100%" />

<!-- 4–8 in one row -->
<div>
  <img src="4.png" width="19%" />
  <img src="5.png" width="19%" />
  <img src="6.png" width="19%" />
  <img src="7.png" width="19%" />
  <img src="8.png" width="19%" />
</div>

<img src="9.png" width="100%" />

---

## Reference: Mirai Nikki (Future Diary)
This reminded me of the anime *Mirai Nikki (Future Diary)*. In the story, the protagonist receives a phone that gets messages about future events. The messages arrive irregularly. They are short, direct, and sometimes scary. The key part for me is not the plot, but the interaction format:
- a device that sends you a “future entry”
- you don’t fully control when it arrives
- the message changes how you act in the present

This is why “Future Diary” works as a product concept: it’s not a normal tool, it changes your mindset. I wanted to build a prototype that can deliver that feeling, even if the “future” is not truly real.

<img src="10.png" width="100%" />

Video: [Open 1.mp4](1.mp4)

---

## Prototype V0: GPS + time → “future diary” messages
I started with a simple pipeline:
- Input: GPS location + current time  
- Send to an LLM API  
- Output: future diary messages shown on the screen  

The idea was: if the device knows *where you are* and *when you are*, it can generate a context-based “future.” The phone would periodically show a message like a diary entry.

<img src="11.png" width="100%" />

However, the “future” was not accurate. It often felt like random generation. The messages could be interesting, but they were not grounded. It was more like “LLM imagination” than “prediction.”

This became the core design problem:
- If the output is not accurate, users will not trust it as a prediction tool.
- If it is just random, it becomes a toy, and the concept loses weight.

Instead of trying to force accuracy, I changed the product framing. I stopped treating it as “predicting the future” and moved toward “a fortune / oracle device.” That direction matches the behavior of the system better (a machine that generates possible futures, not verified futures).

<img src="12.png" width="100%" />

<img src="13.png" width="100%" />
<img src="14.png" width="100%" />

---

## Interaction: keypad functions (fortune / oracle mode)
After the concept shift, I wanted a clearer interaction structure. In Huaqiangbei Museum, old phones feel direct: buttons, actions, feedback. So I added a keypad and mapped keys to specific functions.

This made the device more interactive and less dependent on “accurate future prediction.” It also changes the user relationship: instead of passively receiving a message, you actively request a certain type of output.

<img src="15.png" width="100%" />
<img src="17.png" width="100%" />

Current mapping:
- Press **1**: today’s luck + lucky color  
  This is a lightweight daily output. It is not “true” or “false,” but it gives a starting point and a tone.  
  Video: [Open fortune.mp4](fortune.mp4)

- Press **3**: warning / things to watch out for today  
  This output is designed to be more “practical” (what to avoid, what to pay attention to).  
  Video: [Open warning.mp4](warning.mp4)

- Press **4**: summarize previous future diary entries  
  Since the device generates multiple entries, it needs a way to compress them. This is important for readability and continuity.

- Press **6**: tomorrow’s possible events  
  This is closer to the original “future diary” idea, but now it is framed as “possible tomorrow,” not guaranteed tomorrow.  
  Video: [Open tomorrow.mp4](tomorrow.mp4)

This version feels closer to a “fortune machine” than a forecasting device. The device is still about the future, but it becomes a controlled interaction: different buttons = different kinds of future.

---

## Rewriting: future changes when movement changes
One issue with any “future diary” system is that the future should not be fixed. If you move to a different place, your next day should not read the same. So I added a rewriting mechanism.

Video: [Open 2.mp4](2.mp4)

I added a rewriting feature:
- If travel distance changes a lot, the diary result should update (the “future” is rewritten).
- This is a rule-based trigger for now.

The goal is simple: make the device respond to real-world change. Even if the diary is speculative, it should at least acknowledge that context has changed.

Video: [Open Rewrite.mp4](Rewrite.mp4)

---

## Voice interaction (attempt)
I also tried to add voice interaction, because speaking is a natural input for “fortune/oracle” devices. Voice could allow:
- faster input than typing
- more emotional cues
- a more personal interaction mode

But it did not work reliably in this iteration. The main issues were stability and audio pipeline reliability (recording, recognition, playback). I decided not to force it into the current prototype, but I want to solve it later.

<img src="16.png" width="100%" />

Below is the full component + wiring / connection diagram for the system.

<img src="18.png" width="100%" />

---

## Next step
Next I will focus on:
- the physical form factor (retro-future look)

I want the device to look like a phone, but not like a modern smartphone. I want it to have a “retro future” feel: a limited interface, clear controls, and a physical identity. The goal is to make it feel like a dedicated object, not a general-purpose computer.

<img src="19.png" width="100%" />

- what kinds of inputs could make the “future diary” more meaningful (without turning it into surveillance)

GPS + time is too weak. It gives context but not enough personal structure. In the future, I may explore additional inputs (for example: occupation, personality traits, personal background data, etc.). With richer inputs, the “future diary” might feel more grounded and less random.

I hope a real Future Diary device could exist one day.
