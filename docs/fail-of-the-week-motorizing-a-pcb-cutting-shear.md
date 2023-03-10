# 本周失败:电动 PCB 剪切机

> 原文：<https://hackaday.com/2013/08/29/fail-of-the-week-motorizing-a-pcb-cutting-shear/>

本周的失败是试图用齿轮电机改装一个 PCB 剪切机。该项目由[戴维·库克]承担。顺便说一句，他和我们非常亲近，因为他的书*初学者机器人制造*让我们一开始就接触了黑客。

这款价值 200 美元的剪切工具是手动操作的，可以切割 1/16 英寸厚的木板。但是[大卫]真的需要转动曲柄来切割。这经常导致弯曲的板边缘。为了达到更高的精度，他决定进行改造。他从易贝采购了一台高扭矩发动机，交货价格约为 50 美元。

库存处理接口与一个方形轴出来的剪切机的变速箱。他认为这是连接马达最简单的方法。在移除齿轮箱盖后，他能够加工一些孔以将马达安装在外部。这涉及到一些有趣的技巧，比如在加工铸铁时不要使用润滑剂，以及一种加工方孔的技术，他需要与剪刀连接。

![fail-shear-coupler](img/f7756e3dcd97e542615bdd10d07fea9a.png)

尽管看起来如此光滑，发动机的测试却导致了彻底的失败。听到“砰”的一声巨响，马达开始转动。所有连接电机外壳和电机支架的螺丝都被剪断了。他认为他的机器零件没问题，但事实并非如此。试图移除螺钉导致六角键扭曲。更糟糕的是，马达的扭矩实际上扭曲了它自己的轴，耦合器上的固定螺钉在钢中挖出了深沟。那是很大的力量！

[![](img/f048b89313013c1abc93772c7842300b.png)](https://hackaday.com/2013/08/29/fail-of-the-week-motorizing-a-pcb-cutting-shear/01-fail-shear-damage/)

Sheared off screws

[![](img/0389f5b51daa28fa4882fe3881ce3597.png)](https://hackaday.com/2013/08/29/fail-of-the-week-motorizing-a-pcb-cutting-shear/02-fail-shear-damage/)

Twisted hex key

[![](img/5ed050457a190e4531073bf90a619bbf.png)](https://hackaday.com/2013/08/29/fail-of-the-week-motorizing-a-pcb-cutting-shear/03-fail-shear-damage/)

Damaged motor shaft

感谢[托马斯]发来[大卫]精彩失败报道的链接。

每周失败是一个每周三运行的黑客专栏。通过写下你过去的失败和[给我们发送一个故事](mailto:tips@hackaday.com?Subject=[Fail of the Week])的链接，或者发送你在互联网旅行中发现的失败记录的链接，帮助保持乐趣。