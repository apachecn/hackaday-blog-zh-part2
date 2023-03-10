# Android VOIP 电话和 Raspberry Pi Mate 实现了有趣的 PBX 设置

> 原文：<https://hackaday.com/2012/11/26/android-voip-phone-and-raspberry-pi-mate-for-an-intriguing-pbx-setup/>

![](img/3954f8e237a4fca47eca73c0d1566477.png "rpi-and-android-voip-phone-pdx")

[沃德·蒙迪]发现了一个伟大的东西，他将 GXP-2200 电话和树莓派结合起来，创建了一个专用小交换机。所以 PBX 设置背后的想法有点像公司内部网。系统中的所有电话都分配有一个分机号码，可以使用内部系统功能，如语音邮件，并与外界共享电话线。在之前，我们已经讨论过[使用 RPi 作为 PBX，但是他这次使用的高科技电话将一切都结合得非常好。](http://hackaday.com/2012/08/22/building-a-pbx-setup-around-the-raspberry-pi/)

GXP-2200 的售价不到 200 美元。它运行安卓系统，有一个全彩色触摸屏，如上图所示。它以多媒体手机的身份进行营销，事实上它将 Skype 和谷歌语音带到了派对上。但它也提供六条 SIP 线路。硬件甚至似乎是为这种用途设计的，因为手机提供了第二个以太网端口，RPi 板可以连接到该端口。在这个例子中,[Ward]只需将 RPi 固定在手机的塑料支架上，并用一根 6 英寸的电缆将两者连接起来。从那里可以用手机的浏览器配置 PBX。对滑头来说怎么样？