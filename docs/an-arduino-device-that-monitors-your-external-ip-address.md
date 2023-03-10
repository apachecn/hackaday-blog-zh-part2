# 一个 Arduino 设备，用于监控您的外部 IP 地址

> 原文：<https://hackaday.com/2015/03/06/an-arduino-device-that-monitors-your-external-ip-address/>

爸爸安装了一个网络摄像头作为一个远程财产的监控摄像头。唯一的问题是，他们在这个地方能得到的唯一稳定的互联网连接是 DSL。这意味着网络摄像头的外部 IP 地址会经常改变；他们需要一种方法来跟踪外部 IP 地址的变化。那时[Bayres] [使用 Arduino 和以太网屏蔽建立了一个解决方案](http://hackaday.io/project/2495-external-ip-address-tracker "External IP tracker")。

该设备的主要功能是监控公共 IP 地址并报告任何变化。这通过首先向 checkip.dyndns.org 提出请求来实现。该网站只报告您当前的公共 IP 地址。[Bayres]使用名为 Textfinder 的 Arduino 库来搜索返回的字符串并识别 IP 地址。

然后，程序将当前值与之前的值进行比较。如果有任何变化，该程序将使用 Sendmail()函数联系 SMTP 服务器，并向[Beyres'] dad 发送电子邮件警报。该系统还包括一个小型液晶显示器。Arduino 将当前的 IP 地址输出到这个显示器上，这样就很容易检查连接。LCD 由 74HC595 [移位寄存器](http://hackaday.com/2013/02/07/learn-shift-registers-without-involving-a-microcontroller/ "Shift registers without micros")驱动，以节省 Arduino 上的引脚。

该系统还设计了一个非常光滑的设置界面。启动时，用户可以通过串行终端进入配置菜单。该设置菜单允许用户配置诸如 SMTP 服务器、电子邮件地址等选项。然后对这些变量进行编辑，并将其提交至 EEPROM，作为更永久的存储解决方案。每当系统启动时，这些值就会从 EEPROM 中读出，并返回到相应的变量中。这意味着您可以即时重新配置设备，而无需编辑源代码并重新上传。