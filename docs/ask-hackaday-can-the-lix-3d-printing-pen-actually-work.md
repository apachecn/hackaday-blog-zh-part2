# 问 hack aday:Lix 3D 打印笔实际能用吗？

> 原文：<https://hackaday.com/2014/05/03/ask-hackaday-can-the-lix-3d-printing-pen-actually-work/>

[介绍 Lix](https://www.kickstarter.com/projects/lix3d/lix-the-smallest-3d-printing-pen-in-the-world) ，世界上最小的 3D 打印笔，可以让你用 3D 绘制塑料结构。它在 Kickstarter 上发布才几天，就已经获得了近百万美元的认捐。这是一个惊人的成就，尤其是考虑到我们可以用数学和物理证明它并不像宣传的那样有效。然而，我们想知道它是否能在*工作*，所以我们询问 Hackaday 社区。

该设备通过 USB 3 端口供电。在视频中，Lix 团队正在使用一台 MacBook Pro。这有一个 USB 端口[能够在 5 伏、](http://support.apple.com/kb/ht4049)[或 4.5 瓦](#footnote1)下传输 900 毫安。另一种 3D 打印笔， [3Doodler](http://hackaday.com/2013/02/20/3doodler-a-3d-drawing-pen/) ，使用 2A 12V 电源适配器，相当于 24 瓦。考虑到 3Doodler *的工作方式*，并且它们都做相同的基本事情，这里发生了一些*极其奇怪的事情*。

作为比较，[这里有一个绕线电阻](https://ultimachine.com/content/68-ohm-3w-5-resistor)，通常在 3D 打印机的加热元件或“热端”中发现。这是一个 6.8 欧姆的电阻，电压为 12 伏。那是 21 瓦。[这里有一个加热器筒](http://www.dx.com/p/12v-40w-ceramic-cartridge-heater-for-reprap-3d-printer-red-silver-198825#.U2GiivldXTo)，在很多热端也能找到。它消耗 40 瓦。Lix Kickstarter 再次清楚地显示了这只笔仅使用 4.5 瓦的功率挤出细丝。这里真的很可疑。

直觉和数学不可同日而语，所以让我们弄清楚它为什么行不通。

![The computer used in the Lix promo video. If that isn't an Apple device, I will buy a hat and film myself eating it.](img/aa8715fd54ccf4dfc588b9eafcadfd83.png)

The computer and USB port used in the Lix promo video. If that isn’t an Apple device that can only supply 900mA at 5 V,  I will buy a hat and film myself eating it.

我们认为，计算 4.5 瓦是否足以用于 3D 打印笔的最简单方法是从纯粹的热力学分析中得出:特定量的细丝进入，加热到熔点，然后从喷嘴中挤出。计算系统中特定温度变化需要多少能量的方程式是*Q = cmδT*，其中 Q 是以焦耳为单位的能量，c 是 ABS 的比热(1.3j/g·K，[来源](//www.matbase.com/material-categories/natural-and-synthetic-polymers/commodity-polymers/material-properties-of-acrylonitrile-butadiene-styrene-general-purpose-gp-abs.html#properties))，m 是以克为单位的质量，δT 是温度的变化。我们现在要做的就是计算出这支笔挤出的速度，以及挤出细丝的质量。

[在这个视频](https://www.youtube.com/watch?v=Hd-H_7IZZd8)中，从 10 秒开始，你看到 Lix 在 5 秒钟内通过 Lix 附带的 0.6 毫米喷嘴挤出约 13 厘米的细丝。稍微算一下(高 13 厘米，直径 0.06 厘米的圆柱体的体积)，我们可以算出 Lix 每秒挤出 0.038 克细丝(ABS 密度为 1.04 克/立方厘米，[来源](http://teststandard.com/data_sheets/ABS_Data_sheet.pdf))。这种计算是通过计算像素和帧数来完成的，可能会不准确，但不会太多。

估计每秒钟挤出 0.038 克细丝，210°C 的温度变化(20°C 室温，230°C 挤出温度)，以及 1.3J/g°C 的 ABS 比热([来源](//www.matbase.com/material-categories/natural-and-synthetic-polymers/commodity-polymers/material-properties-of-acrylonitrile-butadiene-styrene-general-purpose-gp-abs.html#properties))意味着从 Lix 笔中挤出一秒钟的细丝需要 10 焦耳。由于 1 瓦= 1 焦耳持续 1 秒，每当 Lix 挤出灯丝时，约有 10 瓦被吸走。同样，Lix 只能从 USB 3 端口获得 4.5 瓦的功率。数学根本不起作用，没有 USB 3 供电的设备可以挤出 ABS 丝那么快。数学也是很慷慨的，因为它没有考虑灯丝的相变，这需要更多的能量。我没有包括这个，因为我找不到 ABS 的熔化热的参考。该数学也没有考虑到加热器部件、空气和任何真实世界设备中的许多其他低效率的损失。

但是 ABS 需要相当高的温度来挤出。尽管 Lix 团队声称这种笔可以与 ABS 一起工作，但假设他们使用的是 PLA 塑料，在 180°C 下挤出。计算 160°C 的δT 意味着从 USB 3 端口吸收 7.9 瓦，而 USB 3 端口只能提供 4.5 瓦。这里出了很大的问题。这就是我们向您求助并询问 Hackaday 社区其他成员的原因。

我们能确定 Lix 实际工作的唯一方法是挤压速度非常非常慢。将 PLA 的挤压速率减半至 1.3 毫米/秒，让我们大致了解 Lix 电源能做些什么；这只需要大约 4 瓦特，剩下的足够运行笔内的电机和电子设备。这对于任何塑料挤出机来说都非常慢——reprap 挤出塑料的速度可以快 50 到 100 倍。有很好的证据表明 Lix 的视频速度明显加快了，鉴于免责声明，“一些视频场景的速度加快了”在活动的第一天和第二天之间的某个时候出现在 Kickstarter 上。

虽然我们知道该视频完全歪曲了任何 USB 3 供电设备的功能，但我们无法确定 Lix 是否是一款可行的产品。我们转向你。你能弄清楚 Lix 笔是否真的能用吗？我们只知道 Lix pen 有一个 USB 3 端口的 4.5 瓦电源。USB 3 驱动的 3D 打印笔有可能工作，尽管很慢，但工程很困难，我们不知道 Lix 团队是否有能力。

* * *

* For the hardware heads out there, *yes*, I know there is a USB 3 spec  – [the USB Power Delivery Specification](http://www.usb.org/developers/docs/) – out there that will supply up to 100 Watts through a USB port. Apple does not support this spec in any of their products, and the Lix Kickstarter video uses a MacBook Pro for power. The maximum amount of current the Lix can draw from a MacBook is 900mA, and the Lix has a power budget of 4.5 Watts. There really is no arguing that fact.

> 作为题外话，这篇文章启发我们考虑一个关于 Kickstarters 的专栏，它似乎违背了物理定律。我们正在考虑将其命名为 Kickherder，因为这类项目的大多数 Kickstarter 支持者都是无脑羊。如果你有更好的名字，请在评论中留下。