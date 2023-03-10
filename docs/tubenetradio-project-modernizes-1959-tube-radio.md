# TubeNetRadio 项目使 1959 年的电子管收音机现代化

> 原文：<https://hackaday.com/2015/05/03/tubenetradio-project-modernizes-1959-tube-radio/>

几年前，[卢克]偶然发现了一台旧电子管收音机。从那以后，他就想把它变成一个网络收音机，但从未真正着手。现在我们生活在一个只需 35 美元就能买到微型电脑的时代，[卢克]决定是时候完成他丢失已久的项目了。

他选择了树莓派作为他的项目的大脑，因为它是一种便宜且记录良好的产品，非常适合他想要做的事情。[Luk]有一个目标，尽可能少地修改收音机，以便让它既能播放互联网广播，又能播放本地存储的 MP3。1959 年的收音机当然很旧了，但它有一个你可能想不到的特点。它有一个辅助输入，前面有一个单独的音量旋钮。就像收音机本身一样，输入是单声道的。为了将 Raspberry Pi 连接到收音机上，[Luk]必须制作一个 1/8 英寸的立体声到香蕉插头适配器，这是一个伟大的解决方案，不需要对原始收音机进行任何修改。

WiFi 通过现成的 USB 无线模块接入。在评估接入无线电中某处的 5v 直流电源后，决定使用壁式电源为 Raspberry Pi 供电。墙上电源插座的插头插在收音机主开关的后面。这样收音机和树莓派就能一起打开和关闭。收音机外壳内有足够的空间放置所有这些附加组件。

RaspPi 可以通过 WiFi 网络完全控制，但有几个按钮连接到 GPIO 引脚，用于有限的手动控制。这些控制按钮完全安装在收音机外壳后面板上的圆形通风孔中。虽然按钮是可见的，但不需要进行永久性的修改！[Luk]报告说，一切都很好，收音机的原始功能也是如此。