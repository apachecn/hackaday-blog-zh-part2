# 在飞行模拟器中使用遥控发射器

> 原文：<https://hackaday.com/2015/01/26/using-rc-transmitters-with-flight-simulators/>

现在是冬天，这意味着恶劣的天气和很少几天可以忍受飞行遥控飞机和直升机。[sjtrny]已经花了一个赛季与遥控飞行模拟器的一些实践时间。他一直在使用一个旧的 Xbox 360 控制器，但这真的不适合正确的 RC 模拟-一个更好的解决方案是使用他的普通 RC 发射器作为计算机外设。

在计算机上使用 RC 发射器的通常方式是购买 USB 模拟器适配器，通过发射器上的端口模拟 USB 游戏手柄。购买一个这样的适配器意味着要等一周才能发货，所以[sjtrny] [顺理成章地做了自己的](http://sjtrny.com/posts/2015/1/26/interfacing-an-rc-radio-with-your-computer.html)。

通常，USB 模拟器适配器插入用于“伙伴盒”的发射器上的 3.5 毫米插孔，但[sjtrny]有一个额外的接收器。由于接收器只是向伺服系统输出信号，这为 Arduino 监听提供了一个非常简单的接口。将接收器上的方向舵、升降舵、副翼和油门信号连接到 Arduino 后，一段简单的代码和 [UnoJoy 库](https://github.com/AlanChatham/UnoJoy)就可以让任何 Arduino 和 RC 接收器变成 USB 操纵杆。

[sjtrny]经历了这个项目的第二次硬件迭代，推出了 Teensy 3.1。这个版本在操纵杆轴上有更高的分辨率，代码的布局也不算太糟糕。对于那些在恶劣天气中无法休息的遥控飞机飞行员来说，这是一个很好的项目，对于你可能有的备用接收器来说，这也是一个很好的用途。