# FPGAs 的门:TTL 电气属性

> 原文：<https://hackaday.com/2015/06/30/gates-to-fpgas-ttl-electrical-properties/>

在探索复杂逻辑的过程中，让我们讨论一下数字逻辑信号的电气特性。虽然数字信号有多种类型，但这里我们讨论的是更常见的基于电压的单端信号，而不是基于双导线的差分信号。

[![Simulated "Real Life"](img/52cfd21634e80ca8a25b3a84bdd2bfaf.png)](https://hackaday.com/wp-content/uploads/2015/06/square.jpg)

Single-ended Logic Signal

我认为大部分逻辑都属于两个主要领域之一，就今天的逻辑所使用的技术而言:双极和 CMOS。双极晶体管的特点是使用(非绝缘栅)晶体管，通常与基于晶体管逻辑(TTL)的逻辑电平相关联。随着 CMOS 技术的成熟，速度越来越快，能够驱动更高的电流，它开始扩大或提供双极性逻辑系列的替代方案。随着电源电压的下降和对低功耗需求的增加，这一点尤其明显。我们将在下一部分详细讨论 CMOS。

 [![TTL](img/a3f24934de2b9ce1b6b9ac0f62457f20.png "TTL")](https://hackaday.com/2015/06/30/gates-to-fpgas-ttl-electrical-properties/ttl-3/)  [![rtl](img/c4b00a07c50379d893797c2d6008c3af.png "rtl")](https://hackaday.com/2015/06/30/gates-to-fpgas-ttl-electrical-properties/rtl-3/)  [![dtl](img/a2399b65c1601e686aef80bcaccb7674.png "dtl")](https://hackaday.com/2015/06/30/gates-to-fpgas-ttl-electrical-properties/dtl/) 

TTL 是早期电阻晶体管逻辑(RTL)和二极管晶体管逻辑(DTL)技术自然发展的结果，早期 TTL 使用的标准成为众多逻辑家族遵循的标准。

[https://www.youtube.com/embed/b7koDIN4m-Q?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/b7koDIN4m-Q?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

### TTL 信号电压

当将两个逻辑门连接在一起时，基本上有四个感兴趣的电压:门的输出将产生的高电压和低电压，以及门的输入预期的高电压和低电压。
![Image2](img/00be2a061116c3c4ea0aaf78f5ba5bbe.png)

| **TTL 输出信号电压规格:** |
| 电压输出高 V [OH] | 2.4V |
| 电压输出低 V [OL] | . 4-.5V |
| **TTL 输入信号电压规格:** |
| 电压输入高 V [IH] | 2V |
| 电压输入低 V [IL] | . 8V |

简而言之，输出门产生的信号略大于输入门所需的信号；输出电压和输入电压之间的差异会造成一些信号损失和/或在等式中增加一些噪声。这种差异通常被称为噪声容限。

### TTL 电压兼容性

“标准”5 伏 TTL 和低压 3.3 伏 TTL(通常称为 LVTTL)的 TTL 信号电平通常相同或非常接近。虽然这听起来像是它们应该能够安全地连接在一起，但大多数 TTL/双极性逻辑系列都有一个规范，规定输入信号不能超过电源电压十分之几伏。一个 5 伏的门电路有可能在其输出端产生超过 3.3 伏的电压，这就是问题所在。

[![](img/28dcba3ccc76c1369873613a6055aea0.png)](https://hackaday.com/2015/06/30/gates-to-fpgas-ttl-electrical-properties/5v-resized/)

3.3V TTL Feeding 5V TTL

[![](img/d6b23c2be83e86753e89b77bca5d5e2a.png)](https://hackaday.com/2015/06/30/gates-to-fpgas-ttl-electrical-properties/3v-resized/)

5V TTL feeding 3.3v TTL

有些逻辑系列，如 74AHCT，可以承受比其输入电源更高的电压，但这是 CMOS 系列，将在下一篇文章中讨论。

### 肖特基逻辑

在简要介绍双极性/TTL 系列之前，我先解释一下什么是“肖特基”系列逻辑器件，以及它的速度提升源于何处。

[![](img/2e208fdc5076aa9580053f03e18da566.png)](https://hackaday.com/wp-content/uploads/2015/06/schottky4.png)

当晶体管用作开关时，它会进入饱和状态。“晶体管饱和”的部分定义包括基极-发射极和基极-集电极结都正向偏置时的状态，然而，这里感兴趣的特性是，它关闭起来也很慢，因为在器件开始响应之前，积累了过量的电荷，必须首先将其排出。基极-集电极结上的肖特基二极管有效地将晶体管保持在“导通”的边缘，并防止过多的电荷积累。栅极中与肖特基二极管配对的晶体管通常被重绘，如上图右侧所示。

### TTL 逻辑系列

| **74** | 原始 TTL–一些零件仍然存在。 |
| **74LS** | 低功耗肖特基–良好的折衷速度与功耗/噪声比，价格低廉。 |
| **74S** | 肖特基——早期 TTL 的大锤，快速但沉重。 |
| **74AS** | 高级肖特基-当你真的要走得很快。 |
| **74ALS** | 先进的低功耗肖特基二极管–速度快、功耗低，但由于信号变化速度(压摆率)的原因，必须考虑噪声问题。 |
| **74F** | 飞兆半导体高级肖特基 TTL–快速、低功耗，根据我的经验，比 ALS 噪声小一点。 |
| **74L** | 低功耗–未广泛使用。 |
| **74H** | 高速——早期对更快速度的妥协，没有广泛使用。 |

这里可以看到基于双极性 TTL 的系列。上面的一些系列也能够吸收和流出大量电流，我们将来也会将它们与 CMOS 同类产品进行比较。

## 故障测验

最后，如果你还记得上一篇讨论基本逻辑的文章，我问了一下左边所示电路中的小故障风险。当“D”改变状态时会出现毛刺，因为理论上有一段时间，当一个等式(称为一项)在另一项变为真之前停止为真。事实上，D 信号本身是不需要的，因为这两组项在其他方面是相同的

[![](img/62df20dcbf1cef624962c28183b0cbd1.png)](https://hackaday.com/2015/06/30/gates-to-fpgas-ttl-electrical-properties/example1-resized/)[![](img/1ea8b2a8a4f8c09a2bfd434e07971901.png)](https://hackaday.com/2015/06/30/gates-to-fpgas-ttl-electrical-properties/example2/)

看右边的电路；既然各项不再相等，我们是否已经排除了故障的可能性？