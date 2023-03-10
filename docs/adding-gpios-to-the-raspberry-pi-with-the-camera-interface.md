# 使用相机接口将 GPIOs 添加到 Raspberry Pi

> 原文：<https://hackaday.com/2014/07/24/adding-gpios-to-the-raspberry-pi-with-the-camera-interface/>

![GPIOs](img/c2f343e606fdd02d301ccc1989966e72.png)

Raspberry Pi Model B+刚刚发布，现在每个人都有更多的 GPIO 引脚可以使用。对于数百万使用两年前 Pi 版本的人来说，我们仍然停留在同样的老问题上:大标题上有 17 个 GPIOs，就切换引脚而言，也就这样了。

Pi 上的 Broadcom SoC 的 GPIO 引脚远远多于大接头上的 GPIO 引脚，其中一些引脚连接到 CSI 摄像头接口。[这些 gpio 可以用几根扁平电缆](http://blog.everpi.net/2014/06/raspberry-pi-expandir-gpio-interface-csi.html)(葡萄牙语， [Google Translatrix](https://translate.google.com/translate?sl=auto&tl=en&js=y&prev=_t&hl=en&ie=UTF-8&u=http%3A%2F%2Fblog.everpi.net%2F2014%2F06%2Fraspberry-pi-expandir-gpio-interface-csi.html&edit-text=&act=url) )断开，给你多四个 gpio，这种技术也可以用于新的扩展型号 B+

CSI 摄像机连接器有两条直接连接到摄像机的 I C 线，在 Linux 中可控制为 GPIO0 和 GPIO1。CSI 连接器上还有两个 GPIO 连接器，可控制为 GPIO5 和 GPIO21。通过小心地将电线切片并焊接到扁平电缆上，这些 GPIO 线可以在试验板上断开。

下面有一个视频演示了这些 GPIO 线用于控制几个 led。当然，使用 CSI 连接器 GPIO 线，任何使用普通 Raspi GPIO 的事情都是可能的。

[https://www.youtube.com/embed/p5YnFI9Pq1A?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/p5YnFI9Pq1A?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)