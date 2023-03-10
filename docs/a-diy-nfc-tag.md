# DIY NFC 标签

> 原文：<https://hackaday.com/2013/11/14/a-diy-nfc-tag/>

[Nicholas]使用 ATtiny84 微控制器、四个电阻、三个电容、一个二极管和一个天线构建了一个简单的 NFC 标签。它实现了 ISO 14443-3，这是一种识别卡标准，可以与大多数新智能手机中的 NFC 芯片组进行通信。

该标准使用[开关键控](http://en.wikipedia.org/wiki/On-off_keying)进行通信，这使得硬件比我们几年前看到的 [AVR RFID 标签](http://hackaday.com/2009/06/27/avr-rfid-tag/ "AVR RFID tag")稍微复杂一些。天线和可变电容器形成调谐在 13.56 MHz 的 LC 电路，这是协议的载波频率。二极管充当[包络检测器](http://en.wikipedia.org/wiki/Envelope_detector)，让微控制器恢复信号。

它可能不完全符合标准，但[Nicolas]成功地用他的 Lumia 620 手机测试了这款设备。该固件可在 [Google Code](https://code.google.com/p/simple-nfc/source/browse/trunk) 上获得，因此你可以将自己的标签数据编程到 main.c 中，构建固件，并发送一些 NFC 数据包。休息之后，您还可以观看该设备的演示。

[https://www.youtube.com/embed/1lhdr3zefUA?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/1lhdr3zefUA?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)