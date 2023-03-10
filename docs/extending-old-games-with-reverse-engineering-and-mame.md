# 用逆向工程和 MAME 扩展旧游戏

> 原文：<https://hackaday.com/2013/03/27/extending-old-games-with-reverse-engineering-and-mame/>

对于去年的 Toorcamp，DorkbotPDX 的人帮助安装了机器人教堂。一个建立在 2084 年控制论起义预言基础上的宗教甚至对我们来说都有点深奥，所以呆瓜机器人的工作人员想办法让玩《机器人战士:2084》变得更真实一点。使用 MAME 和一些调试工具，他们[能够读取一台玩机器人](http://dorkbotpdx.org/blog/skinny/use_mames_debugger_to_reverse_engineer_and_extend_old_games)的机器的内存，从而将游戏扩展到现实世界。当玩家死亡时，灯光熄灭，警报声响起，机器人教堂的先知很高兴。

机器人教堂的设备包括一台运行 MAME 的机器，它带有机器人 ROM。当游戏中发生事件时，如激光射击或玩家死亡，物理事件将被触发。为了做到这一点，Dorkbot 团队在不同时间读取了 Robotron 游戏的内存位置，并找到了与游戏内事件相关的内存位置。在他们的博客上，他们使用 MAME 调试工具检测到一个玩家的死亡，然后可以转化为机器人教堂的物理幻影。

这是一个非常酷的黑客，我们希望我们有一个视频。让一个塑料幽灵在玩吃豆人的时候击中一个玩家似乎是一个很棒的主意，有了呆子机器人教程，这看起来相当容易。