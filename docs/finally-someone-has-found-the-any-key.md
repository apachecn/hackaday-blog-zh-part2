# 终于，有人找到了钥匙

> 原文：<https://hackaday.com/2014/06/13/finally-someone-has-found-the-any-key/>

![keyboard and any key device](img/9343ca4893982373a351d49988466ed4.png)

“任何钥匙在哪里？”嗯，就是这里的。在 STM 平台遇到麻烦后，[lukasz.iwaszkiewicz]使用德州仪器 C 系列 Launchpad 构建了他的“任意键”HID 设备。他能够利用 [TI TM4C123G LaunchPad 的](http://www.ti.com/tool/ek-tm4c123gxl)扩展 USB 库，该库分为四层——最顶层是设备类 API。这使得程序员能够只用几行代码实现简单的设备。[lukasz.iwaszkiewicz]指出，ST 没有这个选项。

Any 键使用主机 PC 程序，允许用户在虚拟键盘上输入击键。该信息然后被传递到任何密钥设备。当它被按下时，它将把记录的击键推回到主机 PC。简单，但是有效！

该项目是完全开源的，所有文件和代码都是可用的。请务必在休息后观看演示任意键运行的视频。

[https://www.youtube.com/embed/CeLo8d0pDmI?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/CeLo8d0pDmI?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)