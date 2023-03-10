# 英特尔爱迪生的实践

> 原文：<https://hackaday.com/2014/09/10/hands-on-with-the-intel-edison/>

昨天，技术世界回荡着令人震惊的消息，苹果不能运行 CMS，旋转编码器只是为 Apple Watch 发明的，英特尔的开发者论坛被安排在苹果媒体马戏团之前。英特尔迄今最小的计算机爱迪生[也在](http://hackaday.com/2014/09/09/intel-releases-edison-a-computer-slightly-larger-than-an-sd-card/)发布。没有英特尔员工徽章的人很少会有这种很酷的小设备，幸运的是[他们中的一个人放了一个实践评论](http://blog.dimitridiakopoulos.com/2014/09/10/hands-on-intel-edison/)。

有很多评论问爱迪生有什么用处，[Dimitri]告诉我们爱迪生不仅仅是一个开发板。更好的比较是类似于[Raspberry Pi 计算模块](http://hackaday.com/2014/04/07/the-raspberry-pi-compute-module/)的东西——产品设计师可以围绕它构建一个设备的小电路板。这当然不是新闻，也不应该让任何人感到意外。无论如何，Edison 中使用的 70 针连接器并不适合高频插入。

##### 储备电平转换器

与树莓派或 Arduino Mega 相比，Edison 的 Arduino 分线板非常大。这是因为大量的电平转换器。Arduinos 可以在 3.3V 和 5V 下运行，Pi 使用稍微不常见的(至少对于业余爱好者市场来说)3.3V 逻辑，*大多数 Edison 在 1.8V 下运行，* 较小分线点上的所有用户可配置引脚都是 1.8V 逻辑。有人看到这个会炸了他们的爱迪生，所以别说我们没警告你。

##### 表演

[迪米特里]很想知道爱迪生有多强大。那里有一个非常好的芯片——Atom Z34XX——它的主频不足 500MHz。尽管有这种明显的性能限制，一些基准测试显示爱迪生可以工作在高达 615 MIPS。这大约是 Raspberry Pi B+性能的两倍，结合 OpenCV 跟踪进行 FFT 的真实测试让[Dimitri]很高兴。功耗？在中等负载下，爱迪生消耗大约 200 毫安。大量的数字运算和从无线电中释放出来的比特增加到最大 500 mA。算不上低功耗，但性能功耗比非常好。

##### 无线的

爱迪生上有两个收音机，一个用于蓝牙低能耗，另一个用于 a/b/g/n WiFi(是的，它支持接入模式)。片上天线是可以接受的，但要将信号发送到大厅下面的会议室，您可能需要连接一个外部天线。

##### Linux、编程和 Arduino

Edison 上的 Linux 不像 Raspberry Pi 那样是友好的 Debian 衍生版本。相反，英特尔正在使用专门为嵌入式环境设计的 Yocto。这不完全是一个发行版，而是一个构建系统。没有容易得到的东西。现在，这可能被视为一种限制，但是有进取心的内核向导[已经将 Debian 移植到英特尔 Galileo](https://communities.intel.com/message/218148) 上。对 Linux 的全面支持即将到来，但可能不是(正式)来自英特尔。

爱迪生推出了 Arduino 分线板，但 Arduino 兼容性实际上只是一个表象。英特尔重新设计了 Arduino IDE，因此它可以写文件，而不是切换引脚。这意味着任何可以写文件的编程语言都可以用爱迪生灯使 LED 闪烁。这只是个人喜好的问题，但是如果你的嵌入式开发理念是单芯片和 C 编译器，你最好使用 ATMega 和 UART。

##### 结束语

这不是一个 Raspi 杀手，一个 Beaglebone 杀手，一个 TI CC3200 杀手，或者一个 [ESP8266](http://hackaday.com/2014/08/26/new-chip-alert-the-esp8266-wifi-module-its-5/) 杀手。这是一个 x86 板，有 WiFi，蓝牙和 Linux，可以切换几个引脚。是不一样的东西。与众不同是好事。这意味着有更多的选择。