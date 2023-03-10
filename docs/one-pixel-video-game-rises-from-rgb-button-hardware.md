# 一个像素的视频游戏从 RGB 按钮硬件中崛起

> 原文：<https://hackaday.com/2013/08/17/one-pixel-video-game-rises-from-rgb-button-hardware/>

![rgb-button-one-pixel-video-game](img/400630c721dfe2ca7e506ae5b97b6389.png)

这个项目完全是组件驱动的。[Christopher]和[Robert]想尝试带有 RGB 背光选项的按钮。他们找到了上面显示的那个，看起来很棒。应该可以，因为一个单位要 20 多美元。他们想出的是一个一像素的视频游戏，它的工作原理就像一个配色版本的西蒙说。该按钮将显示目标颜色一会儿。然后，玩家按住按钮，让其颜色逐渐变淡。在正确的时刻释放它会产生绿色闪光，错误的阴影会导致红色闪光。

他们为这个项目配备了一台 Arduino Mega，因为它触手可及。一大块 protoboard 被用作屏蔽，它包括按钮本身，通过一些限流电阻连接到驱动 LED 的引脚。还有一个触动开关，可以启动 AVR 的复位引脚。

当试图让 LED 在所有颜色范围内褪色时,[Christopher]遇到了一个常见的问题。由于我们的眼睛不会以相同的方式检测低强度和高强度光的变化，所以您无法在 PWM 中使用线性变化并获得平滑的结果。他通过使用高斯曲线设置强度等级来解决这个问题。

[https://www.youtube.com/embed/udD6vIgGDao?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/udD6vIgGDao?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)