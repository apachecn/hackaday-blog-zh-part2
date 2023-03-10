# 按键嗅探器隐藏作为一个墙疣，是可怕的

> 原文：<https://hackaday.com/2015/01/14/keystroke-sniffer-hides-as-a-wall-wart-is-scary/>

对于我们这些担心无线设备安全的人来说，时不时会发生一些事情，甚至会吓到已经偏执的人。最新的是来自[Samy]的设备，它能够通过嗅探和解密键盘无线协议中使用的 RF 信号来记录微软键盘的击键。哦，[整个设备伪装成一个 USB 壁式电源适配器](http://samy.pl/keysweeper/)。

该设备是由一个 Arduino 或 Teensy 连接到一个 NRF24L01+ 2.4GHz 射频芯片上实现的，该芯片可以进行嗅探。一旦 Arduino 的固件被加载，两个芯片加上一个 USB 充电电路(用于为 USB 设备充电和保持伪装)就与锂电池一起被塞进一个更大的 USB 充电器的塑料外壳中。检索嗅探数据的选项是 SPI 串行闪存芯片或 GSM 模块，用于通过 SMS 自动发送数据。

这里可怕的事情并不是这个设备的存在，而是微软键盘的加密不够出色，提供了一种虚假的安全感。这也给我们敲响了警钟，那些我们甚至看都不看一眼的东西可能正是不太光彩的人可能会利用他们可以得到的任何信息的地方。休息之后，请继续观看该设备的运行视频，并确保在[Samy]的网页上查看该项目的更多详细信息，包括源代码和原理图。

感谢[朱迪]的提示！

[https://www.youtube.com/embed/WqkmGG0biXc?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/WqkmGG0biXc?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)