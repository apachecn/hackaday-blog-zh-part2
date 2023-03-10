# 使用 XBEE 传输 MIDI 信号

> 原文：<https://hackaday.com/2015/07/17/transmitting-midi-signals-with-xbee/>

当你想摆脱线缆的束缚，在键盘上尽情摇滚时，你会怎么做？你当然可以制作你自己的无线键盘！为了完成工作，[kr1st0f]内置了一个[逻辑翻译电路](http://ayatomm.com/index.php/2015/07/10/wireless-midi-radio-xbee/)。这允许他使用 XBEE 将 MIDI 信号从 MIDI 键盘直接传输到远程系统。

[kr1st0f]从一个 MIDI 键盘开始，该键盘具有带有 5 针 DIN 连接器的旧式 MIDI 接口。许多新键盘只有一个 USB 接口，这将使事情变得复杂。主电路使用一个[光隔离器](http://hackaday.com/2014/10/10/macgyvered-optoisolator-is-a-great-introduction/)和一个逻辑转换器来完成工作。MIDI 信号从标准 5V 逻辑转换为 3.3V，以便与 XBEE 一起工作。

XBEE 本身也需要进行配置，以便该电路正常工作。MIDI 信号以每秒 31，250 位的速率工作。另一方面，XBEE 的默认工作速率为 9,600 bps。[kr1st0f]首先必须重新配置 XBEE 以 MIDI 比特率运行。他通过串行接口连接到 XBEE 并使用一系列 AT 命令来实现这一点。他还必须在 XBEE 模块中配置正确的 ID 号。当一切都结束后，他的新发射器电路可以将 MIDI 信号无线传输到与计算机相连的接收器电路。