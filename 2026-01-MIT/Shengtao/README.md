# Future Diary Phone (Prototype) — Shengtao

## Overview
This is a prototype built during the residency in Shenzhen. It started from Huaqiangbei (repair / resale culture + old phone designs) and the anime *Mirai Nikki (Future Diary)*. The first idea was “future prediction,” but the project later shifted toward a keypad-based fortune / diary device with a rewriting trigger.

---

## Huaqiangbei
I went to Huaqiangbei and saw many phone repair and phone resale stores. A place that caught my attention was the Huaqiangbei Museum. It collects phones from around the 2000s (flip phones, feature phones, early mobile products). These phones are not used anymore, but their form factor and button-driven interaction are still impressive.

<img src="1.png" width="49%" />
<img src="2.png" width="49%" />

<img src="3.png" width="49%" />
<img src="9.png" width="49%" />

<!-- 4–8 in one row -->
<div>
  <img src="4.png" width="19%" />
  <img src="5.png" width="19%" />
  <img src="6.png" width="19%" />
  <img src="7.png" width="19%" />
  <img src="8.png" width="19%" />
</div>

---

## Reference: Mirai Nikki (Future Diary)
This reminded me of the anime *Mirai Nikki (Future Diary)*. In the story, the protagonist receives a phone that gets messages about future events. The messages arrive irregularly.

<img src="10.png" width="70%" />

---

## Prototype V0: GPS + time → “future diary” messages
I started with a simple pipeline:
- Input: GPS location + current time
- Send to an LLM API
- Output: future diary messages shown on the screen

However, the “future” was not accurate. It often felt like random generation. That made me rethink the direction.

<img src="11.png" width="49%" />
<img src="12.png" width="49%" />

---

## Interaction: keypad functions (fortune / oracle mode)
I added a keypad and mapped keys to different functions. This made the device more interactive and less dependent on “accurate future prediction”.

Current mapping:
- Press **1**: today’s luck + lucky color  
- Press **3**: warning / things to watch out for today  
- Press **4**: summarize previous future diary entries  
- Press **6**: tomorrow’s possible events  

<img src="13.png" width="49%" />
<img src="14.png" width="49%" />

<img src="15.png" width="49%" />
<img src="16.png" width="49%" />

---

## Rewriting: future changes when movement changes
I added a rewriting feature:
- If travel distance changes a lot, the diary result should update (the “future” is rewritten).
- This is a rule-based trigger for now.

<img src="17.png" width="49%" />
<img src="18.png" width="49%" />

---

## Voice interaction (attempt)
I also tried to add voice interaction, but it did not work reliably in this iteration. I plan to solve it later.

<img src="19.png" width="49%" />
<img src="20.png" width="49%" />

---

## Next step
Next I will focus on:
- the physical form factor (retro-future look)
- what kinds of inputs could make the “future diary” more meaningful (without turning it into surveillance)
