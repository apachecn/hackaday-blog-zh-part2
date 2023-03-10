# 修复苹果电视糟糕的用户界面

> 原文：<https://hackaday.com/2014/04/14/fixing-apple-tvs-terrible-ui/>

![IR](img/86cd105e65c9d4c191e7f41be2777b92.png)

尽管苹果对用户界面做出了不懈的努力，但他们有时还是会设法推出一些讨厌的东西。其中最新的是苹果电视搜索界面的“键盘”。这是一个按字母顺序排列的键盘，放在一个正方形里，伴随着这个糟糕想法的是明显的挫败感。[Lasse]对这个设计感到失望，并意识到用 Apple TV IR 遥控器搜索任何东西都是一件痛苦的事情。他的解决方案是制作他自己版本的苹果电视遥控器，带有网络界面，由 Arduino 驱动。

受几年前我们推出的[苹果远程 Arduino Shield](http://hackaday.com/2009/11/03/apple-remote-arduino-shield/) 的启发，[Lasse]用以太网屏蔽将一个红外 LED 插入 Arduino 的引脚，让限流电阻见鬼去吧。web UI 是这个版本的创新部分。他在 Arduino 上托管了一个简单的网站，允许他用真正的键盘在网站上输入搜索查询，并让 Arduino 负责移动 Apple TV 光标来选择每个字母。

网络用户界面拥有苹果电视遥控器的所有功能，包括滑动手势，并且拥有真正光滑的拉丝金属纹理。你可以看看[Lasse]在苹果电视上快速输入文本的视频。

[https://www.youtube.com/embed/ZVBl-f-sF9c?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/ZVBl-f-sF9c?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)