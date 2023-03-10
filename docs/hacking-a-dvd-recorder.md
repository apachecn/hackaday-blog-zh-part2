# 黑进 DVD 录像机

> 原文：<https://hackaday.com/2014/02/16/hacking-a-dvd-recorder/>

[![Hacked DVD Recorder](img/45ff4d1e9663998e33a6cc91e0a63c93.png)](http://hackaday.com/2014/02/16/hacking-a-dvd-recorder/dvdr-hacked/)

[w00fer]想看看是否有可能对 DVD 刻录机进行任何修改。最初，我们的目标是升级内部硬盘以增加存储空间。然而，在打开 DVDR3570H 并找到一个服务端口后，他[决定看得更深一点](http://www.w00fer.nl/blog/philips-dvdr-service-mode-via-rs232/)。

将 RS232 转 USB 转换器连接到服务端口会导致数据混乱。原来，该端口使用的是 TTL 信号电平，而不是 RS232 电平。这可以通过使用 [MAX232](http://en.wikipedia.org/wiki/MAX232) 转换器 IC 构建转换器来解决。

转换器就位后，出现了维修菜单。它执行一些测试，并在设备启动时输出结果。之后，它会在提示符下等待命令。幸运的是，[w00fer]找到了列出可用命令的[维修手册](http://www.serwis-elektroniki.com.pl/BPS/pdf/et3028.pdf)。到目前为止，他已经能够生成测试模式，测试灯，改变显示文本，旋转硬盘驱动器，并读取设备信息。但是，接下来的步骤包括禁用 Macrovision 复制保护、转储 EEPROM 和 NVRAM 以及从硬盘复制数据。如果你认为你能帮上忙，就告诉他。