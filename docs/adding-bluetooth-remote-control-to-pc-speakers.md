# 为电脑扬声器添加蓝牙遥控器

> 原文：<https://hackaday.com/2013/03/30/adding-bluetooth-remote-control-to-pc-speakers/>

![adding-bluetooth-remote-control-to-pc-speakers](img/eeee8ae06016dc2c158fb70371715e3f.png)

普通的老式电脑扬声器已经不再普通了。他完成了一项相当复杂的黑客技术，现在[可以让他通过蓝牙](http://emerythacks.blogspot.com/2013/03/adding-bluetooth-remote-control-to.html)控制扬声器。

他有一套创意品牌的电脑扬声器，带有一个需要更换的音量电位计。他很难找到一个现成的替换零件，于是决定用一个旋转编码器。显然，你不能只放一个进去，他需要一个微控制器来监控编码器，并将变化转化为适当的电阻。他认为如果他要走这么远，还不如充分利用加州大学。

上面你可以看到他塞进原箱子里的所有东西。旋转编码器在左下方。一个 ATmega8 在他自己做的 PCB 上。左侧的白色部分是一个数字电位计，用于向原扬声器 PCB 提供电阻。左边是蓝牙模块，他可以通过手机控制一切。休息之后你可以看到一个演示。

[https://www.youtube.com/embed/z863gmc8VE0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/z863gmc8VE0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)