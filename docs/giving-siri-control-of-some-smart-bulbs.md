# 让 Siri 控制一些智能灯泡

> 原文：<https://hackaday.com/2012/11/21/giving-siri-control-of-some-smart-bulbs/>

![](img/0ad08270b86dcf39df727cef9ca8a3d3.png "giving-siri-control-of-smart-bulbs")

[Brandon Evans]拿到飞利浦 Hue 智能灯泡后，打开了一些硬件，看看里面是什么。他还花时间研究出必要的软件技巧，以便在 iOS 系统中使用 Siri 来控制灯泡。

如果你以前没有听说过 Hue 产品，它是一种适合标准介质底座的 LED 灯泡，其颜色和强度可以无线控制。每个单元都包括 Zigbee 兼容硬件，让灯泡形成自己的网状网络。[Brandon]没有打开灯泡，因为这些东西成本很高，拆卸需要切割。但是他确实给我们指出了这个帖子，在这个帖子里[Michael Herf] [展示了灯泡的盒子里藏着什么](https://plus.google.com/photos/107696725527584609973/albums/5806291983792940817)。当[Brandon]揭示了通过以太网将网状网络连接到家庭网络的基本单元的内部结构时，我们确实看到了这个难题的另一部分。STM32 芯片负责控制基本单元。

除了看看胆量[布兰登]黑了 Siri(苹果的语音激活虚拟助手)来控制系统。休息过后，你可以在视频中看到演示。细节可以在他文章的后半部分找到，链接在顶部。代码在他的 siriproxy-hue 库中找到。

[https://player.vimeo.com/video/53788941](https://player.vimeo.com/video/53788941)