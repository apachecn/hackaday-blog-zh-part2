# MSP430 触摸屏钢琴

> 原文：<https://hackaday.com/2013/05/05/msp430-touchscreen-piano/>

![msp430-touchscreen-piano](img/2e0d8cb4463efbf3dd8fc086808219d0.png)

[Rohit Gupta]来信分享了他围绕 TI Launchpad 开发的触摸屏钢琴项目。这为他提供了一种使用许多移动设备上都有的电阻式数字化仪进行探索的方法。这些只是简单地粘在液晶显示屏的顶部，替换物并不昂贵，但从旧硬件中抢救一个也是一种选择。

他做的第一件事就是用万用表测试数字化仪的四个输出。记录变化的电阻将有助于确保您正在读取正确的焊线，并且能够在开始编码之前将设置归零。[Rohit]使用 MSP430 芯片上的 ADC 从屏幕上读取数据。他使用 TI 的一个应用程序笔记中的算法将读数转换成 X 和 Y 坐标。

他将屏幕分成七列，每一列产生不同的音调。触摸该列上的更高或更低将改变产生的音符的音高。你可以在跳跃后的演示中听到这样的例子。

[https://www.youtube.com/embed/Aw63-2rYthY?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/Aw63-2rYthY?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)