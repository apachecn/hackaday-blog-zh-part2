# 对 GPS 手表进行逆向工程以上传定制固件

> 原文：<https://hackaday.com/2014/08/10/reverse-engineering-a-gps-watch-to-upload-custom-firmwares/>

[![](img/cc3e8cf7137629ae59de586912be5578.png)](https://hackaday.com/wp-content/uploads/2014/08/kalenji300_anot.jpg)

有时 GPS 手表太好了，不能和它们的库存固件放在一起。[Renaud]打开他的卡伦吉 300 GPS 手表，[对其进行逆向工程](http://renaud.schleck.free.fr/montre_gps.php?lang=en)，以便上传他自己定制的固件。

第一步是在升级固件时嗅探 PC 和微控制器之间的串行流量，以了解所使用的协议和命令。[Renaud]然后打开手表，找出不同的测试点和组件。他使用他的带有 OpenOCD 的 buspirate 来提取现有的 STM32F103 固件。固件帮助他找到合适的值，存储在专用寄存器中，以便启动引导加载程序。

通过查看反汇编代码，他还发现了 SPI LCD 初始化序列，并发现它使用了与 ST7571 类似的控制器。他最终利用图形库编写了自己的程序。休息后请关注我们的演示视频。

[https://www.youtube.com/embed/m0BXtlJwMRo?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/m0BXtlJwMRo?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)