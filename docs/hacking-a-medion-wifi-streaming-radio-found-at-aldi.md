# 黑掉在阿尔迪发现的 Medion 无线流媒体收音机

> 原文：<https://hackaday.com/2013/06/21/hacking-a-medion-wifi-streaming-radio-found-at-aldi/>

![hacking-medion-streaming-wifi](img/cdce600c35f39bba5a46cfffad04dba5.png)

在 Aldi 购物时，[Aaron Christophel]偶然发现了这款 Medion 流媒体设备，它可以通过 WiFi 连接到您的家庭网络，并可以作为互联网收音机使用。他忍不住买了一个，回家后就设法在这个设备上做了不少黑客操作。

他的第一个任务是拆卸硬件。对电路板的检查显示，这显然是一个 USB 迷你插孔的闲置足迹。他添加了这个组件，以为这样可以让他把它连接到电脑上，但是没有成功。为了进一步调查这个问题，他使用难以猜测的凭证 root 和密码连接到设备的串行端口。它运行 Linux 内核，lsusb 命令显示 usb 被启用为主机模式。这意味着你可以附加大容量存储…甜！

他还做了一些固件黑客。上图是刷新他修改过的图像文件的确认屏幕。这导致了一个自定义的闪屏启动时。