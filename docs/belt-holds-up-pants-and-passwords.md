# 安全带支撑裤子和密码

> 原文：<https://hackaday.com/2015/05/06/belt-holds-up-pants-and-passwords/>

[丹·威廉姆斯]做了一条腰带，它可以在记住你的密码的同时把你的裤子系起来。这是他上周末在 2015 年 TC Disrupt 黑客马拉松的 Hackaday 硬件村露营时的项目。

这个想法始于携带复杂密码的专用设备的概念；一些你自己都不记得并且很难打字的东西。[丹]还决定，如果设备不需要自己的电源，如果用户界面非常简单，那会好得多。答案是由一根 USB 电缆和一个只有一个按钮的微控制器组成的腕带。

在右边你可以看到原型的内部。他使用的是 Teensy 2.0 板，能够作为 HID 键盘枚举。唯一的用户输入是顶部的按钮。按下它一次，它就发出存储的密码。是的，实现起来非常简单，但是编程只是竞赛的一部分。他剩下的时间都花在了把它提炼成一种可以合理地被认为是产品的东西上。他在这方面做得非常好，以至于他收到了 Hackaday 的荣誉奖，以表彰他在构建中的表现。

## 制造

![IMG_20150502_183207](img/83994683f0c22c0a6bb5aa017ee5faa2.png)[Dan]想出了为 Teensy 2.0 设计一对交配板的主意。顶部有一个按钮，底部有一个 USB 端口，用作皮带扣的“扣子”。USB 电缆的一端插入 Teensy，另一端插入这个虚拟端口。早期测试表明，这太笨重，不能作为手环使用。但是[丹]只是简单地转动了一下，就把它变成了一条皮带。

![safety-belt-built-at-hackathon-thumb](img/d49bd4457932caf00be5466a82dd137f.png)[Kenji Larsen]帮[Dan]做 PCB 三明治。他们没有在额外的板上安装引脚插座，而是加热了几个细小引脚上的焊点，并用钳子将它们夹住。这样就留下了几个引脚，可以将按钮附加板焊接到这些引脚上。

为了完成制作，[Dan]与[Chris Gammell]合作，为电子设备制作了一个由两部分组成的外壳。他还想出了一个迎合皮带扣，也是一个按钮帽。它是 3D 打印的，带有略微凹陷的 TechCrunch 徽标。然后，他用蓝色油漆工的胶带填满这个空隙，形成一个很好的对比。

[丹]台上演示展示了高水准的提炼。没有一根电线(不包括 USB 带电缆)或未完成的部分显示！由于他在现场演示期间没有深入了解该构建的实质内容，我们确保在之后找到他，并记录下下面嵌入的硬件演示。

[https://www.youtube.com/embed/N_XkreOEB8c?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/N_XkreOEB8c?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

* * *

#### 2015 年[黑客日奖](http://hackaday.io/prize)由以下机构赞助:

[![](img/8e6c49d55ea91b307d7d191b75ab18c8.png)](http://hackaday.io/atmel)[![](img/6b53a13e67e0346985e237ef126c1bcc.png)](http://hackaday.io/freescale)[![](img/3fe105965ef22414d89f71032d9babee.png)](http://hackaday.io/microchip)[![](img/ebcbe4e97993de26ebcf849e70523a14.png)](http://hackaday.io/mouser)[![](img/15f4f8aaed16b020832d8be6282e47f5.png)](http://hackaday.io/ti)