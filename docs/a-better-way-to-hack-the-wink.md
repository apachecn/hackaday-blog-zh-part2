# 破解传情动漫的更好方法

> 原文：<https://hackaday.com/2015/01/05/a-better-way-to-hack-the-wink/>

如果你正在寻找家庭自动化设备，你可能想看看 Wink Hub。它的价格是 50 美元，船上有六个收音机:WiFi、蓝牙、Z-Wave、Zigbee 和 433MHz Lutron 和 Kidde。这是在一个非常便宜的包中的疯狂的连接数量。以前也有过 pwnzor3d，[但是 dinnovative 有一个好得多的在这个设备上获得 root 的解决方案。](http://www.dinnovative.com/?p=348)

早期的方法是通过 URL 传递命令，这并不安全。新方法利用已经安装在 Wink 上的东西，特别是 [Dropbear](http://en.wikipedia.org/wiki/Dropbear_(software)) ，在 Wink hub 上生成公钥，并将该密钥安全地传输到另一台计算机上。完整的利用只是终端中的几行代码，但是一旦完成，你就有了一个根深蒂固的 Wink hub。

尽管 Wink hub 之前已经扎根了几次，但我们还没有看到任何利用这种硬件功能的东西。市场上没有另一种 50 美元的物联网无线电设备，我们渴望看到人们能拿出什么。如果你的眨眼做了什么，[在提示热线](http://hackaday.com/submit-a-tip/)上发送。