# 建立在线网络带宽监视器

> 原文：<https://hackaday.com/2013/12/15/build-an-in-line-network-bandwidth-monitor/>

[Kurt]想知道他的网络发生了什么。他已经在支持 DD-WRT 的路由器上使用了带宽检查软件，但他想听听其他人的意见。所以他建造了自己的网络监视器。【库尔特】从[建造无源以太网分接头](http://hackaday.com/2008/09/14/passive-networking-tap/)开始。然后他需要一个网络接口芯片来满足他的需求。Arduinos 使用的普通 Wiznet 芯片不允许对原始数据包进行足够的处理，所以他改用了一种[微芯片 ENC624J600](http://ww1.microchip.com/downloads/en/DeviceDoc/39935b.pdf) (PDF)。微芯片控制器允许他计算原始以太网数据包中的字节数。

以太网接口完成后，[Kurt]将注意力转向一个微控制器来运行这个节目。他从一个 Arduino 开始，但缺乏调试很快就把他送到了 Atmel Studio 中的一个 Atmega128。在基本电路工作后，[Kurt]切换到 PIC24F 芯片。随着数据最终从电路中出来，他能够说他最初对带宽的粗略计算是错误的。[Kurt]创建了一个 PCB 来容纳微控制器，然后编写了一个 Python 程序来绘制电路的数据输出。带宽曲线与 DD-WRT 的曲线非常吻合。现在他只需要一个[巨型 LED 矩阵](http://hackaday.com/2013/10/26/an-impressively-large-led-matrix/)来展示他当前的网络统计数据！