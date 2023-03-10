# 拆解和重新编程网络密钥

> 原文：<https://hackaday.com/2012/10/02/disassembling-and-reprogramming-webkeys/>

![](img/965e3f50a802d0665a453c856da7b9b3.png "Webkey frontbackcloseup")

网络钥匙是一种小巧、廉价的 USB 设备，当它插入电脑时可以启动网络浏览器。它们是作为促销品分发的，但是破解起来也很有趣。[Brad antonewicz]最近得到了一个，并决定打开它，看看他能完成什么。

该设备的大部分是包装，但他并没有花很长时间来得到这里看到的内脏。上图中显示了两个单元，这样我们可以看到电路板的两面。如您所见，有一个片上处理器(黑色斑点)处理 USB 连接。但是输入计算机的数据存储在顶部的 EEPROM 芯片中。它的腿渴望被探测。[Brad]无法找到确切的数据表，但他得到了一些关于引脚排列的线索。使用他的总线海盗，他能够建立通信和嗅探 i2c 流量。随着这一成功，他继续改写这一数据。休息之后你可以看到一个快速演示。

[Brad]希望在硬件方面做得更多。他认为这四个垫片可以用来重新编程微控制器。我们会密切关注他在任务中的进展。

[https://www.youtube.com/embed/XvRS7oHr62M?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/XvRS7oHr62M?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)