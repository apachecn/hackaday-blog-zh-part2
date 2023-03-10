# Pi 2 意味着更快的 GPIO

> 原文：<https://hackaday.com/2015/03/27/the-pi-2-means-faster-gpio/>

Raspberry Pi 是一个很好的机器，可以学习闪烁针的来龙去脉，但是要做任何需要快速闪烁针的事情，你最好用 BeagleBone。这是多年来的传统智慧，现在更新的 Raspberry Pi 2 出来了，人们期望你能更快地眨眼。[数据在这里，是的，你可以](http://codeandlife.com/2015/03/25/raspberry-pi-2-vs-1-gpio-benchmark/)。

测试方法是将 PicoScope 5444B 连接到 GPIO 引脚上的一个引脚，并尽可能快地在 0 和 1 之间切换。最初的测试并不令人鼓舞。Python 的最大频率约为 70 kHz，Ruby 很糟糕，只有带原生库的 C 对有趣的东西有用——22 MHz。

使用相同的实验设置，Raspberry Pi 2 大约快 2 到 3 倍。最快的仍然是 C 原生库，最高不到 42 MHz。其他语言和库要慢得多，但是 RPi。GPIO Python 库 stukk 看到了 2.5 倍的增长。