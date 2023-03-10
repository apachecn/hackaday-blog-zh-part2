# 一点润滑剂可以用很长时间。用你的数控机床

> 原文：<https://hackaday.com/2014/09/07/a-little-lubricant-goes-a-long-way-with-your-cnc-machine/>

[Peter]最近他的 CNC3020 路由器出现了一些位置重复性问题。问题主要出在 Z 轴上，经过测量，在移动 10 厘米后，偏离位置达 0.3 毫米。这可能看起来不多，但足以打破几个 1 毫米直径的端铣刀。X 轴和 Y 轴总体上看起来没问题。网上冲浪揭示了控制板的电源轨没有任何滤波电容，这可能是问题的原因。不幸的是，即使在添加了 cap 之后，定位问题仍然存在。沮丧之余，[Peter]开始了一项全面的调查,以找出为什么他的 Z 轴没有成功。

在一个数控系统中有两个主要部分，电子设备和物理机器。由于不知道系统的哪个部分存在问题，[Peter]决定快速交换 X 和 Z 通道，用 X 轴电子设备运行 Z 轴。这个问题在 Z 轴上仍然很明显，这意味着机器的机械结构有问题。将 Z 电子设备放回 Z 轴上，通过降低加速度和最大速度继续测试。定位误差仍然存在。由于 Z 电机可能是问题所在，因此决定交换 X 和 Z 电机，但在过程中途，问题变得明显。当试图用手旋转 Z 轴导螺杆时，明显缺乏平滑度，并且轴似乎跳了一圈！

必须拆卸 Z 轴才能接触到丝杠螺母和线性轨道。这揭示了[彼得的]问题的根源；没有润滑剂，不在线性轨道上，也不在导螺母或导螺杆上。随着时间的推移，未润滑的 Z 轴线性滚珠轴承在线性轨道中磨损出 4 个看起来粗糙的等距凹槽。轴承被冲洗掉，产生了数量惊人的金属粉尘，积聚在内部。清洗后，轴承被润滑，否则似乎没有损坏。由于铁轨上的凹槽仅在 4 个局部区域，它们被旋转了 45 度，因此轴承现在位于未受损区域。即使在清洁、润滑和旋转连杆后，轴承仍然感觉不到应有的光滑。由于替换轴承不可用，Z 轴被重新组装。在重新组装之前，还在丝杠和螺母上涂抹了润滑脂。

[Peter]对他的“修复”抱有很低的期望，但是在进行了更多的测试后，Z 轴似乎表现得更好；10 厘米行程的误差为 0.01 毫米。还不错！[Peter]不怕被这个 CNC3020 弄脏，他增加了一个[冷却系统](http://hackaday.com/2014/06/20/adding-spindle-direction-and-coolant-control-to-your-cnc-machine/)、[限位开关和一个 PWM 主轴控制](http://hackaday.com/2014/02/15/chinese-3020-cnc-machine-gets-some-upgrades/)。