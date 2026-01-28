# Future Diary Phone (Prototype) — Shengtao

## Context
I visited Huaqiangbei and saw many phone repair / resale stores. One place stood out: the Huaqiangbei Museum. It collects phones from around the 2000s (flip phones, feature phones, etc.). These products are not used anymore, but their form factor and button-based interaction are still interesting to me.

![Huaqiangbei / museum](assets/img/01.png)
![Old phones collection](assets/img/02.png)
![Flip phones details](assets/img/03.png)

This reminded me of the anime **Mirai Nikki (Future Diary)**. In the story, the main character has a phone that receives messages about what will happen in the future.

![Mirai Nikki reference](assets/img/04.png)

So during this residency, I decided to build a **Future Diary Phone**. This is a prototype.

---

## Idea V0: “Predict the future” with GPS + time
Initial idea:
- Input: GPS location + time
- Send to an LLM API
- Output: future diary messages on the screen (pushed occasionally)

![System sketch](assets/img/05.png)
![Prototype setup](assets/img/06.png)
![Early UI test](assets/img/07.png)

Problem:
The “future” was not accurate. It felt like random generation. It was interesting sometimes, but not reliable.

![Example outputs](assets/img/08.png)
![More outputs](assets/img/09.png)

That made me rethink the project. Instead of “prediction”, I treated it more like a **fortune / oracle device**.

---

## Interaction: keypad input → different functions
I connected a keypad and mapped keys to functions. This made the device more interactive and less dependent on “accurate prediction”.

Current mapping:
- Press **1** → today’s luck + lucky color
- Press **3** → warnings for today
- Press **4** → summary of previous diary entries
- Press **6** → tomorrow’s possible events

![Keypad integration](assets/img/10.png)
![Key mapping notes](assets/img/11.png)
![UI screenshots](assets/img/12.png)
![More UI screenshots](assets/img/13.png)

This version feels closer to a “fortune machine” than a forecasting device.

---

## Rewriting: future changes when your movement changes
I added a rewriting mechanism:
- If travel distance changes a lot, the future diary should update (the “future” is rewritten).
- This is a simple rule-based trigger for now.

![Rewriting logic](assets/img/14.png)
![Movement test](assets/img/15.png)
![Before/after rewrite](assets/img/16.png)

---

## Voice interaction (attempt, failed)
I tried to add voice input, but didn’t finish it in this iteration. Main issues were stability and audio pipeline reliability. I want to solve this later.

![Voice hardware test](assets/img/17.png)
![Notes / debugging](assets/img/18.png)

---

## Next: physical design + input question
Next step is the form factor. I want a retro-future look (old phone feeling + “future device” behavior).

![Form sketches](assets/img/19.png)
![Reference images](assets/img/20.png)
![Enclosure test](assets/img/21.png)

Main open question:
What kinds of inputs can actually make “future” meaningful?
GPS + time is too weak. I want to explore other inputs, but also avoid turning this into surveillance.

![Input brainstorm](assets/img/22.png)
![More notes](assets/img/23.png)

---

## Extra process photos / visits (optional)
![Visit photo](assets/img/24.png)
![Market photo](assets/img/25.png)
![Prototype detail](assets/img/26.png)
![More detail](assets/img/27.png)
![Testing](assets/img/28.png)
![Final prototype shot](assets/img/29.png)
![Closing image](assets/img/30.png)
