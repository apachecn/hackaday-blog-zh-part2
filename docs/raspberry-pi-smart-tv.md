# 树莓派智能电视

> 原文：<https://hackaday.com/2013/11/20/raspberry-pi-smart-tv/>

[Tony]认为他的“智能”LED 电视不够智能。所以他在里面塞了一个覆盆子馅饼。

打开他的 40 英寸海信智能 LED 电视的外壳，他发现逻辑板实际上有两个未使用的 USB 垫——真幸运！他从它们中取出 5V @ 500mA 来给 Pi 供电…后来他意识到这不是理想的解决方案——当电视关闭时，它也切断了 Pi 的电源。于是他拿出万用表探测电路板，这一次他找到了一个 5V 的电源，这个电源在设备插上电源时一直亮着。

接下来是树莓派的摆放。这台电视的内置扬声器并不太好，因为[Tony]使用的是环绕声系统，所以他决定更好地利用它们的空间。切掉格栅并移除整个组件给他留下了足够的空间来存放 Pi 并安装 3D 打印局域网和 USB 端口盖！

他正在运行 Raspbmc，这为电视提供了大量的功能。如果你不介意取消你的保修，这是一个伟大的黑客！