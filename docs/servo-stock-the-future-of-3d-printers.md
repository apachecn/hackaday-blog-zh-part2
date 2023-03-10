# 伺服库存，3D 打印机的未来

> 原文：<https://hackaday.com/2014/05/26/servo-stock-the-future-of-3d-printers/>

如果你仔细想想，我们今天拥有的 RepRaps 和其他商用 3D 打印机与未来车间里的打印机完全不同。它们比需要的更贵，尽管 RepRap 项目已经存在了几年，但还没有人破解闭环控制的难题。Hackaday Projects 网站上的[mad hephaestus]、[Alex]和[Will]正在利用伺服系统研究 3D 打印的未来[，这是一种使用伺服系统和闭环控制的 delta 打印机，其价格约为传统 3D 打印机的四分之一。](http://hackaday.io/project/962)

打印机本身是一个 Kossel 衍生产品，经过高度修改，以展示一些有趣的技术。代替步进器，打印机有三个由伺服系统控制的轴。每个轴上都有一块包含磁性编码器和连续旋转伺服系统的小电路板。通过这种设置，这些家伙能够通过闭环控制获得每转 4096 步，可以驱动伺服系统 2 个节拍。

电子设备和固件是普通 3D 打印机装载的全新设计。主板使用 80MHz 的 Pic32。甚至主机和打印机之间的通信也被完全重新设计。该团队使用的不是 Gcode，而是 Bowler 协议 T1，这是一种通过串行、TCP/IP 或你能想到的任何其他通信协议发送数据包的系统。

下面是 ServoStock 在计算机上解释 Gcode 并将代码和运动学发送到打印机的视频。它似乎工作得很好，使用廉价的伺服系统和减少电子设备意味着这个项目可能是第一个打破 200 美元障碍的 3D 打印机。

 [https://www.youtube.com/embed/b0-EFWNfIOE?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/b0-EFWNfIOE?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)