# Arduino、电阻器和桶形插头浪费了数百万把酒店锁

> 原文：<https://hackaday.com/2012/07/25/arduino-resistor-and-barrel-plug-lay-waste-to-millions-of-hotel-locks/>

![](img/4494fa5ce4ea11edf5e8ce41638a62ad.png "brocious-onity-hotel-lock-arduino")

这种普通酒店钥匙卡锁的安全缺陷简直愚蠢透顶。仔细看上图。这是一个开着的旅馆房间的门。他手里拿着的设备是一个 Arduino，连接到门锁的外部。从攻击者插入设备到门被打开大约需要 200 毫秒。是的，在不到 1/4 秒的时间里，一个 Arduino 可以打开数百万个正在使用的锁中的任何一个。

在 Blackhat 会议上，[Cody Brocious] 揭露了 Onity 可编程钥匙卡锁的漏洞。显然，锁外面的 DC 桶形插孔用作单线协议接口。一旦建立了通信，就可以从任何一把锁上读取 32 位的站点代码，并立即用来开门。没有**认证或加密**用于混淆这种攻击。更糟糕的是，你甚至可以读出万能钥匙和万能钥匙的密码。这些代码有助于使用“魔法”钥匙打开系统中各种不同的门。

我们对简单的酒店口角并不陌生。但是，存在这种漏洞的数字锁怎么可能被出售呢？真的！？

这里有关于这个漏洞的白皮书和 T2 演讲的幻灯片。

[via [Reddit](http://www.reddit.com/r/arduino/comments/x4tmg/hacker_uses_arduino_to_gain_access_to_4_million/)