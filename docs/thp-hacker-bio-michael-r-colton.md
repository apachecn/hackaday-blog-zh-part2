# THP 黑客传记:迈克尔·R·科尔顿

> 原文：<https://hackaday.com/2014/09/07/thp-hacker-bio-michael-r-colton/>

随着许多黑客意识到连接到计算机的几个 RF 模块可以做多少事情，软件定义无线电进入 Hackaday 奖的半决赛也就不足为奇了。[迈克尔]的项目是 [PortableSDR](http://hackaday.io/project/1538-PortableSDR) ，这是一个小型的独立装置，可以处理 30MHz 以下的一切。不，[迈克尔]不是在处理用更好的 SDR 可以达到的千兆赫，但这不是重点:PortableSDR 是为了做*所有的事情——*矢量分析，一个整洁的瀑布显示，传输和接收——在一个小的，便携式的包里，你可以带去任何地方。它的构建也相当便宜，当然完全开源。

这不是[迈克尔]的第一次竞技表演；他以前做过很多同样酷的项目。他发来了一份简短的简历，如下所示。

就一个？显然，无线电和电子是大的。如果这能告诉你什么的话，Hackaday 是我最喜欢的网站。

我喜欢各种户外活动，背包旅行、攀岩，最近还喜欢滑翔伞。

多年来，我一直对亚洲文化和语言感兴趣。我在高中和大学学过日语，我在台湾当了两年传教士，在那里我学会了普通话。

![](img/b36bf05c59a5770a2c567b59107c46e0.png)

I wanted to be an inventor as a kid (now I’m actually a little skeptical of people who call themselves that). I took things apart, ruined lots of VCRs, electrocuted myself a bunch of times, even knocked myself out once. My dad says when I was three or four I broke the side view mirror off his sports car and he couldn’t figure out how. I played with electronics, shopped at Radio Shack, bought a BASIC stamp kit (for like $100! Seriously?) and played with that a little, but in college I wasn’t confident I’d ever really understand electronics, so I got my education in psychology instead. But I continued to play, found out how cheap AVRs and PICs are and moved up to those.I was lucky to make friends with a guy who worked for an aerial data collection company (before it was cool) who wanted to split of and use “multi-rotors” for aerial video. I knew a little about electronics so I helped him and together we started [Utah Aerials](http://www.utahaerials.com/). I started making [my own aircraft](https://www.kickstarter.com/projects/1703258614/maxrotor-open-source-plug-and-play-modular-quadcop), and eventually met with a start-up engineering firm about producing them. The boss was impressed and hired me.That was about three years ago, now I work as a product designer and electrical engineer at RPH Engineering, spending most of my time doing circuit design and firmware, but I get to do concept art and mechanical design from time to time. I’m lucky to have a job where I get to work on lots of interesting projects. I feel very blessed that I was hired, as I don’t have a degree in any of this, and only had light experience at the time (It didn’t hurt that my boss didn’t have to pay me very much).I hope that might be inspiring to some people out there. I didn’t go to school for this, and for years I thought I’d never understand any of it well enough to make the things I wanted to make. I just followed what was interesting to me and kept learning. To those that are overwhelmed with how much there is to know, hang in there. I still have so much to learn, but when it starts to click, it’s a pretty amazing feeling.

除了我的妻子，我可能会学习、制作和体验新事物。在我能建造东西之前，我会画很多，我会创造只存在于纸上的人、地方和东西。

打印机是一个很好的选择。也许是一般的电脑。有时候我希望软件是一个可以被砸碎的东西…唉。

我小时候是一个死忠的 Mac 用户，我仍然认为它设计得非常好，非常有用，但我想做的几乎所有事情都需要 Windows(请安装 Windows 7 或 Server editions ),所以这是我最常使用的。我到处玩 Linux，我喜欢它能做的事情，但还没有真正适应它，一切似乎都需要这么多工作。

![](img/86cb90b2c0b6af0a653ce112a7f83607.png)示波器。刚拿起一个 Rigol DS1074Z 就爱不释手(获取信号 gen，值得！)也就是说，如果 Tektronics 想赞助我，我很乐意接受 MDO3/4000。

此外，目前有限的长凳供应已经节省了我的培根很多次…..还有助焊剂笔。如果你能转动它，一个双目显微镜，我不知道没有它我是怎么生活的。

我非常喜欢 STM32 微控制器。PortableSDR 里的 F4 是一只野兽！180Mhz，FPU，大量的内存，以及你想要的每一种外设。它们也很灵活。在 AVR-Arduino/PICs 上，您的 GPIO 是数字或模拟的，有时您有一个内置的上拉电阻。STM32s(我想很多也适用于其他 arm)具有上拉和下拉、开漏，每个 GPIO 有不同的驱动电平。它内置了 DAC 等。我曾经用 AVR 做一些事情，我打算用 TTL 串行，但它是反相的，所以我必须添加一些电路来翻转它，不需要在 STM32s 上它有内置的能力。

![](img/308a7648f6e9856896236bbb41dc80a5.png) C .(也是 C++/C#/Java)没什么真正的原因，这只是我所知道的和感到舒服的(并不是说我特别擅长其中任何一个)也运行在任何东西上！

我有一个秘密的(我知道没什么用。)我希望在某个时候 Kickstart。我正在连接家庭安全/家庭自动化系统，该系统包括恒温器控制和功耗测量。不过，最酷的部分是它使用了传送门炮塔的声音(打开一扇门，你会听到，“喂？谁在那里？”走到运动传感器前面，然后说，“你在这里！”)

我想做一个动力伞(电动偶)或者尝试做一个超高效的电动汽车(我觉得是带空气动力学整流罩的反向三轮车)。

Electrostatic headphone drivers and amplifier.That was three right? And really, that’s just want I’d like to do in the next few years. Sometimes I wish I would get fired so I had time to work on all this stuff!

![](img/b695bbab69a146f980245f1ec391f5f7.png)自从几年前我第一次听说软件定义无线电(特别是[这篇文章](https://www.arrl.org/files/file/Technology/tis/info/pdf/020708qex013.pdf))以来，我就对它很感兴趣，并想建立自己的软件定义无线电。随着我对电子尤其是微控制器的了解越来越多，我认为我可以将 SDR 与我对户外的兴趣结合起来。

很多东西！下面是几个:对于 DSP 的家伙，我如何建立一个任意滤波器的 FFT 卷积与已知的内核长度？虽然我已经填充了样本，但我现在做的方式似乎是在绕圈子。我可能犯了很多错误… RF 伙计们，我喜欢设计一个有效的 RF 放大器，以达到 1-5 wh 范围，这是小的，可以运行 3 伏。对于输入莫尔斯电码的火腿，你用哪只手，你把钥匙放在什么角度，我想是 45 度？尝试过电容键盘，你觉得怎么样？在 Hackaday 社区中有大量的脑力，所以我希望人们能加入 PortableSDR 并帮助我把它做得更好。我期待(希望是建设性的)反馈！

![Cut](img/48f76dfe842c64dd697fabb5010d0e7a.png)几个。我认为 GPS 时钟非常精致。我不介意给自己造一个。还有微波失落的 PLA 项目？！混合摩托艇，我要一辆。纸板气垫船。仅举几个例子。我喜欢的几个项目*都进了半决赛。*

 *![Project](img/b3d287ff71123bed7640665e599679f6.png)

Things are progressing very well. My main problem is time. We’ve got less than a month until the next round of judging, but it takes about a week to have a PCB produced and another week to have it shipped (if you are cheap/poor) so that’s half of the available time gone right there! And I haven’t even finished designing the next revision yet… I want to source some LCDs from China and I am having the same problem shipping times.There is a lot I am learning as I go, so some things take longer than expected or don’t work right at first. But that’s part of why I wanted to do this. It’s amazing how much I’m learning. It’s really stretching my brain. It’s really fun.

我在比赛中获得了很多乐趣，看到其他人想出的所有很酷的东西让我很受鼓舞。此外，我真的很感激在我参与这个项目的过程中，人们给予我的积极支持。一些人已经建立了自己的项目，有人甚至在 reddit 上发布了我的项目。谢谢大家！*