# 宜家 Dioder 流光溢彩黑客

> 原文：<https://hackaday.com/2013/03/28/ikea-dioder-ambilight-hack/>

宜家 Dioder LED 灯组有很多问题。[Lambertus]想要创造一种简单实惠的流光溢彩，同时尽量减少硬件改动。他还希望任何人都能轻松复制他的作品。他最近写信分享了他的成功解决方案。

定制归结为三个主要步骤:将 ICSP 连接器导线焊接到 Dioder PCB 上的测试点，将 PIC 编程器连接到 ICSP 端口(并重新编程)，并将 5V RS-232 设备连接到 ICSP 端口。对兰伯特来说，软件是整个过程中最困难的部分。PIC16F684 不包含所需的 UART 和 PWM 控制器，所以他必须变得狡猾。幸运的是，他为我们做了所有的工作，并列出必要的清单。他在网站上创建的十六进制文件。

通过增加对 boblight 的支持，他的新流光溢彩与他的媒体中心配合得非常好。休息之后有一小段演示视频。

[https://www.youtube.com/embed/GyrZ5HvOXz0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/GyrZ5HvOXz0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)