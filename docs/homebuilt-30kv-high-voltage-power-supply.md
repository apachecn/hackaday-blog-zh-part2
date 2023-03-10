# 自制 30kV 高压电源

> 原文：<https://hackaday.com/2013/09/23/homebuilt-30kv-high-voltage-power-supply/>

如果你需要 30，000 伏电压来启动你的 ionocraft(升降机)或为其他 DIY 项目供电，那么就穿梭到 RimstarOrg 的 YouTube 频道，查看[Steven Dufresne]的[自制 30kV 电源](http://www.youtube.com/watch?v=GEuK1OdYxHk)。[Steven]在他的视频中包含的构造细节总是令人惊叹，尤其是对视觉学习者来说。如果你更喜欢文字而不是视频，他在 rimstar.org 的[很友好地分享了一个原理图和完整的文字记录。](http://rimstar.org/equip/30kv_pwr_supply.htm)

电源可以在输出端配置为 1.2kv–4.6kv 或 4kV–30kV，而在输入端需要 0-24V DC。在视频中，[Steven]尝试了两种电源。他的[自制的 8V 和 2.5A 的 DC 台式电源](http://rimstar.org/equip/24v_pwr_supply.htm)和一个额定 20V 1.8A DC 的笔记本电脑电源。几个常见的 2N3055 功率晶体管，适当瓦数的电阻器，一个反激式变压器和一个高压三倍频器是你所需要的。回扫变压器可以在旧的阴极射线管类型的电视中找到，他也详细介绍了这种结构的初级绕组。高压三倍频器[Steven]参考源可能有点难找到。他列出了三倍增器的几个替代品，但即使是这些也很少:NTE 521，西门子 76-1 N094，1895-641-045。在野外有很多[电压倍增器](http://en.wikipedia.org/wiki/Voltage_multiplier)的细节，但是记住这个三倍增器需要工作到 30kV。

休息后加入我们观看视频，并听取安全先生的一点建议。

如果你还没有乘坐自制的 [ionocraft](http://hackaday.com/2009/12/08/ionocraft-aka-lifters/) 到处旅行，那么高压电源有什么用？也许你需要给你的[狼獾爪子](http://hackaday.com/2013/05/31/already-impressive-wolverine-claws-now-energized-with-high-voltage/)或者[雷神之锤](http://hackaday.com/2013/05/02/high-voltage-thors-hammer-mjolnir-at-80000-volts/)充电。在结束这篇文章之前，我们不能不对 YouTube 上的[高压黑客大师](http://hackaday.com/2011/08/28/high-voltage-hacks-finale-do-not-try-this-under-any-circumstances/)【photonic induction】也就是现在的【Photonvids】大声疾呼。

安全先生的时间:
问:安全先生，这危险吗？
答——非常！除非你真的知道自己在做什么，否则不要尝试构建这样的东西。你很容易被输出和电路中的其它点杀死。操作此类电源时，请遵循[Steven 的]安全提示。关断后，记得将输出接地。高压三倍频器可以在其内部电容器中存储相当大的震动，因此要小心该设备本身。

[https://www.youtube.com/embed/GEuK1OdYxHk?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/GEuK1OdYxHk?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)