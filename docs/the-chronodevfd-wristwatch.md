# ChronodeVFD 腕表

> 原文：<https://hackaday.com/2014/10/26/the-chronodevfd-wristwatch/>

不仅仅是另一个蒸汽朋克时尚宣言，[John gineer]ChronodeVFD 腕表既精致又美丽。当然，我们已经看到了我们的 VFD 产品(如果你想要一个真空荧光显示器的速成班，可以看看 [Fran 今年早些时候的视频](http://hackaday.com/2014/01/04/frans-leds-nixies-and-vfds/))但是我们很少看到它们是便携式计时器，更不用说如此引人注目的了。

ChronodeVFD 使用 IVL2-7/5 显示管，除了体积小、电流低之外，它还是扁平的，而不是圆形的，并且具有透明背衬。[Johngineer]基于一个 AtMega88 和一个 [Maxim DS3231 RTC](http://www.maximintegrated.com/en/products/digital/real-time-clocks/DS3231.html) (实时时钟)制作了一个定制板:他承认后者有点贵，但没有人抱怨剩余部分简化了你的设计。

VFD 采用 Maxim MAX6920 12 位移位寄存器，由一节碱性 AA 电池供电。可充电的镍氢电池会更好，但较低的标称电压意味着升压转换器的效率较低，VFD 的电流较小。[Johngineer]的寿命不会超过 6-10 个小时，但最终 ChronodeVFD 是一件不适合日常穿着的服装。浏览他的博客，获取一些高分辨率的照片，以及关于他如何建造铜管“防滚架”外壳以及皮革表带支架的更多细节。