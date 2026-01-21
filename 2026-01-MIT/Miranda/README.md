> **If you're a future Research @ Scale resident reading this, scroll to the bottom to see my pro-est pro tips for navigating life in Shenzhen -- I had to do a lot of logistical learning and I'd like to save you, dear reader, the trouble of figuring out the things I figured out along the way!**

Here's what I worked on during my month in Shenzhen, as a part of the Research @ Scale residency.
I am so incredibly grateful to all of the sponsors for giving me the opportunity to experience what has been truly one of best months of my life!
During the first hectic week I had a lot of fun attending the Scalable HCI conference, visiting factories / Huaqiangbei / the UABB Biennale / AIRS, and getting settled into my apartment at Boyu and the makerspace at Chaihuo. I spent the rest of my time in Shenzhen making a whimsical art robot called Labububot.

# Labububot
For more information, see [our Github repo](https://github.com/mirandali707/labububot).

## Abstract
==TODO TODO==
social robotics
humanoid robots, (made for function, made to look anthropomorphic)
cute baby schema robots (made to look cute, made to deceive user into trust)
many other robot mechanisms exist: snake robots, soft robots, etc. -- but social robots are largely either humanoid or extremely cute

inspired by BALLU, balloon robot -- anthropomorphic enough (legs) to evoke a strong emotional reaction, while not being overly anthro (eg humanoid, has face that emotes)

how can we subvert traditional social robot aesthetics by using non-traditional materials and eliciting emotionally ambiguous responses?
instead of referencing animals and people (real life), what if we designed mythical creatures instead?
(we can make robots any shape we want. why have we chosen human? why not pokemon?)
[mythical many-headed creatures](https://en.wikipedia.org/wiki/Category:Mythical_many-headed_creatures)
show pokemon fotos

[Vox - The dopamine-driven secret to Labubu obsession](https://www.vox.com/culture/421637/labubu-doll-pop-mart-plush-obsession-shopping)
baby schema
mythology, folklore
Made in China
appropriating a uniform, scaled design (labubu) into a one-off, hand-crafted abomination
(digital craft - industrial design vs craft)

## BOM
* [Seeed Xiao ESP32](https://wiki.seeedstudio.com/xiao_esp32s3_getting_started/)
* [Sparkfun 6-DOF IMU](https://www.sparkfun.com/sparkfun-6dof-imu-breakout-lsm6dsv16x-qwiic.html)
* [Seeed Grove 16 channel PWM Driver](https://wiki.seeedstudio.com/Grove-16-Channel_PWM_Driver-PCA9685/)
* 12 servos
* 12 Labubus (decapitated)
* A lot of PETG filament and access to as many 3D printers as possible :^)

## Process
* IMU + browser controller tests
* digital twin
* assembly
* controls

## Future work
* labububot in the wild
* potential alt.HRI paper on speculative robot futures: social consequences of robots with no associations (not animal, not human...)

# Logistical advice for future generations
* Begin the VISA process as soon as you can! If you're a US citizen, the nearest Chinese embassy is in New York. The process I went through went like this:
1. Fill out the online form [here](https://consular.mfa.gov.cn/VISA/visa/visaform). I applied for a  L (tourist) visa valid for 120 months (10 years), max duration 90 days, multiple entry. Pro tip: it doesn't cost any extra money to max out the parameters like this on the tourist visa, so you may as well -- that way if you want to come back you won't have to go through this process again! Some people in the program applied for a student visa, using the invitation letter from SUSTech. It seems like either way is fine.
2. Check the status of your application -- it usually takes around 2 days before you are "invited" to bring your passport in (in-person!) to the embassy.
3. Drop off your passport at the NY embassy -- Ben and I went first thing in the morning and the line was very short. They will give you a slip -- DO NOT LOSE IT! Take a picture of it just in case.
4. Wait a few days (depending on if you've gotten express or normal service), then return to the embassy to collect your passport. Or, have someone you trust bring the slip to the embassy, and they can collect your passport for you! You don't have to collect it immediately when it is ready.
* If you're only staying in China you don't need an outlet converter; most outlets are also compatible with US-style plugs.
* You **must** download WeChat. WeChat can be used for everything from ordering at restaurants to calling cabs to messaging, and more.
* Set up WeChat Pay and AliPay before you arrive! Most places will take both.
* I used the [MIT VPN](https://ist.mit.edu/vpn) on my laptop, and got a [trip.com e-SIM](https://www.trip.com/things-to-do/detail/40017785/) which covers both China and Hong Kong (since my flight was out of HK). I'd highly recommend this, it comes with a VPN built in when you use the cellular data, so as long as you get enough data you don't need to fuss with an additional mobile VPN!
* China Mobile has a 2-month, **free** phone plan for getting a +86 phone number; all you need is a vessel for a physical SIM! If I had known, I would have done this as soon as I arrived in China.
	* I still had an e-SIM I was using for data, but having a Chinese phone number is super helpful for many things, including but not limited to creating a Taobao account ;)
* Google Maps doesn't work well, Apple Maps is alright, Amap is best.
* Dianping is the Chinese version of Yelp. I used this to find a salon to dye my hair at :)
* I haven't tried it, but I only recently found out that [hqew.com](https://www.hqew.com/) is a website where you can search for components and find them in the HQB markets. Might be helpful if you're trying to find something specific!
* Visiting Hong Kong is cheap and easy from Shenzhen - you can take high speed rail from Futian or Shenzhenbei to West Kowloon; it's about a 15min train ride and costs less than $20! You can book tickets through trip.com or klook.com, for example. I recommend arriving at the station an hour before your train, *especially on the way back from HK -> SZ* -- there are some airport-esque baggage and customs checks which will take some time! On the SZ -> HK route, the customs happen in West Kowloon after you arrive. **Make sure to bring an outlet converter -- HK uses UK plugs!**
* Calling cars is cheap and easy via Didi - I usually do this from within the WeChat mini-program. *When you get into the car, you will need to confirm the last 4 digits of your phone number with the driver.* If you don't speak Chinese I'd recommend having these written down so you can just show the driver instead.