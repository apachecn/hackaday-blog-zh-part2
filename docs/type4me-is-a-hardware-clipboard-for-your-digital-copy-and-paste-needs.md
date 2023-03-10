# Type4me 是一款硬件剪贴板，可满足您的数字复制和粘贴需求

> 原文：<https://hackaday.com/2013/01/14/type4me-is-a-hardware-clipboard-for-your-digital-copy-and-paste-needs/>

![type4me-hardware-clipboard](img/49d65028c18a72882658b197c2e123b2.png)

这并不经常发生，但我们不时会发现自己想要一个更具可扩展性的剪切和粘贴体验。最值得注意的是，我们搜索了一些东西，使得*非常容易*在剪贴板中保存多个东西，并在需要时粘贴它们。虽然我们已经尝试了几个软件产品，但没有一个真正符合标准，但是[这个硬件剪贴板看起来很有前途](http://www.lucadentella.it/en/2013/01/14/type4me/)。[Luca Dentella]称它为 Type4me，因为它的功能是 USB 键盘。

PIC 18F14K50 枚举为 USB 键盘，允许它将字符发送到光标所在的任何位置。它发送存储在里面的任何字符串，在末尾有一个可选的返回字符。除了它的键盘属性之外，它还建立了一个串行连接，允许你将新的字符串推送到设备。这种设置确实需要您将字符串复制或输入到串行终端，以及微控制器解析的四个特殊命令之一。其中一个命令允许您将字符串保存到 EEPROM，以便它在整个上电周期中保持不变。

粘贴回计算机只需按一下按钮。休息之后我们嵌入了视频演示。它是意大利语的，但是有英语字幕。在快结束的时候,[Luca]展示了这款作为游戏宏按钮的设备。

[https://www.youtube.com/embed/36fenYwEfBI?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/36fenYwEfBI?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)