# 被动式蓝牙无钥匙进入系统

> 原文：<https://hackaday.com/2013/09/29/passive-bluetooth-keyless-entry-system/>

现代智能钥匙允许您将钥匙链放在口袋或钱包中，而您只需抓住把手把门拉开。[Phil]决定放弃智能钥匙，而是用他的 Android 手机实现了一个被动蓝牙无钥匙进入系统。汽车制造商可能不太可能很快接受基于手机的钥匙，而且[菲尔]承认他的原型带来了巨大的挑战。然而，他建造的东西看起来相当诱人。如果汽车和手机通过蓝牙配对，车门就会解锁。走出范围，当连接断开时，汽车会自动锁定。

他的建筑使用了一个 Arduino Mega，带有一个 BlueSMiRF Silver 蓝牙板，可以主动搜索他的手机，如果在范围内，就启动连接。车门通过双通道继电器模块直接解锁，车内的 LED 指示灯显示系统状态。脉冲灯表示它正在搜索手机，而实心环表示连接已建立。

我们希望[菲尔]将实现更多的功能，这样我们就可以让我们的口袋更轻一点。休息后观看他的原型视频演示，然后查看我们最近在这里报道的大量与汽车相关的黑客:添加智能刹车灯的 [OpenXC 界面](http://hackaday.com/2013/09/15/smart-brake-lights-and-more-with-openxc/ "Smart Brake lights and more with OpenXC")，或[moto brain](http://hackaday.com/2013/09/13/motobrain-a-bluetooth-controlled-pdu/ "Motobrain: A Bluetooth controlled PDU")，它可以让你通过蓝牙控制辅助电气系统。

[https://www.youtube.com/embed/RnQieNPgA6E?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/RnQieNPgA6E?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)