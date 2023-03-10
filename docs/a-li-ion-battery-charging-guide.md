# 锂离子电池充电指南

> 原文：<https://hackaday.com/2014/09/21/a-li-ion-battery-charging-guide/>

虽然[pinomelean 的] [锂离子电池指南](http://www.instructables.com/id/Li-ion-battery-charging/)听起来主题有点具体，但你会发现其中详细讨论了许多可充电电池的基础知识。不知道什么是 [C-rate 是](http://batteryuniversity.com/learn/article/what_is_the_c_rate)？噗噗。卷起袖子，让我们深入一些理论。

就像你需要一个提醒一样，如果处理不当，许多类型的锂电池容易爆炸:正确的充电技术是必不可少的。[pinomelean]提供了一个充电周期中涉及的典型阶段的详细分类，并在将注意力转向实际方面之前，提供了一些关于降低电压阈值的优势的提示:从头开始设计自己的充电器电路。

该电路本身基于几个 LM324 运算放大器，产生一个电流和电压受限的电源。电压限制为 4.2V，电流可调:从 160mA 到 1600mA。这种充电器可能需要几个小时来给电池充电，但它是安全的，并且[pinomelean]对该设备的逐步描述有助于准确说明该过程是如何工作的。

[谢谢曼萨尔沃]