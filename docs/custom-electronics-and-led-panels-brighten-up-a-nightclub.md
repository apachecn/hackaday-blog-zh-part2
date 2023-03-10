# 定制电子产品和 LED 面板点亮了夜总会

> 原文：<https://hackaday.com/2014/05/31/custom-electronics-and-led-panels-brighten-up-a-nightclub/>

![ledPanels](img/b59be3a44640a4b310464196d14e0517.png)

当[罗伯特]面临挑战时，他[没有退缩](http://armageddon421.de/?p=335 "LED panels in the night club")。他的朋友梦想将一些旧的 LED 面板安装到朋友的夜总会的天花板上，从而重复利用这些面板。每个面板由一个由五个红色、绿色和蓝色 led 组成的网格组成，每个面板总共有 75 个 led。这听起来像是一个相对简单的任务，但有一些注意事项。首先，面板附带的控制器盒只能控制 16 个面板，而这位朋友想要控制其中的 24 个。第二，控制器的唯一输入设备是一个红外遥控器。这位朋友想要一种简单的方法让 DJ 控制面板的颜色，而红外线遥控器是无法做到的。哦，是的，他也给了[罗伯特]仅仅三周的时间来完成这件事。

[罗伯特]开始是建立一个可以复制的电路来控制每个面板。这个电路的大脑是一个 ATtiny2313。对于专家组之间的沟通，[Robert]选择使用 [DMX 协议](http://en.wikipedia.org/wiki/DMX512 "DMX protocol")。考虑到 DMX 通常用于控制舞台灯光效果，这是一个不错的选择。选择了 [SN75176 IC](http://www.mikrocontroller.net/part/SN75176 "SN75176 IC") 来处理这种通信。在匆忙制造这种 PCB 的过程中，[Robert]没有意识到 led 面板被设计为公共阴极，而他的 25 个闪亮的新 PCB 被设计为与公共阳极设计一起工作。为了解决这个问题，他用 p 沟道 MOSFET 替换了所有的 n 沟道 MOSFET。他还花了几个小时手动切断线路，给电路板重新布线。做完这一切后，他发现了另一个问题。LED 由与微控制器相同的 5V 电源供电。这导致电源问题，从而导致 ATtiny 不断复位。解决方案是增加一些电容。

点击休息时间，了解更多关于[Robert]LED 面板的信息。

至于软件，[罗伯特]完全填满了阿提尼的记忆。他用三个通道来控制红色、绿色和蓝色。他添加了第四个通道来控制预先设计的动画效果，如褪色、频闪和随机颜色。DIP 开关通常用于设置面板的地址，但还有第二个选项可将面板置于独立模式。在这种模式下，开关用于对面板进行编程，以执行特定的效果，无需 DMX 控制器。

现在面板都设计好了，可以工作了，[罗伯特]仍然需要一种方法来控制它们。他在 [Shackspace](http://shackspace.de/ "Shackspace") hackerspace 使用激光切割机设计实际的面板，然后在上面安装一堆按钮、开关和电位计。所有这些东西都通过一个性能板和一个手动连线电路连接到一个[天线上。另一个 SN75176 IC 用于控制面板的 DMX 通信。控制面板允许 DJ 在不同的预建动画效果、颜色效果之间切换，并且还可以改变动画的速度以匹配音乐的速度。](https://www.pjrc.com/store/teensy3.html "Teensy3")

[https://www.youtube.com/embed/mDyfunMEgC4?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/mDyfunMEgC4?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)