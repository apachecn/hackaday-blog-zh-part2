# Hackaday 奖决赛选手:一台无噪音分光计

> 原文：<https://hackaday.com/2014/11/10/hackaday-prize-finalist-an-un-noodly-spectrometer/>

所以我们来到了 Hackaday 奖的最终入围者简历。再过三天，我们就能知道[【fl @ C @】的 RamanPi 光谱仪](http://hackaday.io/project/1279-ramanpi-raman-spectrometer)或者进入决赛的[其他四个项目之一](http://hackaday.com/2014/10/13/announcing-the-five-finalists-for-the-hackaday-prize/)是否会进入太空，或者只有日本。

管间有数量惊人的分光计项目，但大多数这些设置只测量吸收光谱——字面意思是被测物质吸收的光的波长。拉曼光谱仪完全不同，它使用激光照射样品，测量材料的光散射。这项工作获得了诺贝尔奖，[fl@C@]用 3D 打印机做了一个。

下面是我的简历，以及发给评委的最终视频。如果你想知道谁是黑客日奖的得主，连我都不知道。[迈克]和几个黑客霸主知道，但我们其余的人将保持无知，直到我们在下周四在慕尼黑举行的派对上宣布获胜者。

[https://www.youtube.com/embed/BH2BKBWdsYo?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/BH2BKBWdsYo?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

```
What was the ultimate inspiration to create a Raman spectrometer? 
You say you needed to do spectroscopy for another project, but
why did you  choose Raman spectroscopy? There are several other
photoemissive spectroscopy projects out there. Is it just an
issue of being able to scan everything, or just wanting to a
project for the hackaday prize that replicated work that won a
Nobel prize, or something else?
```

我已经为我的大项目工作了大约 5 年了..不幸的是，这不是一个开源项目，也许有一天..因此，在不涉及太多细节的情况下，我需要确定一种前后方案中的键角和拉曼位移，因为这将表明我在测试时是否在正确的路径上。这自然让我想到了拉曼光谱仪..我没有资金买一辆二手的，更大的项目就靠它了。我没有见过任何其他项目提供这种类型的信息，所以我只是决定建立它。没有什么比复制任何获得诺贝尔奖的作品更迷人的了。:)

```
You're building complex optical paths with a 3D printer, and 3D
printing is obviously a 'good enough' solution for building a
prototype. Given unlimited funds we know you wouldn't be using a
DaVinci printer, but would you still use filament-based 3D
printers if you were to do this all over again? What problems did
you encounter in printing the spectrometer?
```

用 3D 打印零件建造它似乎是一种快速而廉价的建造方式。当比赛开始时，分享计划并使其更容易建造的想法更加受到关注。保持 3D 打印零件似乎是一种非常合理的方式，使人们更容易建造，因为越来越多的人可以使用 3D 打印机，而不是其他方法。所以，我想再来一次，我还是会保留 3D 打印的零件。这似乎是最好的中间地带，给那些想为自己建造一个的人最大的可用性。

![1867341411967375105](img/b1ab1064d3b6d1ac334c896da991497a.png)

3D Printed optical paths

话虽如此，考虑到“无限的资金”……我可能会选择用铝来加工零件，或者可能用一些不太贵的材料，如尼龙或 HDPE(虽然不确定 HDPE 与铝的价格/磅相比如何)。我在打印中遇到的最大问题是 ABS 收缩的补偿，明显的打印机问题，以及如何处理无数有小错误的作品。收缩花了一点时间才掌握。这是我第一个使用 3D 打印机的实际项目。

```
Keeping a local database of spectrometry is insane, and in your
documents you say you're using online spectrometry databases. Is
there an issue in getting the data from these databases into a
coherent format, and what does the future of these proprietary
databases look like, given that the RamanPi will eventually be
released into the wild?
```

以一致的格式从在线数据库获取数据并不是一个真正的问题。我相信大多数都是逗号分隔的格式，或者类似的格式。我认为大部分数据库都是由大公司维护的，这些大公司对访问数据收费。这是我认为最大的问题。有几个是免费的，我已经从他们那里得到了访问数据的许可，只要它不是完整下载的。保持一个本地数据库有点疯狂，这将是一个全职工作，仅仅是从你能找到的任何材料中编目所有的光谱。很高兴看到未来是一种点对点的数据库，人们共享他们的数据，并为之做出贡献，就像光谱的 Napster 一样！

```
Have you given any thought to the commercialization of your
project? How much are you looking at to turn this into a product
(if you even can), and from the responses, what do you think a
product based on the RamanPi would cost?
```

最初，我没有考虑商业化。我只是为自己建造的。然后，比赛开始后，人们开始感兴趣，问我是否打算出售工具包等。我想提供几个版本。我想要一个低端版本，有不太贵的光学系统和一个 Raspberry Pi 相机模块，一个中间版本，有不太贵的光学系统和一个 CCD..还有一个更贵的版本，配有良好的光学系统和 CCD。我还想提供没有拉曼系统的光谱仪，作为普通的 CCD 光谱仪使用。至于成本，我认为低端应该在 300 美元左右，中端在 500 美元左右，高端在 700-800 美元左右。分光计本身是最昂贵的部分，可能要 350 美元左右。

```
Hypothetical, and we’re not going to hold you to whatever answer
you give. You win the grand prize, a trip to space or about
$200,000 USD. Which one to you take, and what is your reasoning
for doing so?
```

所以，我想了很久…如果我足够幸运，必须在空间和金钱之间做出选择…我最初说的是空间，毫无疑问。对我来说这是板上钉钉的事。

我认为在看了旅行的选择后，这种情况发生了变化，而且是在最近的事故之前。我只是不相信维珍银河的选择。我完全支持自动化，让飞行员不再犯错。作为一名飞行员，我知道这可能是一个因素。

![fly0811_rutan7](img/059b6d6ce2c0d191979c6c0826a77ab7.png)

A normal-looking Rutan design. Not shown: variable geometry sideburns

我也从来不是鲁坦作品的超级粉丝。我不关心其他人，因为我没有看到这些数字..毕竟这是我的生活。对我来说，乘坐圣母 SS2 以 3.5 马赫的速度旅行的想法听起来比太空更有趣。但是在这一点上…我不得不诚实地说现金选择。将这些钱投资到我更大的项目中可能会为以后的旅行买单。