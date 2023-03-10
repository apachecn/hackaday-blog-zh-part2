# 在 USB VoIP 电话中发现协议

> 原文：<https://hackaday.com/2014/11/02/discovering-the-protocol-in-a-usb-voip-phone/>

[Daniel]拿起一个便宜的 USB 手机和他的 VoIP 提供商一起使用，盒子里有一张 CD，里面有所有能让这个手机和 Windows 一起工作的软件。[Daniel]正在他的主战台上运行 Linux，使得附带的 CD 变得一文不值。在 Linux 下使用手机会是一个问题；虽然扬声器和麦克风工作正常，但按钮和屏幕却不行。没问题，然后:[【丹尼尔】只是摆弄命令行，直到他想通了](http://danman.eu/blog/cheap-usb-skype-voip-phone-protocol-discovery/)。

手机作为声卡和 HID 设备出现在 Linux 盒子上。声卡显然是扬声器和麦克风，而按钮和显示器则是 HID 设备。[Daniel]通过在 HID 设备上运行 hexdump 并按下几个按钮来检查这一点。他的怀疑得到了证实，用一点点 Python 就能轻松读懂按钮。

弄清楚了手机上的扬声器、麦克风和按钮之后，[丹尼尔]将注意力转向了手机上他尚未攻克的一个电子部件:显示屏。在向手机发射一些随机数据后，显示屏闪烁并显示出一个杂乱的像素块，确认显示屏是通过 HID 驱动程序控制的。加载 [usbsnoop](http://sourceforge.net/projects/usbsnoop/) 查看原始软件如何更新 screed 向[Daniel]显示显示器接受的数据格式，使他能够控制这部 VoIP 电话中的一切。