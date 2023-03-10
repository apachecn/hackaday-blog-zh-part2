# 穿过溪流的双 PIR 照片触发器

> 原文：<https://hackaday.com/2012/08/03/dual-pir-photo-trigger-by-crossing-the-streams/>

![](img/062224e4bc691a1325f76a68cd9ee38c.png "pir-photo-trigger-by-crossing-the-streams")

拍摄野生动物照片时，动作感应非常有效。但是，我们怎么能确定运动是在画面的中心呢？PIR 传感器在其整个观察范围内拾取运动。这真的不是可以瞄准的东西。但是如果你[使用两个 PIR 传感器，你可以监控一个聚焦区域的运动](https://getsatisfaction.com/triggertrap/topics/trigger_camera_through_the_aux_port_when_a_ir_beam_is_crossed)。

诀窍是使用逻辑电路。通过构建一个与门，您可以基于两个传感器重叠区域中的运动进行触发。在这种情况下，与门由分压器构成。PIR 传感器的输出连接到光触发器分配器连接的上方和下方。两者都有一个保护二极管，分压器经过调谐，因此两个 PIR 输出必须合二为一，以便将触发输入提高到电压阈值以上。关于[永远不要穿越溪流](http://www.youtube.com/watch?v=jyaLZHiJJnE)的事情到此为止。

[通过[触发陷阱](https://triggertrap.com/crossed-pir-sensors/)