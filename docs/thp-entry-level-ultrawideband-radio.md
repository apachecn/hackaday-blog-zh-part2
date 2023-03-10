# THP 半决赛:级别，超宽带无线电模块

> 原文：<https://hackaday.com/2014/08/29/thp-entry-level-ultrawideband-radio/>

![LEVEL](img/1e4a89bcdff489b06be6cd7a6d786188.png)

当你开始研究物联网时，你首先意识到的是，尽管有互联网连接一切的宏伟构想，但没有人知道这些东西将如何实际连接到互联网。有数百种不同的无线电协议正在推广，目前有几十种网络方案正在开发中。这个问题的解决方案是一个无线电模块，它可以完成所有这些工作，与所有这些模块进行对话，并向互联网提供服务。这是[【亨特·斯科特】的 Level](http://hackaday.io/project/1594-level%3A-An-Ultrawide-band-Radio-Module) 的想法，一个无线电模块，频率范围是 30 MHz 到 4.4 GHz。这将涵盖几乎所有内容，包括电视空白领域的一些有趣应用。

[Hunter]的模块基于 TI 的 CC430，基本上是一个 MSP430 微控制器和一个 [CC1101 收发器](http://www.ti.com/product/cc1101)组装在一块硅片上。有一点过滤，使其在现在有点空的电视空白频谱中可用，这是许多物联网和无线网络协议正在考虑的事情。

如果设备的外形看起来很熟悉，那是因为它是；该板本身与 Arduino 兼容，但与 Arduino 本身不兼容；不过，它将接受*屏蔽*，这意味着建立一个到以太网或 WiFi 的桥梁，连接到该板正在与之对话的任何无线电设备，这实际上只是固件的一个变化。

该板非常适合试验不同的无线电模块，但也非常适合试验不同的无线电协议。[Hunter]一直在研究不同的网状网络协议。

您可以查看[Hunter]的两分钟视频概述，以及下面示意图的更详细概述。

* * *

![SpaceWrencher](img/4892437613088ab3882681a2ec04a2bb.png) **本帖介绍的项目是[入围 Hackaday 奖的半决赛。](http://hackaday.io/list/2864-The-Hackaday-Prize%3A-Semifinalists)**

[https://www.youtube.com/embed/9vLNtCqOhVs?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/9vLNtCqOhVs?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)
[https://www.youtube.com/embed/FLb11qhgQl8?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/FLb11qhgQl8?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)