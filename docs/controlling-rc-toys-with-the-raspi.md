# 用 Raspi 控制遥控玩具

> 原文：<https://hackaday.com/2014/06/03/controlling-rc-toys-with-the-raspi/>

![signal](img/49591927ecfc897fcae7526011757750.png)

利用快速 CPU 和直接映射到存储器的 GPIO 引脚，可以实现一个有趣的技巧，那就是 FM 发射器。只要足够快地打开和关闭一个插销，你就有了一个粗制滥造的发射机。[Brandon]看到了一些将 Raspberry Pi 变成 FM 无线电发射机的构建，并意识到许多玩具遥控车使用的频率与 Pi 可以传输的频率范围相同。实现[Pi 可以控制这些遥控车](http://brskari.wordpress.com/2014/06/02/turn-your-raspberry-pi-into-a-radio-controller-for-rc-vehicles/)并不困难，只需使用一段连接到 GPIO 引脚的电线。

[最初的黑客](http://hackaday.com/2012/12/10/transmit-fm-using-raspberry-pi-and-no-additional-hardware/)将 Pi GPIO 引脚转换为 FM 发射器，将 GPIO 引脚映射到存储器，以大约 100 MHz 的频率在存储器中循环，并添加小数分频器来稍微调整频率，将其转换为 FM 发射器。廉价的遥控汽车通常监听 27 和 49 兆赫的无线电信号。用 Pi 控制遥控汽车是可能的，这并不需要花费太多时间。

这种想法的唯一问题是，大多数遥控汽车使用脉冲调制。RC 发射器发送“前进”命令时，会发送一个同步脉冲，然后是一系列脉冲和暂停。频率完全不变，这是最初的 FM 代码所不具备的。[布兰登]意识到，如果他只是把频率提高到遥控汽车听不到的频率，那就会被记为 0。

剩下的就是找出遥控卡车的指令代码。为此，[布兰登]决定蛮力将是最好的选择。用一个脚本和一个摄像头，他循环通过所有可能的组合，直到摄像头检测到一辆移动的卡车。如果你问我们的话，我觉得很巧妙。当然，更复杂的命令需要示波器，但现在[Brandon] [有一个装满所有代码的 git](https://github.com/bskari/pi-rc)来控制一辆带有 Pi 的廉价遥控汽车。