# Future Diary Phone — A Retro-Futuristic Fortune Prototype  
**Shengtao Shen | Research at Scale, Shenzhen 2026**

> A phone that doesn’t “predict” the future as a fact, but performs the future as a ritual: a daily prompt, a warning, a rewrite, a small spell.

---

## Table of Contents
- [0. Arrival & First Impressions](#0-arrival--first-impressions)
- [1. Huaqiangbei: Repair Culture & the Museum of Phones](#1-huaqiangbei-repair-culture--the-museum-of-phones)
- [2. A Childhood Reference: *Mirai Nikki* (Future Diary)](#2-a-childhood-reference-mirai-nikki-future-diary)
- [3. What Does “Future” Mean in an LLM Era?](#3-what-does-future-mean-in-an-llm-era)
- [4. Prototype V0: GPS + Time → Diary Messages](#4-prototype-v0-gps--time--diary-messages)
- [5. The Problem: Random Futures, Beautiful but Unreliable](#5-the-problem-random-futures-beautiful-but-unreliable)
- [6. Shifting the Concept: From Prediction to Fortune](#6-shifting-the-concept-from-prediction-to-fortune)
- [7. Interaction Design: Keypad Rituals](#7-interaction-design-keypad-rituals)
- [8. Rewriting: When Movement Changes the Story](#8-rewriting-when-movement-changes-the-story)
- [9. Voice Interaction (Attempt & Failure)](#9-voice-interaction-attempt--failure)
- [10. Form Factor: Toward a Retro-Future Aesthetic](#10-form-factor-toward-a-retro-future-aesthetic)
- [11. Open Questions & Next Steps](#11-open-questions--next-steps)

---

## 0. Arrival & First Impressions

I began this residency with a simple feeling: **Shenzhen is not a city you “visit”—it is a city you calibrate to.**  
Everything is dense, fast, modular, and repairable. Hardware is not hidden behind branding; it is exposed as a living ecosystem of parts, vendors, and hands.

I came here wanting to build a device, but also to understand a different relationship between people and electronics:  
not consumption, but **maintenance**, **modification**, and **street-level expertise**.

![Fig 01 — First day in Shenzhen](assets/img/01.png)

---

## 1. Huaqiangbei: Repair Culture & the Museum of Phones

My first stop was **Huaqiangbei**. I walked through endless rows of phone repair stalls and phone shops—screens, batteries, camera modules, tiny screws, adhesives. The space felt like an open laboratory where the phone is no longer sacred: it is **repairable**, **swappable**, **hackable**.

![Fig 02 — Huaqiangbei street scenes](assets/img/02.png)
![Fig 03 — Repair stalls / parts displays](assets/img/03.png)

Then a quiet place caught my attention: **Huaqiangbei Museum**.

It collects phones from the late 1990s to early 2010s—flip phones, candy-bar phones, early touch phones. Nobody uses them now, but their design logic is still vivid:  
physical buttons, tactile constraints, dedicated functions, playful UI metaphors.

![Fig 04 — Huaqiangbei Museum exterior / signage](assets/img/04.png)
![Fig 05 — Flip phones & early devices](assets/img/05.png)
![Fig 06 — Detail shots: hinges, buttons, screen proportions](assets/img/06.png)

What impressed me wasn’t nostalgia. It was **clarity**:  
these devices had fewer inputs, but the interactions felt intentional and legible.

---

## 2. A Childhood Reference: *Mirai Nikki* (Future Diary)

The museum triggered a memory from childhood: the anime **_Mirai Nikki_ (Future Diary)**.

In the story, the protagonist receives a phone that delivers “future diary” entries at irregular intervals. It does not show a map of tomorrow—it sends short messages that become both guidance and curse. You are never sure whether you are reading fate, probability, or manipulation.

That narrative became my seed:

**What if a phone doesn’t optimize your present, but haunts it—gently—with possible futures?**

![Fig 07 — Future Diary reference / mood](assets/img/07.png)
![Fig 08 — “Diary message” visual inspiration](assets/img/08.png)

---

## 3. What Does “Future” Mean in an LLM Era?

I initially thought: we now have LLMs, we have sensors, we have GPS—so the future diary can be computational.

But soon I realized:  
LLMs do not “know” the future. They generate futures that feel plausible, poetic, or dramatic.

So I reframed the question:

- If prediction is unreliable, can it still be meaningful?
- If accuracy is impossible, can the device still produce **agency**?
- What if the “future diary” is not truth, but a **ritual interface**?

This project became less about forecasting and more about **how we interact with uncertainty**.

![Fig 09 — Concept sketches / notes](assets/img/09.png)

---

## 4. Prototype V0: GPS + Time → Diary Messages

The first prototype is simple in principle:

**Inputs**
- GPS location (where you are)
- Time (when you are)

**Process**
- Send to an LLM API
- Generate a “future entry”
- Display it as a push-like message on the device

The goal: the phone periodically whispers what might happen next.

![Fig 10 — System diagram (GPS + time + LLM)](assets/img/10.png)
![Fig 11 — Early screen/UI tests](assets/img/11.png)
![Fig 12 — Prototype desk setup](assets/img/12.png)

---

## 5. The Problem: Random Futures, Beautiful but Unreliable

This version produced messages that were sometimes eerie and sometimes funny—but rarely grounded.

It felt less like prophecy and more like **machine improvisation**.

And that was the turning point:  
I didn’t want the device to pretend it was “accurate.”  
I wanted it to be honest about what it is: a machine that generates possibilities.

So the design direction shifted:

From **prediction** → to **fortune**.

![Fig 13 — Examples of early diary outputs](assets/img/13.png)
![Fig 14 — Notes on “randomness” and “meaning”](assets/img/14.png)

---

## 6. Shifting the Concept: From Prediction to Fortune

In many cultures, fortune-telling is not about objective truth.  
It is a performative structure that helps you read your day differently.

A fortune machine can be:
- comforting
- warning
- playful
- interpretive

In this framing, the Future Diary Phone becomes less like a navigation app and more like a small daily oracle.

**The future is not delivered as a schedule—  
it is delivered as a prompt.**

![Fig 15 — Fortune machine references / keypad objects](assets/img/15.png)

---

## 7. Interaction Design: Keypad Rituals

I introduced a physical keypad and mapped keys into “ritual functions.”  
This moved the device away from passive prediction toward **active participation**.

### Current key mappings
- **Press 1** → Today’s luck + lucky color + a small blessing  
- **Press 3** → A warning: what to avoid today  
- **Press 4** → Summary of the last few diary entries  
- **Press 6** → What tomorrow might bring

Each key becomes a deliberate gesture:  
not “tell me the truth,” but “give me a lens.”

![Fig 16 — Keypad wiring / integration](assets/img/16.png)
![Fig 17 — Key mapping chart](assets/img/17.png)
![Fig 18 — UI shots: luck / warning / summary](assets/img/18.png)

### Why physical buttons?
Because they slow you down. They make the request feel intentional.  
And they echo the old phones in the museum:  
a time when interaction was not infinite scroll, but discrete actions.

![Fig 19 — Button-driven interaction inspiration](assets/img/19.png)

---

## 8. Rewriting: When Movement Changes the Story

I added a feature I call **Rewriting**:

When the device detects a **large change in travel distance**, it considers the future “rewritten.”  
The diary updates because the world context has shifted.

This is a narrative mechanic:
- Small movement → small drift in the diary’s tone
- Major relocation → the diary “edits itself,” like fate has been rewritten

It also reflects a simple belief:
**the future is not one line. It branches.**

![Fig 20 — Rewriting logic / movement thresholds](assets/img/20.png)
![Fig 21 — Tests / debug screenshots for movement change](assets/img/21.png)
![Fig 22 — “Before rewrite / after rewrite” examples](assets/img/22.png)

---

## 9. Voice Interaction (Attempt & Failure)

I also tried to integrate voice interaction, imagining the phone as something you could speak to.  
Voice would enable more ambiguity: tone, hesitation, confession.

But I failed in this iteration:
- the pipeline was unstable
- latency and audio routing were inconsistent
- the interaction felt worse than buttons

Still, I see voice as a future layer—not as a replacement for the keypad, but as a second mode.

![Fig 23 — Voice attempt / hardware setup](assets/img/23.png)
![Fig 24 — Notes on failure & future plan](assets/img/24.png)

---

## 10. Form Factor: Toward a Retro-Future Aesthetic

My next step is to design the body of the device.

I want a form that feels **retro-futuristic**:
- nostalgic enough to evoke old devices
- strange enough to feel like an artifact from an imagined future

This is not “sleek minimalism.”  
It is a **future that still has screws**, seams, textures, and personality.

Possible directions:
- flip-phone silhouette (hinge as narrative gesture)
- chunky keycaps / visible keypad
- small screen, high contrast UI
- a “worn future” that looks carried, not displayed

![Fig 25 — Form factor sketches](assets/img/25.png)
![Fig 26 — Material / aesthetic references](assets/img/26.png)
![Fig 27 — Prototype enclosure experiments](assets/img/27.png)

---

## 11. Open Questions & Next Steps

This prototype led me to a larger question:

**What inputs could ever meaningfully “predict” a personal future?**  
GPS and time are not enough.

Possible input directions (future exploration):
- routine patterns (but that risks surveillance)
- calendar + social signals (but that risks over-determination)
- mood / voice tone (more intimate, less factual)
- environmental sensors (air, light, sound)
- your own “diary” as training context (memory as future seed)

Maybe the future diary shouldn’t “predict” at all.  
Maybe it should help you **notice**:  
what you fear, what you desire, what you repeat.

![Fig 28 — Brainstorm diagrams](assets/img/28.png)
![Fig 29 — Next-step hardware/UI notes](assets/img/29.png)
![Fig 30 — Closing image / prototype in hand](assets/img/30.png)

---

## A question for you

If you had a Future Diary Phone, would you want it to:
- be accurate, like a forecast?
- be symbolic, like a fortune?
- be playful, like a game?
- or be intimate, like a diary that writes back?

**Would you want to own one?**
