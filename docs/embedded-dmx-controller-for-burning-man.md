# 燃烧人的嵌入式 DMX 控制器

> 原文：<https://hackaday.com/2013/07/19/embedded-dmx-controller-for-burning-man/>

![embedded-dmx-controller](img/55ae44eb4fa5f892dabdae4e66312f06.png)

这是为火人族打造的灯光控制器【Paul Stoffregen】。他们今年想用 DMX 控制的灯光，但通常包括一台电脑来运行灯光序列。这个板[使用一个被破解的照明设计文件](http://www.dorkbotpdx.org/blog/paul/dmx_lighting_sequence_player)运行预编程的 DMX 序列。

灯光的编排是用一个叫做 Vixen 2 的程序设计出来的。该软件有一个较新的版本，但[Paul]需要翻译输出文件以用于微控制器，版本 2 比版本 3 更容易一些。说到转换，他不想从头开始，一点搜索就引出了[比尔·波特]去年发布的关于转换 Vixen 文件以用于 Arduino 的教程。这并不完全符合他的想法，但大部分的基础工作都在那里。

几处代码调整使剧本符合了(保罗的)意愿。他修改了 XML 解析函数，忽略了文件中除主通道以外的所有通道。他还让它输出一个可以存储在 SD 卡上的文本文件。因为输出没有被闪存到芯片中，这大大增加了可用的存储空间，为更长更复杂的显示铺平了道路。

想进一步了解 DMX 设备使用的协议吗？[看看这个引物](http://hackaday.com/2011/11/01/looking-toward-christmas-decor-by-learning-about-dmx/)。