# 恶意的树莓 Pi 电源板看起来有点吓人

> 原文：<https://hackaday.com/2012/10/04/malicious-raspberry-pi-power-strip-looks-a-bit-scary/>

你在这里看到的是一个硬塞进电源板的树莓派。这个想法是[利用这个板的力量和低成本成为一个隐形的网络观察设备](http://gnurds.com/index.php/2012/10/02/raspberry-pi-power-strip/)。它的威力与动力 Pwn 的[相似，但至少要便宜 1100 美元！](http://hackaday.com/2012/07/22/power-pwns-price-tag-is-as-dangerous-as-its-black-hat-uses/)

事实上，当你把你的以太网插入这个“电涌保护器”时，它就开始嗅探你的流量，这并没有吓到我们。穿过 RPi 本身的主接线有点让人不安。你可以说我们保护过度，但我们希望在高压和低压元件之间有一些屏蔽。但除此之外，其余的黑客是相当坚实的。那个用绝缘胶带包着的东西是电路板本身的电源转换器。这里没有显示，但是网卡是插在电涌保护器的 RJ-45 连接器上的。有一件事可能是很好的，包括一个 WiFi 小块，这样你就可以无线访问带。这将为其他窥探项目打开大门，如小型麦克风。