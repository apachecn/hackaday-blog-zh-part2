# Rigol DS1022C Hack 将其速度提升至 100MHz

> 原文：<https://hackaday.com/2013/05/16/rigol-ds1022c-hack-brings-it-up-to-100mhz-speed/>

![rigol-1022c-100MHz-hack](img/67262ed0b63141fd8c271f0a6af99ee0.png)

[Andreas Schuler]一直在摆弄他的 Rigol DS1022C 数字存储示波器。这是一个旧型号，可以以高达 25MHz 的频率捕获样本，但[Andreas]声称使用服务菜单黑客将该频率翻了两番。他的技术[改变设置以在 100Mhz](http://codenaschen.de/tichyblog/index.php?action=blog&entry=17_Hacking%20Rigol%20DS1022C%20DS1042C%20DS1062C%20DS1102C) 下使用 DS1022C。

通常像这样的攻击包括一些测试测量，以确认硬件确实以更高的速率采样，而不仅仅是*声称*它有能力这样做。如果你已经有了这个硬件平台，并决定自己尝试一下，我们很乐意在评论中听到你的意见。他的方法是从系统信息菜单进入一系列按钮。如果操作正确，这将添加一个以前没有的服务菜单选项。稍微导航一下，您就会看到上面的屏幕，在这里您可以将型号更改为 DS1102C。这是 1022 更强大的 100MHz 同类产品。

如果你认为你以前见过这种黑客攻击，那很可能是因为 Rigol 1052E 之前被固件黑客拉到了 100MHz。